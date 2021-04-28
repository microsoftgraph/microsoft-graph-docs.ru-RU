---
title: Перечисление транзитивных групп устройств
description: Получите группы, в которые входит устройство.
author: spunukol
ms.prod: directory-management
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: cf86bfa5235ae00450e14e8c5d221bb41f60e4f2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053225"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="a428c-103">Перечисление транзитивных групп устройств</span><span class="sxs-lookup"><span data-stu-id="a428c-103">List device transitive groups</span></span>

<span data-ttu-id="a428c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a428c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a428c-105">Получите группы, в которые входит устройство.</span><span class="sxs-lookup"><span data-stu-id="a428c-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="a428c-106">Этот запрос API является транзитным и также возвращает все группы, вложенные в устройство.</span><span class="sxs-lookup"><span data-stu-id="a428c-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="a428c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a428c-107">Permissions</span></span>

<span data-ttu-id="a428c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a428c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a428c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a428c-110">Permission type</span></span>      | <span data-ttu-id="a428c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a428c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a428c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a428c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a428c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a428c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a428c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a428c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a428c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a428c-115">Not supported.</span></span>    |
|<span data-ttu-id="a428c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a428c-116">Application</span></span> | <span data-ttu-id="a428c-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a428c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a428c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a428c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a428c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a428c-119">Optional query parameters</span></span>

<span data-ttu-id="a428c-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="a428c-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="a428c-121">Кроме того, включено также приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="a428c-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="a428c-122">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="a428c-122">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="a428c-123">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="a428c-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="a428c-124">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="a428c-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a428c-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a428c-125">Request headers</span></span>

| <span data-ttu-id="a428c-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a428c-126">Header</span></span>       | <span data-ttu-id="a428c-127">Значение</span><span class="sxs-lookup"><span data-stu-id="a428c-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a428c-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a428c-128">Authorization</span></span>  | <span data-ttu-id="a428c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a428c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a428c-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="a428c-131">ConsistencyLevel</span></span> | <span data-ttu-id="a428c-132">необязательный.</span><span class="sxs-lookup"><span data-stu-id="a428c-132">eventual.</span></span> <span data-ttu-id="a428c-133">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="a428c-133">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="a428c-134">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="a428c-134">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a428c-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a428c-135">Request body</span></span>

<span data-ttu-id="a428c-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a428c-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a428c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a428c-137">Response</span></span>

<span data-ttu-id="a428c-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a428c-138">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a428c-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="a428c-139">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-transitive-member-of"></a><span data-ttu-id="a428c-140">Пример 1. Получить группы, которые устройство является транзитным членом</span><span class="sxs-lookup"><span data-stu-id="a428c-140">Example 1: Get groups that the device is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="a428c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a428c-141">Request</span></span>

<span data-ttu-id="a428c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a428c-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a428c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="a428c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="a428c-144">C#</span><span class="sxs-lookup"><span data-stu-id="a428c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a428c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a428c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a428c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a428c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a428c-147">Java</span><span class="sxs-lookup"><span data-stu-id="a428c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a428c-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a428c-148">Response</span></span>

<span data-ttu-id="a428c-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a428c-149">The following is an example of the response.</span></span>

><span data-ttu-id="a428c-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a428c-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="a428c-151">Пример 2: Получение только количества транзитивных участников</span><span class="sxs-lookup"><span data-stu-id="a428c-151">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="a428c-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="a428c-152">Request</span></span>

<span data-ttu-id="a428c-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a428c-153">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a428c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="a428c-154">Response</span></span>

<span data-ttu-id="a428c-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a428c-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-odata-cast-and-search-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="a428c-156">Пример 3. Использование литых и $search OData для получения членства в группе с именами отображения, содержами буквы "Видео", включая количество возвращенных объектов.</span><span class="sxs-lookup"><span data-stu-id="a428c-156">Example 3: Use OData cast and $search to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a428c-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="a428c-157">Request</span></span>

<span data-ttu-id="a428c-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a428c-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a428c-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="a428c-159">Response</span></span>

<span data-ttu-id="a428c-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a428c-160">The following is an example of the response.</span></span>

><span data-ttu-id="a428c-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a428c-161">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="a428c-162">Пример 4. Использование литых и $filter OData для получения членства с именем отображения, которое начинается с "A", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="a428c-162">Example 4: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a428c-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="a428c-163">Request</span></span>

<span data-ttu-id="a428c-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a428c-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a428c-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="a428c-165">Response</span></span>

<span data-ttu-id="a428c-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a428c-166">The following is an example of the response.</span></span>

><span data-ttu-id="a428c-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a428c-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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
