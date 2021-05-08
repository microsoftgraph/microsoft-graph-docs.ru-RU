---
title: Кэширование Microsoft Graph Toolkit
description: В этой статье объясняется, как работает кэширование и как настроить параметры для разработчиков
localization_priority: Normal
author: adchau
ms.openlocfilehash: cef5c06c39ebad58e6a39f094427dea6a1b1be25
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266622"
---
# <a name="microsoft-graph-toolkit-caching"></a><span data-ttu-id="9db9b-103">Кэширование Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="9db9b-103">Microsoft Graph Toolkit caching</span></span>

<span data-ttu-id="9db9b-104">Microsoft Graph Toolkit поддерживает кэширование выбранных вызовов API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9db9b-104">The Microsoft Graph Toolkit supports caching of select Microsoft Graph API calls.</span></span> <span data-ttu-id="9db9b-105">Вызовы кэшироваться для каждого объекта, например людей, контактов, фотографий.</span><span class="sxs-lookup"><span data-stu-id="9db9b-105">Calls are being cached per entity, such as people, contact, photo.</span></span> <span data-ttu-id="9db9b-106">Это позволяет одному компоненту получать данные и другие компоненты для повторного использования без вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9db9b-106">This allows one component to retrieve the data and other components to reuse it without calling Microsoft Graph.</span></span>

> [!TIP]
> <span data-ttu-id="9db9b-107">Дополнительные сведения о том, какие объекты кэшются каждым компонентом, см. в документации компонента.</span><span class="sxs-lookup"><span data-stu-id="9db9b-107">For more information about which entities are cached by each component, see the component's documentation.</span></span>

<span data-ttu-id="9db9b-108">Базы данных, созданные mgt для кэшинга, префиксизются `mgt-` с .</span><span class="sxs-lookup"><span data-stu-id="9db9b-108">Databases created by mgt for caching are prefixed with `mgt-`.</span></span> <span data-ttu-id="9db9b-109">Данные для каждой сущности хранятся в отдельном хранилище объектов.</span><span class="sxs-lookup"><span data-stu-id="9db9b-109">The data for each entity is stored in a separate object store.</span></span> <span data-ttu-id="9db9b-110">Чтобы проверить кэш, используйте вкладку **Application** в панели разработчиков (средства F12) — в разделе **Хранение** нажмите на вкладку **IndexedDB.**</span><span class="sxs-lookup"><span data-stu-id="9db9b-110">To inspect the cache, use the **Application** tab in the developer panel (F12 tools) - under the **Storage** section, click on the **IndexedDB** tab.</span></span> 

![средства разработчика indexedDB](../images/indexedDBpanel.png)

## <a name="cache-configuration"></a><span data-ttu-id="9db9b-112">Конфигурация кэша</span><span class="sxs-lookup"><span data-stu-id="9db9b-112">Cache configuration</span></span>

