## API Report File for "@backstage-community/plugin-github-deployments"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
/// <reference types="react" />

import { AnyApiFactory } from '@backstage/core-plugin-api/index';
import { ConfigurableExtensionDataRef } from '@backstage/frontend-plugin-api';
import { Entity } from '@backstage/catalog-model/index';
import { ExtensionDefinition } from '@backstage/frontend-plugin-api';
import { FrontendPlugin } from '@backstage/frontend-plugin-api';
import { JSX as JSX_2 } from 'react';
import { RouteRef } from '@backstage/frontend-plugin-api';

// @alpha (undocumented)
const _default: FrontendPlugin<
  {
    entityContent: RouteRef<undefined>;
  },
  {},
  {
    'api:github-deployments': ExtensionDefinition<{
      kind: 'api';
      name: undefined;
      config: {};
      configInput: {};
      output: ConfigurableExtensionDataRef<
        AnyApiFactory,
        'core.api.factory',
        {}
      >;
      inputs: {};
      params: {
        factory: AnyApiFactory;
      };
    }>;
    'entity-card:github-deployments/overview': ExtensionDefinition<{
      kind: 'entity-card';
      name: 'overview';
      config: {
        filter: string | undefined;
      };
      configInput: {
        filter?: string | undefined;
      };
      output:
        | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
        | ConfigurableExtensionDataRef<
            (entity: Entity) => boolean,
            'catalog.entity-filter-function',
            {
              optional: true;
            }
          >
        | ConfigurableExtensionDataRef<
            string,
            'catalog.entity-filter-expression',
            {
              optional: true;
            }
          >;
      inputs: {};
      params: {
        loader: () => Promise<JSX.Element>;
        filter?: string | ((entity: Entity) => boolean) | undefined;
      };
    }>;
  }
>;
export default _default;

// (No @packageDocumentation comment for this package)
```