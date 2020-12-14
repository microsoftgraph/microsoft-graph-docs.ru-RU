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
# <a name="microsoft-graph-toolkit-caching"></a><span data-ttu-id="335e3-103">Кэш набор средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="335e3-103">Microsoft Graph Toolkit caching</span></span>

<span data-ttu-id="335e3-104">Microsoft Graph набор средств кэшировать выбранные вызовы API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="335e3-104">The Microsoft Graph Toolkit supports caching of select Microsoft Graph API calls.</span></span> <span data-ttu-id="335e3-105">В настоящее время вызовы конечных точек пользователей, пользователей, контактов и фотографий кэшются по умолчанию в трех хранилищах IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="335e3-105">Currently, calls to the users, person, contact, and photo endpoints are cached by default in three IndexedDB stores.</span></span>

<span data-ttu-id="335e3-106">Кэш можно просмотреть на панели разработчика.</span><span class="sxs-lookup"><span data-stu-id="335e3-106">You can view the cache on the developer panel.</span></span> <span data-ttu-id="335e3-107">На **вкладке "Приложение"** в **области** хранилища перейдите на вкладку **IndexedDB.**</span><span class="sxs-lookup"><span data-stu-id="335e3-107">On the **Application** tab, in the **Storage** pane, go to the **IndexedDB** tab.</span></span>

![devtools indexedDB](../images/indexedDBpanel.png)

## <a name="cache-configuration"></a><span data-ttu-id="335e3-109">Конфигурация кэша</span><span class="sxs-lookup"><span data-stu-id="335e3-109">Cache configuration</span></span>

<span data-ttu-id="335e3-110">Считывать и записывать параметры кэша можно с помощью объекта статического `CacheService.config` класса.</span><span class="sxs-lookup"><span data-stu-id="335e3-110">You can read and write the cache options through the static class `CacheService.config` object.</span></span> <span data-ttu-id="335e3-111">Он отформатирован, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="335e3-111">It is formatted as shown.</span></span>

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

<span data-ttu-id="335e3-112">Отдельные периоды недействительности кэша по умолчанию задействуются в объекте config и по умолчанию имеют общее значение `null` `defaultInvalidationPeriod` 3 600 000 мс (60 минут).</span><span class="sxs-lookup"><span data-stu-id="335e3-112">Individual cache invalidation periods are defaulted to `null` in the config object, and default to the general `defaultInvalidationPeriod` value of 3,600,000 ms (60 minutes).</span></span> <span data-ttu-id="335e3-113">Все переданные значения `config.x.invalidationPeriod` будут переопределяться. `defaultInvalidationPeriod`</span><span class="sxs-lookup"><span data-stu-id="335e3-113">Any value passed into `config.x.invalidationPeriod` will override `defaultInvalidationPeriod`.</span></span>

<span data-ttu-id="335e3-114">Единственное исключение — хранилище присутствия, значение по умолчанию — 30 000 мс или 5 минут.</span><span class="sxs-lookup"><span data-stu-id="335e3-114">The presence store is the only exception, and has a default value of 300000 ms, or 5 minutes.</span></span>

### <a name="examples"></a><span data-ttu-id="335e3-115">Примеры</span><span class="sxs-lookup"><span data-stu-id="335e3-115">Examples</span></span>

<span data-ttu-id="335e3-116">Чтобы отключить отдельный магазин, просто установите для свойств config этого магазина значение `isEnabled` false:</span><span class="sxs-lookup"><span data-stu-id="335e3-116">To individual disable a store simply set the value of `isEnabled` in that store's config properties to false:</span></span>
```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.isEnabled = false;
```
<span data-ttu-id="335e3-117">Отключение кэша **не очищает** кэш.</span><span class="sxs-lookup"><span data-stu-id="335e3-117">Disabling the cache does **not** clear the cache.</span></span>

<span data-ttu-id="335e3-118">Изменение периода оценки аналогично:</span><span class="sxs-lookup"><span data-stu-id="335e3-118">Changing the invalditation period is similar:</span></span>

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.invalidationPeriod = 1800000;
```

## <a name="clearing-the-cache"></a><span data-ttu-id="335e3-119">Очистка кэша</span><span class="sxs-lookup"><span data-stu-id="335e3-119">Clearing the cache</span></span>

<span data-ttu-id="335e3-120">Кэш автоматически очищается при выходе пользователя. Его также можно очистить вручную.</span><span class="sxs-lookup"><span data-stu-id="335e3-120">The cache is automatically cleared when the user signs out. It can also be cleared manually.</span></span>

<span data-ttu-id="335e3-121">При очистке всех хранилищ в кэше метод класса очищает все хранилища, поддерживаемые `clearCaches()` `CacheService` службой CacheService.</span><span class="sxs-lookup"><span data-stu-id="335e3-121">The clear all the stores in the cache, the `clearCaches()` method of the `CacheService` class will clear every store maintained by the CacheService.</span></span>

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.clearCaches();
```

## <a name="creating-your-own-cache-stores"></a><span data-ttu-id="335e3-122">Создание собственных хранилищ кэша</span><span class="sxs-lookup"><span data-stu-id="335e3-122">Creating your own cache stores</span></span>

<span data-ttu-id="335e3-123">Если вы хотите создать и заполнить собственные хранилища кэша для настраиваемого компонента, можно использовать `CacheService` статический класс.</span><span class="sxs-lookup"><span data-stu-id="335e3-123">If you want to create and populate your own cache stores for your custom components, you can use the `CacheService` static class.</span></span>

```JavaScript
CacheService.getCache(schema: CacheSchema, storeName: String);
```
> <span data-ttu-id="335e3-124">**Примечание.** Ссылка в вызове должна соответствовать одному из хранилищ, `storeName` `getCache()` указанных в `CacheSchema` объекте.</span><span class="sxs-lookup"><span data-stu-id="335e3-124">**Note:** The `storeName` you reference in the call to `getCache()` must match one of the stores listed in your `CacheSchema` object.</span></span>

<span data-ttu-id="335e3-125">Объект `CacheSchema` — это словарь с парами "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="335e3-125">The `CacheSchema` object is a dictionary with the key/value pairs.</span></span>

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

<span data-ttu-id="335e3-126">В следующем примере показана реализация кэша.</span><span class="sxs-lookup"><span data-stu-id="335e3-126">The following example shows the cache implementation.</span></span>

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
