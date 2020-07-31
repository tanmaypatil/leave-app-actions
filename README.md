# leave-app-actions
hasura actions repository for business validations

## Purpose of this repository
Hasura actions is a layer which specifically helps to expose a api on top of hasura 
  * business or field level validations can be done before graphql mutation or query is called .
  * expose a different interface to user interface then a pure database expose api

## Business validations for leave application 
  * Does user has sufficient leave balance to as per request
  * Is user making leave request on a weekend or corporate holiday .

