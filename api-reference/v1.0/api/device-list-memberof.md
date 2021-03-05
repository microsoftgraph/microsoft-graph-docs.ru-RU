---
title: Список групп устройств
description: Получите группы, в которые входит это устройство. Эта операция не является транзитивной.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7c8bd0c9df919e69987443ca472b9485c1ffc0fe
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434596"
---
# <a name="list-device-groups"></a><span data-ttu-id="07d58-104">Список групп устройств</span><span class="sxs-lookup"><span data-stu-id="07d58-104">List device groups</span></span>

<span data-ttu-id="07d58-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07d58-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="07d58-106">Получите группы, в которые входит это устройство.</span><span class="sxs-lookup"><span data-stu-id="07d58-106">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="07d58-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="07d58-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="07d58-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07d58-108">Permissions</span></span>

<span data-ttu-id="07d58-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07d58-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07d58-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07d58-111">Permission type</span></span>      | <span data-ttu-id="07d58-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07d58-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07d58-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07d58-113">Delegated (work or school account)</span></span> | <span data-ttu-id="07d58-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07d58-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07d58-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07d58-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07d58-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07d58-116">Not supported.</span></span>    |
|<span data-ttu-id="07d58-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07d58-117">Application</span></span> | <span data-ttu-id="07d58-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d58-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="07d58-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07d58-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="07d58-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="07d58-120">Optional query parameters</span></span>

<span data-ttu-id="07d58-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="07d58-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="07d58-122">Кроме того, включено также приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="07d58-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="07d58-123">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="07d58-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="07d58-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="07d58-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="07d58-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="07d58-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07d58-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07d58-126">Request headers</span></span>

| <span data-ttu-id="07d58-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07d58-127">Header</span></span>       | <span data-ttu-id="07d58-128">Значение</span><span class="sxs-lookup"><span data-stu-id="07d58-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="07d58-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07d58-129">Authorization</span></span>  | <span data-ttu-id="07d58-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07d58-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="07d58-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="07d58-132">ConsistencyLevel</span></span> | <span data-ttu-id="07d58-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="07d58-133">eventual.</span></span> <span data-ttu-id="07d58-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="07d58-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="07d58-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="07d58-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07d58-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07d58-136">Request body</span></span>
<span data-ttu-id="07d58-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07d58-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07d58-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d58-138">Response</span></span>

<span data-ttu-id="07d58-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07d58-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07d58-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="07d58-140">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-direct-member-of"></a><span data-ttu-id="07d58-141">Пример 1. Получить группы, которые устройство является непосредственным участником</span><span class="sxs-lookup"><span data-stu-id="07d58-141">Example 1: Get groups that the device is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="07d58-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="07d58-142">Request</span></span>

<span data-ttu-id="07d58-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07d58-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07d58-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="07d58-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="07d58-145">C#</span><span class="sxs-lookup"><span data-stu-id="07d58-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07d58-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07d58-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07d58-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07d58-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="07d58-148">Java</span><span class="sxs-lookup"><span data-stu-id="07d58-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="07d58-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d58-149">Response</span></span>

<span data-ttu-id="07d58-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="07d58-150">The following is an example of the response.</span></span> 

> <span data-ttu-id="07d58-151">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="07d58-151">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="07d58-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07d58-152">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="07d58-153">Пример 2: Получение только количества участников</span><span class="sxs-lookup"><span data-stu-id="07d58-153">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="07d58-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="07d58-154">Request</span></span>

<span data-ttu-id="07d58-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07d58-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="07d58-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d58-156">Response</span></span>

<span data-ttu-id="07d58-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="07d58-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-3-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="07d58-158">Пример 3. Использование литых и $search OData для получения членства с именами отображения, которые содержат буквы "Видео", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="07d58-158">Example 3: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="07d58-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="07d58-159">Request</span></span>

<span data-ttu-id="07d58-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07d58-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="07d58-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d58-161">Response</span></span>

<span data-ttu-id="07d58-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="07d58-162">The following is an example of the response.</span></span>

><span data-ttu-id="07d58-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07d58-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.count":1396,
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="07d58-165">Пример 4. Использование литых и $filter OData для получения членства с именем отображения, которое начинается с буквы "A", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="07d58-165">Example 4: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="07d58-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="07d58-166">Request</span></span>

<span data-ttu-id="07d58-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07d58-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="07d58-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d58-168">Response</span></span>

<span data-ttu-id="07d58-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="07d58-169">The following is an example of the response.</span></span>

><span data-ttu-id="07d58-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07d58-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "displayName":"AAD Contoso Videos",
      "mail":"AADContosoVideos@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Videos",
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
