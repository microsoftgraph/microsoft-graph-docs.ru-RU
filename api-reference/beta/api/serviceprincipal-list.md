---
title: Перечисление servicePrincipals
description: Получение списка объектов servicePrincipal.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: ec41e5c7d1b673bedda651dab9657515eff5d9db
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290042"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="1fed2-103">Перечисление servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="1fed2-103">List servicePrincipals</span></span>

<span data-ttu-id="1fed2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fed2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fed2-105">Получение списка объектов [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="1fed2-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fed2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1fed2-106">Permissions</span></span>

<span data-ttu-id="1fed2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fed2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1fed2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fed2-109">Permission type</span></span> | <span data-ttu-id="1fed2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fed2-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="1fed2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fed2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1fed2-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1fed2-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="1fed2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fed2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fed2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fed2-114">Not supported.</span></span> |
| <span data-ttu-id="1fed2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fed2-115">Application</span></span> | <span data-ttu-id="1fed2-116">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fed2-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fed2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fed2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1fed2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1fed2-118">Optional query parameters</span></span>

<span data-ttu-id="1fed2-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="1fed2-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="1fed2-120">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="1fed2-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="1fed2-121">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="1fed2-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="1fed2-122">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="1fed2-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fed2-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1fed2-123">Request headers</span></span>

| <span data-ttu-id="1fed2-124">Имя</span><span class="sxs-lookup"><span data-stu-id="1fed2-124">Name</span></span> | <span data-ttu-id="1fed2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1fed2-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="1fed2-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1fed2-126">Authorization</span></span> | <span data-ttu-id="1fed2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fed2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1fed2-129">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="1fed2-129">ConsistencyLevel</span></span> | <span data-ttu-id="1fed2-130">закончить.</span><span class="sxs-lookup"><span data-stu-id="1fed2-130">eventual.</span></span> <span data-ttu-id="1fed2-131">Этот заголовок и `$count` обязательные при использовании `$search` `$filter` с `$orderby` параметром Query.</span><span class="sxs-lookup"><span data-stu-id="1fed2-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="1fed2-132">Он использует индекс, который может быть не последним в актуальном изменении объекта.</span><span class="sxs-lookup"><span data-stu-id="1fed2-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fed2-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1fed2-133">Request body</span></span>

<span data-ttu-id="1fed2-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1fed2-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fed2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fed2-135">Response</span></span>

<span data-ttu-id="1fed2-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1fed2-136">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1fed2-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="1fed2-137">Examples</span></span>

### <a name="example-1-get-a-list-of-service-principals"></a><span data-ttu-id="1fed2-138">Пример 1: получение списка субъектов службы</span><span class="sxs-lookup"><span data-stu-id="1fed2-138">Example 1: Get a list of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="1fed2-139">Запросить</span><span class="sxs-lookup"><span data-stu-id="1fed2-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```http
GET https://graph.microsoft.com/beta/serviceprincipals
```

#### <a name="response"></a><span data-ttu-id="1fed2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fed2-140">Response</span></span>

<span data-ttu-id="1fed2-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1fed2-141">The following is an example of the response.</span></span>
><span data-ttu-id="1fed2-142">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1fed2-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1fed2-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fed2-143">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":true,
      "displayName":"amasf",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-service-principals"></a><span data-ttu-id="1fed2-144">Пример 2: получение только количества субъектов службы</span><span class="sxs-lookup"><span data-stu-id="1fed2-144">Example 2: Get only a count of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="1fed2-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fed2-145">Request</span></span>

<span data-ttu-id="1fed2-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fed2-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1fed2-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fed2-147">Response</span></span>

<span data-ttu-id="1fed2-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1fed2-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="1fed2-149">893</span><span class="sxs-lookup"><span data-stu-id="1fed2-149">893</span></span>


### <a name="example-3-use-filter-and-top-to-get-one-service-principal-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="1fed2-150">Пример 3: используйте $filter и $top, чтобы получить одного участника службы с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="1fed2-150">Example 3: Use $filter and $top to get one service principal with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1fed2-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fed2-151">Request</span></span>

<span data-ttu-id="1fed2-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fed2-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1fed2-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fed2-153">Response</span></span>

<span data-ttu-id="1fed2-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1fed2-154">The following is an example of the response.</span></span>
><span data-ttu-id="1fed2-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fed2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrinciples",
  "@odata.count":1,
  "value":[
    {
      "accountEnabled":true,
      "displayName":"a",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-service-principals-with-display-names-that-contain-the-letters-team-including-a-count-of-returned-objects"></a><span data-ttu-id="1fed2-157">Пример 4: используйте $search, чтобы получить субъекты служб с отображаемыми именами, которые содержат буквы "Team", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="1fed2-157">Example 4: Use $search to get service principals with display names that contain the letters 'Team' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1fed2-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fed2-158">Request</span></span>

<span data-ttu-id="1fed2-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fed2-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_team_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$search="displayName:Team"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1fed2-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fed2-160">Response</span></span>

<span data-ttu-id="1fed2-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1fed2-161">The following is an example of the response.</span></span>
><span data-ttu-id="1fed2-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fed2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrincipals",
  "@odata.count":1396,
  "value":[
    {
      "accountEnabled":true,
      "displayName":"myContosoTeam",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
