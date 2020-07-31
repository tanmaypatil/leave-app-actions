# leave application action repository
hasura actions repository for business validations for leave application .
Earlier this repository was part of leave-application repository .
However in order for each microservice  to be dockerised , have seperated them into seperate repository

## Stack
 * written in node.js and express.

## set up 
   Requires following enviornment variable : GRAPHQL_HOST
   
   GRAPHQL_HOST : http://host.docker.internal:8080/v1/graphql 
   Action will receive the input payload and call the graphql queries to perform operations.

## Purpose of this repository
Hasura actions is a layer which specifically helps to expose a api on top of hasura 
  * business or field level validations can be done before graphql mutation or query is called .
  * expose a different interface to user interface then a pure database expose api

## Business validations for leave application 
  * Does user has sufficient leave balance to as per request
  * Is user making leave request on a weekend or corporate holiday .

