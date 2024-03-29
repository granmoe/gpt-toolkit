# Next

- Deprecate/archive this lib and put update at top of README
- Playground link from README (very basic - codesandbox or replit or whatev)
- Enforce object schema at top level?
- Understand conditional type assertion in return better - super weird and interesting

# Tests

- more retry scenarios
  - updateModelParams
  - assert number of HTTP calls and failed etc
- parse
  - Zod example
  - updateModelParams
  - custom maxParseRetries
- trimTokens overage
- pass in various model params
- e2e / scenarios that combine functionality tested in existing tests (retry + parse + trimTokens etc)

# Future

- Make retry aware of delay time in OpenAI response and incorporate "jitter" and the other stuff the official client does
- Consider throwing custom error from parse instead? Would make types cleaner. Then we only retry if it’s custom error, so people can opt out by just not throwing that error.
- Support "name" in messages and token counting
- Allow passing in custom maxTokensPerRequest (for custom (e.g. fine-tuned) models)
  - Throw error if people override a known model's maxTokensPerRequest tho

# Misc

- Cool logo
- Get added to this https://platform.openai.com/docs/libraries/community-libraries
  - Our library has significantly more downloads than any of the others, except openai-api, but that hasn't had a new version in two years
  - Submitted 12/23/23
