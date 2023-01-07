# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] - 2023-01-09
### Added
- New endpoint to translate todos: curl https://9r18bk9ir7.execute-api.us-east-1.amazonaws.com/Prod/todos/<id>/<lang>

## [1.0.1] - 2023-01-05
### Added
- 80% coverage in unit tests
- Fixed error in Production Jenkins pipeline: AttributeError: module 'lib' has no attribute 'OpenSSL_add_all_algorithms'

## [1.0.0] - 2022-12-23
### Added
- Create todo: curl -X POST https://9r18bk9ir7.execute-api.us-east-1.amazonaws.com/Prod/todos --data '{ "text": "Learn Serverless" }'
- List all todos: curl https://9r18bk9ir7.execute-api.us-east-1.amazonaws.com/Prod/todos
- Get a todo: curl https://9r18bk9ir7.execute-api.us-east-1.amazonaws.com/Prod/todos/<id>
- Update a todo: curl -X PUT https://9r18bk9ir7.execute-api.us-east-1.amazonaws.com/Prod/todos/<id> --data '{ "text": "Learn python and more", "checked": true }'
- Delete a todo: curl -X DELETE https://9r18bk9ir7.execute-api.us-east-1.amazonaws.com/Prod/todos/<id>