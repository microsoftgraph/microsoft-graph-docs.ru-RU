---
title: Перечисление транзитивных групп устройств
description: Получите группы, в которые входит устройство.
localization_priority: Normal
author: spunukol
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 53f8bb896800742d25e14639f2a6b8a1a91d83c6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437158"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="5f796-103">Перечисление транзитивных групп устройств</span><span class="sxs-lookup"><span data-stu-id="5f796-103">List device transitive groups</span></span>

<span data-ttu-id="5f796-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f796-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f796-105">Получите группы, в которые входит устройство.</span><span class="sxs-lookup"><span data-stu-id="5f796-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="5f796-106">Этот запрос API является транзитным и также возвращает все группы, вложенные в устройство.</span><span class="sxs-lookup"><span data-stu-id="5f796-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f796-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f796-107">Permissions</span></span>

<span data-ttu-id="5f796-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f796-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f796-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f796-110">Permission type</span></span>      | <span data-ttu-id="5f796-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f796-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f796-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f796-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5f796-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5f796-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5f796-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f796-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f796-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f796-115">Not supported.</span></span>    |
|<span data-ttu-id="5f796-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f796-116">Application</span></span> | <span data-ttu-id="5f796-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f796-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]


## <a name="http-request"></a><span data-ttu-id="5f796-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f796-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f796-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5f796-119">Optional query parameters</span></span>

<span data-ttu-id="5f796-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="5f796-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="5f796-121">Кроме того, включено также приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="5f796-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="5f796-122">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="5f796-122">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="5f796-123">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="5f796-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="5f796-124">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="5f796-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f796-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f796-125">Request headers</span></span>

| <span data-ttu-id="5f796-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f796-126">Header</span></span>       | <span data-ttu-id="5f796-127">Значение</span><span class="sxs-lookup"><span data-stu-id="5f796-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5f796-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f796-128">Authorization</span></span>  | <span data-ttu-id="5f796-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f796-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5f796-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="5f796-131">ConsistencyLevel</span></span> | <span data-ttu-id="5f796-132">необязательный.</span><span class="sxs-lookup"><span data-stu-id="5f796-132">eventual.</span></span> <span data-ttu-id="5f796-133">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="5f796-133">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="5f796-134">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="5f796-134">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f796-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f796-135">Request body</span></span>

<span data-ttu-id="5f796-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f796-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f796-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f796-137">Response</span></span>

<span data-ttu-id="5f796-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f796-138">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f796-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="5f796-139">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-transitive-member-of"></a><span data-ttu-id="5f796-140">Пример 1. Получить группы, которые устройство является транзитным членом</span><span class="sxs-lookup"><span data-stu-id="5f796-140">Example 1: Get groups that the device is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="5f796-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f796-141">Request</span></span>

<span data-ttu-id="5f796-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f796-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5f796-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f796-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="5f796-144">C#</span><span class="sxs-lookup"><span data-stu-id="5f796-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f796-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f796-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f796-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f796-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f796-147">Java</span><span class="sxs-lookup"><span data-stu-id="5f796-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5f796-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f796-148">Response</span></span>

<span data-ttu-id="5f796-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f796-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="5f796-152">Пример 2: Получение только количества транзитивных участников</span><span class="sxs-lookup"><span data-stu-id="5f796-152">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="5f796-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f796-153">Request</span></span>

<span data-ttu-id="5f796-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f796-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5f796-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f796-155">Response</span></span>

<span data-ttu-id="5f796-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5f796-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="5f796-157">294</span><span class="sxs-lookup"><span data-stu-id="5f796-157">294</span></span>

### <a name="example-3-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="5f796-158">Пример 3. Использование литых и $search OData для получения членства с именами отображения, которые содержат буквы "Видео", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="5f796-158">Example 3: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="5f796-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f796-159">Request</span></span>

<span data-ttu-id="5f796-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f796-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5f796-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f796-161">Response</span></span>

<span data-ttu-id="5f796-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5f796-162">The following is an example of the response.</span></span>
><span data-ttu-id="5f796-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f796-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="5f796-165">Пример 4. Использование литых и $filter OData для получения членства с именем отображения, которое начинается с "A", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="5f796-165">Example 4: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="5f796-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f796-166">Request</span></span>

<span data-ttu-id="5f796-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f796-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5f796-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f796-168">Response</span></span>

<span data-ttu-id="5f796-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5f796-169">The following is an example of the response.</span></span>
><span data-ttu-id="5f796-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f796-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