<span data-ttu-id="9db9b-113">Вы можете читать и записывать параметры кэша с помощью объекта статического класса `CacheService.config`.</span><span class="sxs-lookup"><span data-stu-id="9db9b-113">You can read and write the cache options through the static class `CacheService.config` object.</span></span> <span data-ttu-id="9db9b-114">Он форматируется, как показано.</span><span class="sxs-lookup"><span data-stu-id="9db9b-114">It is formatted as shown.</span></span>

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
  response: {
    invalidationPeriod: number,
    isEnabled: boolean
  }
};
```

<span data-ttu-id="9db9b-115">Для отдельных периодов недействительности кэша в объекте конфигурации по умолчанию задано значение `null`, а общее значение по умолчанию для `defaultInvalidationPeriod` составляет 3 600 000 мс (60 минут).</span><span class="sxs-lookup"><span data-stu-id="9db9b-115">Individual cache invalidation periods are defaulted to `null` in the config object, and default to the general `defaultInvalidationPeriod` value of 3,600,000 ms (60 minutes).</span></span> <span data-ttu-id="9db9b-116">Любое значение, переданное в `config.x.invalidationPeriod`, переопределяет `defaultInvalidationPeriod`.</span><span class="sxs-lookup"><span data-stu-id="9db9b-116">Any value passed into `config.x.invalidationPeriod` will override `defaultInvalidationPeriod`.</span></span>

<span data-ttu-id="9db9b-117">Единственным исключением является хранилище присутствия со значением по умолчанию 300 000 мс, или 5 минут.</span><span class="sxs-lookup"><span data-stu-id="9db9b-117">The presence store is the only exception, and has a default value of 300000 ms, or 5 minutes.</span></span>

### <a name="examples"></a><span data-ttu-id="9db9b-118">Примеры</span><span class="sxs-lookup"><span data-stu-id="9db9b-118">Examples</span></span>

<span data-ttu-id="9db9b-119">Чтобы отключить хранилище, просто задайте для `isEnabled` в свойствах конфигурации хранилища значение false:</span><span class="sxs-lookup"><span data-stu-id="9db9b-119">To individual disable a store simply set the value of `isEnabled` in that store's config properties to false:</span></span>
```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.isEnabled = false;
```
<span data-ttu-id="9db9b-120">Отключение кэша **не** очищает кэш.</span><span class="sxs-lookup"><span data-stu-id="9db9b-120">Disabling the cache does **not** clear the cache.</span></span>

<span data-ttu-id="9db9b-121">Аналогичным образом можно изменить период недействительности:</span><span class="sxs-lookup"><span data-stu-id="9db9b-121">Changing the invalditation period is similar:</span></span>

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.invalidationPeriod = 1800000;
```

## <a name="clearing-the-cache"></a><span data-ttu-id="9db9b-122">Очистка кэша</span><span class="sxs-lookup"><span data-stu-id="9db9b-122">Clearing the cache</span></span>

<span data-ttu-id="9db9b-123">Кэш автоматически очищается, когда пользователь выходит. Его также можно очистить вручную.</span><span class="sxs-lookup"><span data-stu-id="9db9b-123">The cache is automatically cleared when the user signs out. It can also be cleared manually.</span></span>

<span data-ttu-id="9db9b-124">Чтобы очистить все хранилища в кэше, обслуживаемые CacheService, используется метод `clearCaches()` класса `CacheService`.</span><span class="sxs-lookup"><span data-stu-id="9db9b-124">The clear all the stores in the cache, the `clearCaches()` method of the `CacheService` class will clear every store maintained by the CacheService.</span></span>

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.clearCaches();
```

## <a name="creating-your-own-cache-stores"></a><span data-ttu-id="9db9b-125">Создание собственных хранилищ кэша</span><span class="sxs-lookup"><span data-stu-id="9db9b-125">Creating your own cache stores</span></span>

<span data-ttu-id="9db9b-126">Если вы хотите создать и заполнить собственные хранилища кэша для настраиваемых компонентов, можно использовать статический класс `CacheService`.</span><span class="sxs-lookup"><span data-stu-id="9db9b-126">If you want to create and populate your own cache stores for your custom components, you can use the `CacheService` static class.</span></span>

```JavaScript
CacheService.getCache(schema: CacheSchema, storeName: String);
```
> <span data-ttu-id="9db9b-127">**Примечание.** Объект `storeName`, на который вы ссылаетесь в вызове `getCache()`, должен соответствовать одному из хранилищ, перечисленных в объекте `CacheSchema`.</span><span class="sxs-lookup"><span data-stu-id="9db9b-127">**Note:** The `storeName` you reference in the call to `getCache()` must match one of the stores listed in your `CacheSchema` object.</span></span>

<span data-ttu-id="9db9b-128">Объект `CacheSchema` является словарем с парами "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="9db9b-128">The `CacheSchema` object is a dictionary with the key/value pairs.</span></span>

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

<span data-ttu-id="9db9b-129">В примере ниже показана реализация кэша.</span><span class="sxs-lookup"><span data-stu-id="9db9b-129">The following example shows the cache implementation.</span></span>

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
