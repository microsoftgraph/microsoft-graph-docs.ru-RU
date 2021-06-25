---
title: Расширенные возможности запросов для объектов каталога Azure AD
description: Объекты каталога Azure AD поддерживают расширенные возможности запросов для эффективного доступа к данным.
author: Licantrop0
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 7ecd514de1d1be4fea7606b62ca7060e6c15ba08
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118649"
---
# <a name="advanced-query-capabilities-on-azure-ad-directory-objects"></a><span data-ttu-id="03606-103">Расширенные возможности запросов для объектов каталога Azure AD</span><span class="sxs-lookup"><span data-stu-id="03606-103">Advanced query capabilities on Azure AD directory objects</span></span>

<span data-ttu-id="03606-104">В Azure AD постоянно добавляются новые возможности, повышается стабильность, доступность и производительность этого решения. Одновременно ведется работа и над усовершенствованием Microsoft Graph для масштабирования и эффективного доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="03606-104">As Azure AD continues to deliver more capabilities and improvements in stability, availability, and performance, Microsoft Graph also continues to evolve and scale to efficiently access the data.</span></span> <span data-ttu-id="03606-105">Одно из направлений этого усовершенствования заключается в усилении поддержки возможностей расширенных запросов для различных объектов Azure AD и их свойств.</span><span class="sxs-lookup"><span data-stu-id="03606-105">One way is through Microsoft Graph's increasing support for advanced query capabilities on various Azure AD objects and their properties.</span></span> <span data-ttu-id="03606-106">Например, добавление операторов **Not** (`NOT`), **Not equals** (`ne`) и **Ends with** (`endsWith`) к параметру запроса `$filter` в октябре 2020 г.</span><span class="sxs-lookup"><span data-stu-id="03606-106">For example, the addition of **Not** (`NOT`), **Not equals** (`ne`), and **Ends with** (`endsWith`) operators on the `$filter` query parameter in October 2020.</span></span>

