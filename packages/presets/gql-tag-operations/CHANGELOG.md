# @graphql-codegen/gql-tag-operations-preset

## 1.2.1

### Patch Changes

- 6c898efe5: list all dependencies used by the package in the package.json
- Updated dependencies [6c898efe5]
  - @graphql-codegen/typescript@2.3.1

## 1.2.0

### Minor Changes

- 1e9a7e162: feat: support module augumentation for extending the types of gql functions from existing packages via the `augmentedModuleName` config option.

### Patch Changes

- Updated dependencies [1e9a7e162]
  - @graphql-codegen/gql-tag-operations@1.2.0

## 1.1.7

### Patch Changes

- Updated dependencies [5c37b9d11]
  - @graphql-codegen/typescript-operations@2.1.6

## 1.1.6

### Patch Changes

- 06dfd3958: fix: follow "useTypeImports" configuration
- 5394f19bb: prevent duplicate operations
- Updated dependencies [06dfd3958]
- Updated dependencies [25cd11d01]
- Updated dependencies [5394f19bb]
  - @graphql-codegen/gql-tag-operations@1.1.5
  - @graphql-codegen/typescript-operations@2.1.5

## 1.1.5

### Patch Changes

- @graphql-codegen/gql-tag-operations@1.1.4
- @graphql-codegen/typescript-operations@2.1.4
- @graphql-codegen/typed-document-node@2.1.4
- @graphql-codegen/typescript@2.2.2

## 1.1.4

### Patch Changes

- Updated dependencies [cfa0a8f80]
  - @graphql-codegen/typescript@2.2.1

## 1.1.3

### Patch Changes

- Updated dependencies [d6c2d4c09]
- Updated dependencies [8261e4161]
  - @graphql-codegen/typescript@2.2.0
  - @graphql-codegen/gql-tag-operations@1.1.3
  - @graphql-codegen/typescript-operations@2.1.3
  - @graphql-codegen/typed-document-node@2.1.3

## 1.1.2

### Patch Changes

- @graphql-codegen/gql-tag-operations@1.1.2
- @graphql-codegen/typescript-operations@2.1.2
- @graphql-codegen/typed-document-node@2.1.2
- @graphql-codegen/typescript@2.1.2

## 1.1.1

### Patch Changes

- @graphql-codegen/gql-tag-operations@1.1.1
- @graphql-codegen/typescript-operations@2.1.1
- @graphql-codegen/typed-document-node@2.1.1
- @graphql-codegen/typescript@2.1.1

## 1.1.0

### Minor Changes

- 0c0c8a92b: export new utility type `DocumentType`, for accessing the document node type.

  ```tsx
  import { gql, DocumentType } from '../gql';

  const TweetFragment = gql(/* GraphQL */ `
    fragment TweetFragment on Tweet {
      id
      body
    }
  `);

  const Tweet = (props: { tweet: DocumentType<typeof TweetFragment> }) => {
    return <div data-id={props.id}>{props.body}</div>;
  };
  ```

- 440172cfe: support ESM

### Patch Changes

- 290170262: ensure the generated identifier for referencing a document from the documents map is correct
- Updated dependencies [0c0c8a92b]
- Updated dependencies [24185985a]
- Updated dependencies [440172cfe]
- Updated dependencies [440172cfe]
  - @graphql-codegen/gql-tag-operations@1.1.0
  - @graphql-codegen/typed-document-node@2.1.0
  - @graphql-codegen/add@3.1.0
  - @graphql-codegen/typescript-operations@2.1.0
  - @graphql-codegen/typescript@2.1.0

## 1.0.1

### Patch Changes

- Updated dependencies [e8c8e9c06]
  - @graphql-codegen/typescript-operations@2.0.1

## 1.0.0

### Major Changes

- b0cb13df4: Update to latest `graphql-tools` and `graphql-config` version.

  ‼️ ‼️ ‼️ Please note ‼️ ‼️ ‼️:

  This is a breaking change since Node 10 is no longer supported in `graphql-tools`, and also no longer supported for Codegen packages.

### Minor Changes

- b0cb13df4: new plugin/preset gql-tag-operations

### Patch Changes

- Updated dependencies [d80efdec4]
- Updated dependencies [d80efdec4]
- Updated dependencies [b0cb13df4]
- Updated dependencies [b0cb13df4]
- Updated dependencies [bbdad95fd]
  - @graphql-codegen/typescript-operations@2.0.0
  - @graphql-codegen/gql-tag-operations@1.0.0
  - @graphql-codegen/typed-document-node@2.0.0
  - @graphql-codegen/typescript@2.0.0
  - @graphql-codegen/add@3.0.0
