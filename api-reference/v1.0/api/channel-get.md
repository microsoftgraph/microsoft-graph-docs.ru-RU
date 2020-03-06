---
title: Получение канала
description: Получение свойств и связей канала.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b9aa260dfe054c05f80cc0c53c9a2b8a4a10779c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518618"
---
# <a name="get-channel"></a><span data-ttu-id="c7014-103">Получение канала</span><span class="sxs-lookup"><span data-stu-id="c7014-103">Get channel</span></span>

<span data-ttu-id="c7014-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7014-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="c7014-105">Получение свойств и связей [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="c7014-105">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7014-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7014-106">Permissions</span></span>
<span data-ttu-id="c7014-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7014-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7014-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7014-109">Permission type</span></span>      | <span data-ttu-id="c7014-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7014-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7014-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7014-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7014-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7014-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7014-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7014-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7014-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7014-114">Not supported.</span></span>    |
|<span data-ttu-id="c7014-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7014-115">Application</span></span> | <span data-ttu-id="c7014-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7014-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="c7014-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="c7014-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c7014-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="c7014-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c7014-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7014-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7014-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c7014-120">Optional query parameters</span></span>

<span data-ttu-id="c7014-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c7014-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7014-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7014-122">Request headers</span></span>
| <span data-ttu-id="c7014-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7014-123">Header</span></span>       | <span data-ttu-id="c7014-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c7014-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c7014-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7014-125">Authorization</span></span>  | <span data-ttu-id="c7014-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7014-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c7014-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7014-128">Request body</span></span>
<span data-ttu-id="c7014-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7014-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7014-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7014-130">Response</span></span>

<span data-ttu-id="c7014-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7014-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7014-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c7014-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7014-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7014-133">Request</span></span>
<span data-ttu-id="c7014-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7014-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7014-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7014-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
# <a name="c"></a>[<span data-ttu-id="c7014-136">C#</span><span class="sxs-lookup"><span data-stu-id="c7014-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7014-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7014-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7014-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7014-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7014-139">Java</span><span class="sxs-lookup"><span data-stu-id="c7014-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c7014-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7014-140">Response</span></span>
<span data-ttu-id="c7014-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c7014-141">Here is an example of the response.</span></span> 

><span data-ttu-id="c7014-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7014-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
