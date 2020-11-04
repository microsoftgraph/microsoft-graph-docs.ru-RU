---
title: Перечисление транзитивных групп устройств
description: Получение групп, участником которых является устройство.
author: spunukol
ms.prod: microsoft-identity-platform
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: 3c33ae8796420ce1191ca4e79a71aa900063659a
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905290"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="c40e5-103">Перечисление транзитивных групп устройств</span><span class="sxs-lookup"><span data-stu-id="c40e5-103">List device transitive groups</span></span>

<span data-ttu-id="c40e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c40e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c40e5-105">Получение групп, участником которых является устройство.</span><span class="sxs-lookup"><span data-stu-id="c40e5-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="c40e5-106">Этот запрос API является транзитивным, а также возвращает все группы, в которых устройство является вложенным членом.</span><span class="sxs-lookup"><span data-stu-id="c40e5-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="c40e5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c40e5-107">Permissions</span></span>

<span data-ttu-id="c40e5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c40e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c40e5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c40e5-110">Permission type</span></span>      | <span data-ttu-id="c40e5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c40e5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c40e5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c40e5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c40e5-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c40e5-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c40e5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c40e5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c40e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c40e5-115">Not supported.</span></span>    |
|<span data-ttu-id="c40e5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c40e5-116">Application</span></span> | <span data-ttu-id="c40e5-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c40e5-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c40e5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c40e5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c40e5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c40e5-119">Optional query parameters</span></span>

<span data-ttu-id="c40e5-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="c40e5-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="c40e5-121">Кроме того, включено также приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="c40e5-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="c40e5-122">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="c40e5-122">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="c40e5-123">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="c40e5-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="c40e5-124">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="c40e5-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c40e5-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c40e5-125">Request headers</span></span>

| <span data-ttu-id="c40e5-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c40e5-126">Header</span></span>       | <span data-ttu-id="c40e5-127">Значение</span><span class="sxs-lookup"><span data-stu-id="c40e5-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c40e5-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c40e5-128">Authorization</span></span>  | <span data-ttu-id="c40e5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c40e5-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c40e5-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="c40e5-131">ConsistencyLevel</span></span> | <span data-ttu-id="c40e5-132">необязательный.</span><span class="sxs-lookup"><span data-stu-id="c40e5-132">eventual.</span></span> <span data-ttu-id="c40e5-133">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="c40e5-133">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="c40e5-134">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="c40e5-134">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c40e5-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c40e5-135">Request body</span></span>

<span data-ttu-id="c40e5-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c40e5-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c40e5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c40e5-137">Response</span></span>

<span data-ttu-id="c40e5-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c40e5-138">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c40e5-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="c40e5-139">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-transitive-member-of"></a><span data-ttu-id="c40e5-140">Пример 1: получение групп, в которых устройство является транзитивным участником</span><span class="sxs-lookup"><span data-stu-id="c40e5-140">Example 1: Get groups that the device is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="c40e5-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="c40e5-141">Request</span></span>

<span data-ttu-id="c40e5-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c40e5-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c40e5-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c40e5-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="c40e5-144">C#</span><span class="sxs-lookup"><span data-stu-id="c40e5-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c40e5-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c40e5-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c40e5-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c40e5-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c40e5-147">Java</span><span class="sxs-lookup"><span data-stu-id="c40e5-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c40e5-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c40e5-148">Response</span></span>

<span data-ttu-id="c40e5-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c40e5-149">The following is an example of the response.</span></span>

><span data-ttu-id="c40e5-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c40e5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```
### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="c40e5-152">Пример 2: Получение только количества транзитивных участников</span><span class="sxs-lookup"><span data-stu-id="c40e5-152">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="c40e5-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="c40e5-153">Request</span></span>

<span data-ttu-id="c40e5-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c40e5-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c40e5-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="c40e5-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c40e5-156">C#</span><span class="sxs-lookup"><span data-stu-id="c40e5-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c40e5-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c40e5-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c40e5-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c40e5-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c40e5-159">Java</span><span class="sxs-lookup"><span data-stu-id="c40e5-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c40e5-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c40e5-160">Response</span></span>

<span data-ttu-id="c40e5-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c40e5-161">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-odata-cast-and-search-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="c40e5-162">Пример 3: использование функции CAST и $search для получения сведений о членстве в группах с отображаемыми именами, содержащими "видео", в том числе от числа возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="c40e5-162">Example 3: Use OData cast and $search to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c40e5-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="c40e5-163">Request</span></span>

<span data-ttu-id="c40e5-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c40e5-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c40e5-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="c40e5-165">Response</span></span>

<span data-ttu-id="c40e5-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c40e5-166">The following is an example of the response.</span></span>

><span data-ttu-id="c40e5-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c40e5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso Videos",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="c40e5-169">Пример 4: использование функции CAST и $filter для получения членства с отображаемым именем, начинающимся с "A", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="c40e5-169">Example 4: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c40e5-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="c40e5-170">Request</span></span>

<span data-ttu-id="c40e5-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c40e5-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c40e5-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="c40e5-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c40e5-173">C#</span><span class="sxs-lookup"><span data-stu-id="c40e5-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c40e5-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c40e5-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c40e5-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c40e5-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c40e5-176">Java</span><span class="sxs-lookup"><span data-stu-id="c40e5-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c40e5-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="c40e5-177">Response</span></span>

<span data-ttu-id="c40e5-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c40e5-178">The following is an example of the response.</span></span>

><span data-ttu-id="c40e5-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c40e5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Users",
      "securityEnabled":true
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- 
{
  "type": "#page.annotation",
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