<span data-ttu-id="03606-107">Механизм запросов Microsoft Graph использует хранилище индексов для выполнения запросов.</span><span class="sxs-lookup"><span data-stu-id="03606-107">The Microsoft Graph query engine uses an index store to fulfill query requests.</span></span> <span data-ttu-id="03606-108">Чтобы добавить поддержку дополнительных возможностей запросов для некоторых свойств, индексирование этих свойств теперь происходит на отдельном сервере.</span><span class="sxs-lookup"><span data-stu-id="03606-108">To add support for additional query capabilities on some properties, these properties are now indexed in a separate server.</span></span> <span data-ttu-id="03606-109">Благодаря этому отдельному индексированию в Azure AD расширена поддержка и повышена производительность запросов.</span><span class="sxs-lookup"><span data-stu-id="03606-109">This separate indexing allows Azure AD to increase support and improve the performance of the query requests.</span></span> <span data-ttu-id="03606-110">Тем не менее, эти расширенные возможности запросов по умолчанию недоступны. Запрашивающий должен установить для заголовка **ConsistencyLevel** значение `eventual`, *а также*, за исключением `$search`, использовать параметр запроса `$count` (в виде [сегмента URL-адреса](/graph/query-parameters#other-odata-url-capabilities) или строки запроса `$count=true`).</span><span class="sxs-lookup"><span data-stu-id="03606-110">However, these advanced query capabilities are not available by default but, the requestor must also set the **ConsistencyLevel** header set to `eventual` *and*, with the exception of `$search`, use the `$count` query parameter (either as a [URL segment](/graph/query-parameters#other-odata-url-capabilities) or `$count=true` query string).</span></span> <span data-ttu-id="03606-111">Заголовок **ConsistencyLevel** и `$count` называются *расширенными параметрами запроса*.</span><span class="sxs-lookup"><span data-stu-id="03606-111">The **ConsistencyLevel** header and `$count` are referred to as *advanced query parameters*.</span></span>

<span data-ttu-id="03606-112">Например, если нужно получить только учетные записи неактивных пользователей, можно выполнить любой из этих запросов, использующих параметр запроса `$filter`.</span><span class="sxs-lookup"><span data-stu-id="03606-112">For example, if you wish to retrieve only inactive user accounts, you can run either of these queries that use the `$filter` query parameter.</span></span>

+ <span data-ttu-id="03606-113">Используйте параметр запроса `$filter` с оператором `eq`.</span><span class="sxs-lookup"><span data-stu-id="03606-113">Use the `$filter` query parameter with the `eq` operator.</span></span> <span data-ttu-id="03606-114">Этот запрос будет работать по умолчанию, то есть этот запрос не требует расширенных параметров запроса.</span><span class="sxs-lookup"><span data-stu-id="03606-114">This request will work by default, that is, the request does not require the advanced query parameters.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_users_enabled"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled eq false
```

+ <span data-ttu-id="03606-115">Используйте параметр запроса `$filter` с оператором `ne`.</span><span class="sxs-lookup"><span data-stu-id="03606-115">Use the `$filter` query parameter with the `ne` operator.</span></span> <span data-ttu-id="03606-116">Этот запрос не поддерживается по умолчанию, поскольку оператор `ne` поддерживается только в расширенных запросах.</span><span class="sxs-lookup"><span data-stu-id="03606-116">This request is not supported by default because the `ne` operator is only supported in advanced queries.</span></span> <span data-ttu-id="03606-117">Поэтому необходимо добавить заголовок **ConsistencyLevel**, для которого должно быть указано значение `eventual`*, а также* использовать строку запроса `$count=true`.</span><span class="sxs-lookup"><span data-stu-id="03606-117">Therefore, you must add the **ConsistencyLevel** header set to `eventual` *and* use the `$count=true` query string.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_users_not_enabled"
} -->
```msgraph-interactive
https://graph.microsoft.com/v1.0/users?$filter=accountEnabled ne true&$count=true
ConsistencyLevel: eventual
```

<span data-ttu-id="03606-118">Эти расширенные возможности запросов поддерживаются только для объектов Azure AD, то есть для следующих ресурсов и их взаимосвязей, производных от [directoryObject](/graph/api/resources/directoryobject):</span><span class="sxs-lookup"><span data-stu-id="03606-118">These advanced query capabilities are supported only on Azure AD objects, that is, the following resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject):</span></span>

- [<span data-ttu-id="03606-119">application</span><span class="sxs-lookup"><span data-stu-id="03606-119">application</span></span>](/graph/api/resources/application)
- [<span data-ttu-id="03606-120">orgContact</span><span class="sxs-lookup"><span data-stu-id="03606-120">orgContact</span></span>](/graph/api/resources/orgcontact)
- [<span data-ttu-id="03606-121">device</span><span class="sxs-lookup"><span data-stu-id="03606-121">device</span></span>](/graph/api/resources/device)
- [<span data-ttu-id="03606-122">group</span><span class="sxs-lookup"><span data-stu-id="03606-122">group</span></span>](/graph/api/resources/group)
- [<span data-ttu-id="03606-123">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="03606-123">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal)
- [<span data-ttu-id="03606-124">users</span><span class="sxs-lookup"><span data-stu-id="03606-124">users</span></span>](/graph/api/resources/user)

<span data-ttu-id="03606-125">В следующей таблицы приведены сценарии запросов для объектов каталога, поддерживаемые только в расширенных запросах.</span><span class="sxs-lookup"><span data-stu-id="03606-125">The following table lists query scenarios on directory objects that are supported only in advanced queries.</span></span>

| <span data-ttu-id="03606-126">Описание</span><span class="sxs-lookup"><span data-stu-id="03606-126">Description</span></span>                                                              | <span data-ttu-id="03606-127">Пример</span><span class="sxs-lookup"><span data-stu-id="03606-127">Example</span></span>                                                                                                                                                                                                                                                                                                                                                                                                                              |
|:-------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="03606-128">Использование `$count` в качестве сегмента URL-адреса</span><span class="sxs-lookup"><span data-stu-id="03606-128">Use of `$count` as a URL segment</span></span>                                         | <span data-ttu-id="03606-129">[GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%2F%24count&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups/$count`</span><span class="sxs-lookup"><span data-stu-id="03606-129">[GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%2F%24count&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups/$count`</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="03606-130">Использование `$count` в качестве параметра строки запроса</span><span class="sxs-lookup"><span data-stu-id="03606-130">Use of `$count` as a query string parameter</span></span>                              | <span data-ttu-id="03606-131">[GET](https://developer.microsoft.com/graph/graph-explorer?request=servicePrincipals%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../servicePrincipals?$count=true`</span><span class="sxs-lookup"><span data-stu-id="03606-131">[GET](https://developer.microsoft.com/graph/graph-explorer?request=servicePrincipals%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../servicePrincipals?$count=true`</span></span>                                                                                                                                                     |
| <span data-ttu-id="03606-132">Использование `$search`</span><span class="sxs-lookup"><span data-stu-id="03606-132">Use of `$search`</span></span>                                                         | <span data-ttu-id="03606-133">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24search%3D%22displayName%3ABrowser%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$search="displayName:Browser"`</span><span class="sxs-lookup"><span data-stu-id="03606-133">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24search%3D%22displayName%3ABrowser%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$search="displayName:Browser"`</span></span>                                                                                                                     |
| <span data-ttu-id="03606-134">Использование `$orderby` для выбранных свойств</span><span class="sxs-lookup"><span data-stu-id="03606-134">Use of `$orderby` on select properties</span></span>                                   | <span data-ttu-id="03606-135">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$count=true`</span><span class="sxs-lookup"><span data-stu-id="03606-135">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$count=true`</span></span>                                                                                                               |
| <span data-ttu-id="03606-136">Использование `$filter` с оператором `endsWith`</span><span class="sxs-lookup"><span data-stu-id="03606-136">Use of `$filter` with the `endsWith` operator</span></span>                            | <span data-ttu-id="03606-137">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40outlook.com')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@outlook.com')`</span><span class="sxs-lookup"><span data-stu-id="03606-137">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40outlook.com')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@outlook.com')`</span></span>                                                                                       |
| <span data-ttu-id="03606-138">Использование `$filter` и `$orderby` в одном и том же запросе</span><span class="sxs-lookup"><span data-stu-id="03606-138">Use of `$filter` and `$orderby` in the same query</span></span>                        | <span data-ttu-id="03606-139">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24filter%3DstartsWith(displayName%2C%20'Box')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$filter=startsWith(displayName, 'Box')&$count=true`</span><span class="sxs-lookup"><span data-stu-id="03606-139">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24filter%3DstartsWith(displayName%2C%20'Box')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$filter=startsWith(displayName, 'Box')&$count=true`</span></span>                       |
| <span data-ttu-id="03606-140">Использование `$filter` с операторами `startsWith` для определенных свойств</span><span class="sxs-lookup"><span data-stu-id="03606-140">Use of `$filter` with the `startsWith` operators on specific properties.</span></span> | <span data-ttu-id="03606-141">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DstartsWith(mobilePhone%2C%20'25478')%20OR%20startsWith(mobilePhone%2C%20'25473')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=startsWith(mobilePhone, '25478') OR startsWith(mobilePhone, '25473')&$count=true`</span><span class="sxs-lookup"><span data-stu-id="03606-141">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DstartsWith(mobilePhone%2C%20'25478')%20OR%20startsWith(mobilePhone%2C%20'25473')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=startsWith(mobilePhone, '25478') OR startsWith(mobilePhone, '25473')&$count=true`</span></span> |
| <span data-ttu-id="03606-142">Использование `$filter` с операторами `ne` и `NOT`</span><span class="sxs-lookup"><span data-stu-id="03606-142">Use of `$filter` with `ne` and `NOT` operators</span></span>                           | <span data-ttu-id="03606-143">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`</span><span class="sxs-lookup"><span data-stu-id="03606-143">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`</span></span>                     |
| <span data-ttu-id="03606-144">Использование `$filter` с операторами `NOT` и `startsWith`</span><span class="sxs-lookup"><span data-stu-id="03606-144">Use of `$filter` with `NOT` and `startsWith` operators</span></span>                   | <span data-ttu-id="03606-145">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=%2Fusers%3F%24filter%3DNOT%20startsWith(displayName%2C%20'Conf')%26%24count%3Dtrue&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=NOT startsWith(displayName, 'Conf')&$count=true`</span><span class="sxs-lookup"><span data-stu-id="03606-145">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=%2Fusers%3F%24filter%3DNOT%20startsWith(displayName%2C%20'Conf')%26%24count%3Dtrue&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=NOT startsWith(displayName, 'Conf')&$count=true`</span></span>                                                                |
| <span data-ttu-id="03606-146">Использование функции OData cast с другим параметром запроса</span><span class="sxs-lookup"><span data-stu-id="03606-146">Use of OData cast with another query parameter</span></span>                           | <span data-ttu-id="03606-147">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true`</span><span class="sxs-lookup"><span data-stu-id="03606-147">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true`</span></span>                                                                                             |

> [!NOTE]
> <span data-ttu-id="03606-148">Эти расширенные возможности запросов недоступны в клиентах Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="03606-148">These advanced query capabilities are not available in Azure AD B2C tenants.</span></span>

## <a name="support-for-filter-on-properties-of-azure-ad-directory-objects"></a><span data-ttu-id="03606-149">Поддержка фильтрации по свойствам объектов каталога Azure AD</span><span class="sxs-lookup"><span data-stu-id="03606-149">Support for filter on properties of Azure AD directory objects</span></span>

<span data-ttu-id="03606-150">Свойства объектов каталога ведут себя по-разному в отношении поддержки параметров запросов.</span><span class="sxs-lookup"><span data-stu-id="03606-150">Properties of directory objects behave differently in their support for query parameters.</span></span> <span data-ttu-id="03606-151">Ниже приведены распространенные сценарии для объектов каталога:</span><span class="sxs-lookup"><span data-stu-id="03606-151">The following are common scenarios for directory objects:</span></span>

+ <span data-ttu-id="03606-152">Свойства с одинаковыми именами в ресурсах каталога поддерживают одинаковые операторы `$filter`.</span><span class="sxs-lookup"><span data-stu-id="03606-152">Properties with the same name across directory resources support the same `$filter` operators.</span></span> <span data-ttu-id="03606-153">Например, свойство **createdDateTime**, доступное в ресурсах **application**, **group**, **organization** и **user**.</span><span class="sxs-lookup"><span data-stu-id="03606-153">For example, the **createdDateTime** property is available in **application**, **group**, **organization**, and **user** resources.</span></span> <span data-ttu-id="03606-154">Это свойство по умолчанию поддерживает операторы `eq`, `ge` и `le`; при этом оно поддерживает операторы `in`, `ne` и `NOT` только в расширенных запросах.</span><span class="sxs-lookup"><span data-stu-id="03606-154">It supports the `eq`, `ge`, and `le` operators by default and the `in`, `ne`, and `NOT` operators only in advanced queries.</span></span>
+ <span data-ttu-id="03606-155">Оператор `endsWith` поддерживается только для свойств **mail** и **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="03606-155">The `endsWith` operator is supported only on **mail** and **userPrincipalName** properties.</span></span>
+ <span data-ttu-id="03606-156">Запросы, поддерживаемые по умолчанию, поддерживаются в расширенных запросах.</span><span class="sxs-lookup"><span data-stu-id="03606-156">Queries that are supported by default will also work in advanced queries.</span></span>
+ <span data-ttu-id="03606-157">Операторы отрицания `NOT` и `ne` поддерживаются только в расширенных запросах.</span><span class="sxs-lookup"><span data-stu-id="03606-157">The `NOT` and `ne` negation operators are supported only in advanced queries.</span></span> 
  + <span data-ttu-id="03606-158">Все свойства, поддерживающие оператор `eq`, также поддерживают операторы `ne` или `NOT`.</span><span class="sxs-lookup"><span data-stu-id="03606-158">All properties that support the `eq` operator also support the `ne` or `NOT` operators.</span></span>
  + <span data-ttu-id="03606-159">Оператор `ne` задействует отрицание в случаях, когда оператор `eq` выдал бы значение `true`.</span><span class="sxs-lookup"><span data-stu-id="03606-159">The `ne` operator negates where the `eq` operator would otherwise evaluate to `true`.</span></span> <span data-ttu-id="03606-160">Для запросов, использующих лямбда-оператор `any`, используйте оператор `NOT`.</span><span class="sxs-lookup"><span data-stu-id="03606-160">For queries that use the `any` lambda operator, use the `NOT` operator.</span></span> <span data-ttu-id="03606-161">См. [Фильтрация с помощью лямбда-операторов](/graph/query-parameters#filter-using-lambda-operators)..</span><span class="sxs-lookup"><span data-stu-id="03606-161">See [Filter using lambda operators](/graph/query-parameters#filter-using-lambda-operators).</span></span>

<span data-ttu-id="03606-162">В следующей таблице перечислена поддержка операторов `$filter` свойствами объекта каталога [users](/graph/api/resources/user).</span><span class="sxs-lookup"><span data-stu-id="03606-162">The following table summarizes support for `$filter` operators by properties on the [users](/graph/api/resources/user) directory object.</span></span>

- <span data-ttu-id="03606-163">![Работает по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="03606-163">![Works by default.</span></span> <span data-ttu-id="03606-164">Не требуются расширенные параметры запроса.](/graph/images/advanced-query-parameters/default.png)</span><span class="sxs-lookup"><span data-stu-id="03606-164">Does not require advanced query parameters.](/graph/images/advanced-query-parameters/default.png)</span></span> <span data-ttu-id="03606-165">Это свойство поддерживает `$filter` с оператором по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="03606-165">The property supports `$filter` with the operator by default.</span></span>
- <span data-ttu-id="03606-166">![Требуются расширенные параметры запроса.](/graph/images/advanced-query-parameters/advanced.png)</span><span class="sxs-lookup"><span data-stu-id="03606-166">![Requires advanced query parameters.](/graph/images/advanced-query-parameters/advanced.png)</span></span> <span data-ttu-id="03606-167">Для конкретного оператора `$filter` требуются *расширенные параметры запроса.*</span><span class="sxs-lookup"><span data-stu-id="03606-167">The specific `$filter` operator requires *advanced query parameters*:</span></span>
  - <span data-ttu-id="03606-168">Заголовок `ConsistencyLevel=eventual`</span><span class="sxs-lookup"><span data-stu-id="03606-168">`ConsistencyLevel=eventual` header</span></span>
  - <span data-ttu-id="03606-169">Строка запроса `$count=true`</span><span class="sxs-lookup"><span data-stu-id="03606-169">`$count=true` query string</span></span>
- <span data-ttu-id="03606-170">Пустые ячейки указывают, что это свойство не поддерживает использование `$filter` с оператором.</span><span class="sxs-lookup"><span data-stu-id="03606-170">Blank cells indicate that the property does not support the use of `$filter` with the operator.</span></span>
- <span data-ttu-id="03606-171">Столбец **Значения null** указывает, что для этого свойства поддерживается фильтрация по значениям `null`.</span><span class="sxs-lookup"><span data-stu-id="03606-171">The **null values** column indicates that the property is filterable on `null` values.</span></span>
- <span data-ttu-id="03606-172">Свойства, не указанные здесь, не поддерживают `$filter`.</span><span class="sxs-lookup"><span data-stu-id="03606-172">Properties that are not listed here do not support `$filter`.</span></span>

[!INCLUDE [filter-directory-objects](../includes/filter-directory-objects.md)]


## <a name="error-handling-for-advanced-queries-on-directory-objects"></a><span data-ttu-id="03606-173">Обработка ошибок расширенных запросов к объектам каталога</span><span class="sxs-lookup"><span data-stu-id="03606-173">Error handling for advanced queries on directory objects</span></span>

<span data-ttu-id="03606-174">Подсчет объектов каталога поддерживается только с использованием расширенных параметров запросов.</span><span class="sxs-lookup"><span data-stu-id="03606-174">Counting directory objects is only supported using the advanced queries parameters.</span></span> <span data-ttu-id="03606-175">Если заголовок `ConsistencyLevel=eventual` не указан, запрос возвращает ошибку, когда используется сегмент URL-адреса `$count`, или автоматически игнорирует параметр запроса `$count` (`?$count=true`), если он используется.</span><span class="sxs-lookup"><span data-stu-id="03606-175">If the `ConsistencyLevel=eventual` header is not specified, the request returns an error when the `$count` URL segment is used or silently ignores the `$count` query parameter (`?$count=true`) if it's used.</span></span>

```http
https://graph.microsoft.com/v1.0/users/$count
```

```json
{
    "error": {
        "code": "Request_BadRequest",
        "message": "$count is not currently supported.",
        "innerError": {
            "date": "2021-05-18T19:03:10",
            "request-id": "d9bbd4d8-bb2d-44e6-99a1-71a9516da744",
            "client-request-id": "539da3bd-942f-25db-636b-27f6f6e8eae4"
        }
    }
}
```

<span data-ttu-id="03606-176">`$search` для ресурсов Azure AD, производных от [directoryObject](/graph/api/resources/directoryobject), работает только в расширенных запросах.</span><span class="sxs-lookup"><span data-stu-id="03606-176">`$search` on Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject) works only in advanced queries.</span></span> <span data-ttu-id="03606-177">Если заголовок **ConsistencyLevel** не указан, запрос возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="03606-177">If the **ConsistencyLevel** header is not specified, the request returns an error.</span></span>

```http
https://graph.microsoft.com/v1.0/applications?$search="displayName:Browser"
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "Request with $search query parameter only works through MSGraph with a special request header: 'ConsistencyLevel: eventual'",
        "innerError": {
            "date": "2021-05-27T14:26:47",
            "request-id": "9b600954-ba11-4899-8ce9-6abad341f299",
            "client-request-id": "7964ef27-13a3-6ca4-ed7b-73c271110867"
        }
    }
}
```

<span data-ttu-id="03606-178">Если свойство или параметр запроса в URL-адресе поддерживаются только в расширенных запросах, но отсутствует заголовок **ConsistencyLevel** или строка запроса `$count=true`, то запрос возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="03606-178">If a property or query parameter in the URL is supported only in advanced queries but either the **ConsistencyLevel** header or the `$count=true` query string is missing, the request returns an error.</span></span>

```http
https://graph.microsoft.com/beta/users?$filter=endsWith(mail,'@outlook.com')
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "Unsupported Query.",
        "innerError": {
            "date": "2021-05-18T19:12:36",
            "request-id": "63f2093c-399c-4350-9609-3ce9b62abe3c",
            "client-request-id": "e60ed0ba-df5d-e190-f056-f9c0318456d7"
        }
    }
}
```

<span data-ttu-id="03606-179">Если свойство не проиндексировано для поддержки параметра запроса, даже если указаны расширенные параметры запроса, то запрос возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="03606-179">If a property has not been indexed to support a query parameter, even if the advanced query parameters are specified, the request returns an error.</span></span>

```http
https://graph.microsoft.com/v1.0/users?$filter=id ge '398164b1-5196-49dd-ada2-364b49f99b27'&$count=true
ConsistencyLevel: eventual
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "The request uses a filter property that is not indexed",
        "innerError": {
            "date": "2021-06-10T19:32:01",
            "request-id": "5625ba13-0c9f-4fce-a853-4b52f3e0bd09",
            "client-request-id": "76fe4cd8-df3a-f8c3-659b-594274b6bb31"
        }
    }
}
```

<span data-ttu-id="03606-180">При этом необходимо отметить, что указанные в запросе параметры могут просто не сработать.</span><span class="sxs-lookup"><span data-stu-id="03606-180">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="03606-181">Это может произойти, если не поддерживаются либо сами параметры, либо их сочетание.</span><span class="sxs-lookup"><span data-stu-id="03606-181">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="03606-182">В таких случаях необходимо проверить возвращенные запросом данные и определить, дали ли указанные параметры запроса желаемый результат.</span><span class="sxs-lookup"><span data-stu-id="03606-182">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> <span data-ttu-id="03606-183">В следующем примере параметр `@odata.count` отсутствует, даже если запрос успешно выполняется.</span><span class="sxs-lookup"><span data-stu-id="03606-183">For example, in the following example, the `@odata.count` parameter is missing even if the query is successful.</span></span>

```http
https://graph.microsoft.com/v1.0/users?$count=true
```

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "displayName":"Oscar Ward",
      "mail":"oscarward@contoso.com",
      "userPrincipalName":"oscarward@contoso.com"
    },
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="03606-184">См. также</span><span class="sxs-lookup"><span data-stu-id="03606-184">See also</span></span>

- [<span data-ttu-id="03606-185">Настройка откликов с помощью параметров запроса</span><span class="sxs-lookup"><span data-stu-id="03606-185">Use query parameters to customize responses</span></span>](/graph/query-parameters)
- [<span data-ttu-id="03606-186">Ограничения параметров запроса</span><span class="sxs-lookup"><span data-stu-id="03606-186">Query parameter limitations</span></span>](known-issues.md#query-parameter-limitations)
- [<span data-ttu-id="03606-187">Использование параметра запроса $search для сопоставления с условием поиска</span><span class="sxs-lookup"><span data-stu-id="03606-187">Use the $search query parameter to match a search criterion</span></span>](/graph/aad-advanced-queries)
