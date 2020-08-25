---
title: Перечисление транзитивных групп устройств
description: Получение групп, участником которых является устройство.
localization_priority: Normal
author: spunukol
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3249b5634f16295b043e7479e5e0e60fb6186f34
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872714"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="22ec4-103">Перечисление транзитивных групп устройств</span><span class="sxs-lookup"><span data-stu-id="22ec4-103">List device transitive groups</span></span>

<span data-ttu-id="22ec4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22ec4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22ec4-105">Получение групп, участником которых является устройство.</span><span class="sxs-lookup"><span data-stu-id="22ec4-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="22ec4-106">Этот запрос API является транзитивным, а также возвращает все группы, в которых устройство является вложенным членом.</span><span class="sxs-lookup"><span data-stu-id="22ec4-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="22ec4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22ec4-107">Permissions</span></span>

<span data-ttu-id="22ec4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22ec4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22ec4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22ec4-110">Permission type</span></span>      | <span data-ttu-id="22ec4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22ec4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22ec4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22ec4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="22ec4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="22ec4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="22ec4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22ec4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22ec4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22ec4-115">Not supported.</span></span>    |
|<span data-ttu-id="22ec4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22ec4-116">Application</span></span> | <span data-ttu-id="22ec4-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22ec4-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]


## <a name="http-request"></a><span data-ttu-id="22ec4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22ec4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22ec4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="22ec4-119">Optional query parameters</span></span>

<span data-ttu-id="22ec4-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="22ec4-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="22ec4-121">Приведение OData также включено, например, можно выполнить приведение, чтобы получить только перечисление directoryrole, членом которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="22ec4-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="22ec4-122">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="22ec4-122">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="22ec4-123">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="22ec4-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="22ec4-124">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="22ec4-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22ec4-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22ec4-125">Request headers</span></span>

| <span data-ttu-id="22ec4-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22ec4-126">Header</span></span>       | <span data-ttu-id="22ec4-127">Значение</span><span class="sxs-lookup"><span data-stu-id="22ec4-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="22ec4-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22ec4-128">Authorization</span></span>  | <span data-ttu-id="22ec4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22ec4-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="22ec4-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="22ec4-131">ConsistencyLevel</span></span> | <span data-ttu-id="22ec4-132">необязательный.</span><span class="sxs-lookup"><span data-stu-id="22ec4-132">eventual.</span></span> <span data-ttu-id="22ec4-133">Этот заголовок и `$count` при использовании `$search` `$filter` `$orderby` параметров запроса на приведение,, или OData.</span><span class="sxs-lookup"><span data-stu-id="22ec4-133">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="22ec4-134">Он использует индекс, который может не быть актуальным с последними изменениями объекта.</span><span class="sxs-lookup"><span data-stu-id="22ec4-134">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22ec4-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22ec4-135">Request body</span></span>

<span data-ttu-id="22ec4-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22ec4-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22ec4-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="22ec4-137">Response</span></span>

<span data-ttu-id="22ec4-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22ec4-138">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22ec4-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="22ec4-139">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-transitive-member-of"></a><span data-ttu-id="22ec4-140">Пример 1: получение групп, в которых устройство является транзитивным участником</span><span class="sxs-lookup"><span data-stu-id="22ec4-140">Example 1: Get groups that the device is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="22ec4-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="22ec4-141">Request</span></span>

<span data-ttu-id="22ec4-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22ec4-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22ec4-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="22ec4-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="22ec4-144">C#</span><span class="sxs-lookup"><span data-stu-id="22ec4-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22ec4-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22ec4-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22ec4-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22ec4-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22ec4-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="22ec4-147">Response</span></span>

<span data-ttu-id="22ec4-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22ec4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="22ec4-151">Пример 2: получение только количества всех транзитивных членств</span><span class="sxs-lookup"><span data-stu-id="22ec4-151">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="22ec4-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="22ec4-152">Request</span></span>

<span data-ttu-id="22ec4-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22ec4-153">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="22ec4-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="22ec4-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="22ec4-155">C#</span><span class="sxs-lookup"><span data-stu-id="22ec4-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22ec4-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22ec4-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22ec4-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22ec4-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22ec4-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="22ec4-158">Response</span></span>

<span data-ttu-id="22ec4-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22ec4-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="22ec4-160">294</span><span class="sxs-lookup"><span data-stu-id="22ec4-160">294</span></span>

### <a name="example-3-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="22ec4-161">Пример 3: использование функции CAST и $search для получения членства с отображаемыми именами, содержащими видео "Video", включая число возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="22ec4-161">Example 3: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="22ec4-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="22ec4-162">Request</span></span>

<span data-ttu-id="22ec4-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22ec4-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="22ec4-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="22ec4-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="22ec4-165">C#</span><span class="sxs-lookup"><span data-stu-id="22ec4-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-video-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22ec4-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22ec4-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-video-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22ec4-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22ec4-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-video-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22ec4-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="22ec4-168">Response</span></span>

<span data-ttu-id="22ec4-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22ec4-169">The following is an example of the response.</span></span>
><span data-ttu-id="22ec4-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22ec4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso Videos",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="22ec4-172">Пример 4: использование функции CAST и $filter для получения членства с отображаемым именем, начинающимся с "A", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="22ec4-172">Example 4: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="22ec4-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="22ec4-173">Request</span></span>

<span data-ttu-id="22ec4-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22ec4-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="22ec4-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="22ec4-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="22ec4-176">C#</span><span class="sxs-lookup"><span data-stu-id="22ec4-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22ec4-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22ec4-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22ec4-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22ec4-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22ec4-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="22ec4-179">Response</span></span>

<span data-ttu-id="22ec4-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22ec4-180">The following is an example of the response.</span></span>
><span data-ttu-id="22ec4-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22ec4-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
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
}
-->
