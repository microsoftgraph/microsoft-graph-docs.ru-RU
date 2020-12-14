---
title: Кэш набор средств Microsoft Graph
description: Объяснить, как работает кэш и как настроить параметры, предоставляемые разработчикам
localization_priority: Normal
author: adchau
ms.openlocfilehash: f51b4f188fe8ec70f75a50e1d9de049459c97e14
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658710"
---
# <a name="microsoft-graph-toolkit-caching"></a>Кэш набор средств Microsoft Graph

Microsoft Graph набор средств кэшировать выбранные вызовы API Microsoft Graph. В настоящее время вызовы конечных точек пользователей, пользователей, контактов и фотографий кэшются по умолчанию в трех хранилищах IndexedDB.

Кэш можно просмотреть на панели разработчика. На **вкладке "Приложение"** в **области** хранилища перейдите на вкладку **IndexedDB.**

![devtools indexedDB](../images/indexedDBpanel.png)

## <a name="cache-configuration"></a>Конфигурация кэша

Считывать и записывать параметры кэша можно с помощью объекта статического `CacheService.config` класса. Он отформатирован, как показано ниже.

```TypeScript
let config = {
  defaultInvalidationPeriod: number,
  isEnabled: boolean,
  people: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  photos: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  users: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  presence: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  groups: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
};
```

Отдельные периоды недействительности кэша по умолчанию задействуются в объекте config и по умолчанию имеют общее значение `null` `defaultInvalidationPeriod` 3 600 000 мс (60 минут). Все переданные значения `config.x.invalidationPeriod` будут переопределяться. `defaultInvalidationPeriod`

Единственное исключение — хранилище присутствия, значение по умолчанию — 30 000 мс или 5 минут.

### <a name="examples"></a>Примеры

Чтобы отключить отдельный магазин, просто установите для свойств config этого магазина значение `isEnabled` false:
```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.isEnabled = false;
```
Отключение кэша **не очищает** кэш.

Изменение периода оценки аналогично:

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.invalidationPeriod = 1800000;
```

## <a name="clearing-the-cache"></a>Очистка кэша

Кэш автоматически очищается при выходе пользователя. Его также можно очистить вручную.

При очистке всех хранилищ в кэше метод класса очищает все хранилища, поддерживаемые `clearCaches()` `CacheService` службой CacheService.

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.clearCaches();
```

## <a name="creating-your-own-cache-stores"></a>Создание собственных хранилищ кэша

Если вы хотите создать и заполнить собственные хранилища кэша для настраиваемого компонента, можно использовать `CacheService` статический класс.

```JavaScript
CacheService.getCache(schema: CacheSchema, storeName: String);
```
> **Примечание.** Ссылка в вызове должна соответствовать одному из хранилищ, `storeName` `getCache()` указанных в `CacheSchema` объекте.

Объект `CacheSchema` — это словарь с парами "ключ-значение".

```TypeScript
import { CacheSchema } from '@microsoft/mgt';
const cacheSchema: CacheSchema = {
  name: string,
  stores: {
    store1: {},
    store2: {},
    ...
  },
  version: number
};
```

В следующем примере показана реализация кэша.

```TypeScript
import { CacheItem, CacheSchema, CacheService, CacheStore } from '@microsoft/mgt';

const cacheSchema: CacheSchema = {
  name: 'users',
  stores: {
    users: {},
    usersQuery: {}
  },
  version: 1
};

interface CacheUser extends CacheItem {
  user?: string;
}

// retrieves invalidation time from cache config
const getUserInvalidationTime = (): number =>
  CacheService.config.users.invalidationPeriod || CacheService.config.defaultInvalidationPeriod;

// checks for if cache is enabled
const usersCacheEnabled = (): boolean => CacheService.config.users.isEnabled && CacheService.config.isEnabled;

// declare the desired cache store
let cache: CacheStore<CacheUser>

// check if the cache is enabled
if (usersCacheEnabled()) {
  cache = CacheService.getCache<CacheUser>(cacheSchema, 'users');
  const user = await cache.getValue(query);

  // check if an item is retrieved, and if it's not expired
  if (user && getUserInvalidationTime() > Date.now() - user.timeCached) {
    return JSON.parse(user.user);
  }
}

// graph call
const graphRes = graph
  .api('me')
  .middlewareOptions(prepScopes('user.read'))
  .get();

// store graph result into the cache if cache is enabled
if (usersCacheEnabled()) {
  cache.putValue(userId, { user: JSON.stringify(graphRes) });
}
```
