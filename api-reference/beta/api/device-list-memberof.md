---
title: Список групп устройств
description: Получите группы, в которые входит это устройство. Эта операция не является транзитивной.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d37036734e1e00d8130612528ee90305c3986476
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437200"
---
# <a name="list-device-groups"></a><span data-ttu-id="1329c-104">Список групп устройств</span><span class="sxs-lookup"><span data-stu-id="1329c-104">List device groups</span></span>

<span data-ttu-id="1329c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1329c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1329c-106">Получите группы, в которые входит это устройство.</span><span class="sxs-lookup"><span data-stu-id="1329c-106">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="1329c-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="1329c-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="1329c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1329c-108">Permissions</span></span>

<span data-ttu-id="1329c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1329c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1329c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1329c-111">Permission type</span></span>      | <span data-ttu-id="1329c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1329c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1329c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1329c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1329c-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1329c-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1329c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1329c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1329c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1329c-116">Not supported.</span></span>    |
|<span data-ttu-id="1329c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1329c-117">Application</span></span> | <span data-ttu-id="1329c-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1329c-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="1329c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1329c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1329c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1329c-120">Optional query parameters</span></span>

<span data-ttu-id="1329c-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="1329c-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="1329c-122">Кроме того, включено также приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="1329c-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="1329c-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="1329c-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="1329c-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="1329c-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="1329c-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="1329c-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1329c-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1329c-126">Request headers</span></span>
| <span data-ttu-id="1329c-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1329c-127">Header</span></span>       | <span data-ttu-id="1329c-128">Значение</span><span class="sxs-lookup"><span data-stu-id="1329c-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1329c-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1329c-129">Authorization</span></span>  | <span data-ttu-id="1329c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1329c-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1329c-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="1329c-132">ConsistencyLevel</span></span> | <span data-ttu-id="1329c-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="1329c-133">eventual.</span></span> <span data-ttu-id="1329c-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="1329c-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="1329c-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="1329c-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1329c-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1329c-136">Request body</span></span>
<span data-ttu-id="1329c-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1329c-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1329c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1329c-138">Response</span></span>

<span data-ttu-id="1329c-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1329c-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1329c-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="1329c-140">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-direct-member-of"></a><span data-ttu-id="1329c-141">Пример 1. Получить группы, которые устройство является непосредственным участником</span><span class="sxs-lookup"><span data-stu-id="1329c-141">Example 1: Get groups that the device is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="1329c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="1329c-142">Request</span></span>

<span data-ttu-id="1329c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1329c-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1329c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="1329c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="1329c-145">C#</span><span class="sxs-lookup"><span data-stu-id="1329c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1329c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1329c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1329c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1329c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1329c-148">Java</span><span class="sxs-lookup"><span data-stu-id="1329c-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1329c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="1329c-149">Response</span></span>

<span data-ttu-id="1329c-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1329c-150">The following is an example of the response.</span></span> 
> <span data-ttu-id="1329c-151">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="1329c-151">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1329c-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1329c-152">All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="1329c-153">Пример 2: Получение только количества участников</span><span class="sxs-lookup"><span data-stu-id="1329c-153">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="1329c-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="1329c-154">Request</span></span>

<span data-ttu-id="1329c-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1329c-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1329c-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="1329c-156">Response</span></span>

<span data-ttu-id="1329c-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1329c-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="1329c-158">394</span><span class="sxs-lookup"><span data-stu-id="1329c-158">394</span></span>

### <a name="example-3-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="1329c-159">Пример 3. Использование литых и $search OData для получения членства с именами отображения, которые содержат буквы "Видео", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="1329c-159">Example 3: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1329c-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="1329c-160">Request</span></span>

<span data-ttu-id="1329c-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1329c-161">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1329c-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="1329c-162">Response</span></span>

<span data-ttu-id="1329c-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1329c-163">The following is an example of the response.</span></span>
><span data-ttu-id="1329c-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1329c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
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

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="1329c-166">Пример 4. Использование литых и $filter OData для получения членства с именем отображения, которое начинается с буквы "A", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="1329c-166">Example 4: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1329c-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="1329c-167">Request</span></span>

<span data-ttu-id="1329c-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1329c-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1329c-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="1329c-169">Response</span></span>

<span data-ttu-id="1329c-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1329c-170">The following is an example of the response.</span></span>
><span data-ttu-id="1329c-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1329c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
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
}
-->


