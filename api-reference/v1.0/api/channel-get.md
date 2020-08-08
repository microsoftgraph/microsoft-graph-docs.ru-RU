---
title: Получение канала
description: Получение свойств и связей канала.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fbe5833d25f844b06f70fb4e2b242e6883724d20
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589293"
---
# <a name="get-channel"></a><span data-ttu-id="751a6-103">Получение канала</span><span class="sxs-lookup"><span data-stu-id="751a6-103">Get channel</span></span>

<span data-ttu-id="751a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="751a6-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="751a6-105">Получение свойств и связей [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="751a6-105">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="751a6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="751a6-106">Permissions</span></span>
<span data-ttu-id="751a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="751a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="751a6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="751a6-109">Permission type</span></span>      | <span data-ttu-id="751a6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="751a6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="751a6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="751a6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="751a6-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="751a6-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="751a6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="751a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="751a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="751a6-114">Not supported.</span></span>    |
|<span data-ttu-id="751a6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="751a6-115">Application</span></span> | <span data-ttu-id="751a6-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="751a6-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="751a6-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="751a6-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="751a6-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="751a6-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="751a6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="751a6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="751a6-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="751a6-120">Optional query parameters</span></span>

<span data-ttu-id="751a6-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="751a6-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="751a6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="751a6-122">Request headers</span></span>
| <span data-ttu-id="751a6-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="751a6-123">Header</span></span>       | <span data-ttu-id="751a6-124">Значение</span><span class="sxs-lookup"><span data-stu-id="751a6-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="751a6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="751a6-125">Authorization</span></span>  | <span data-ttu-id="751a6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="751a6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="751a6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="751a6-128">Request body</span></span>
<span data-ttu-id="751a6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="751a6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="751a6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="751a6-130">Response</span></span>

<span data-ttu-id="751a6-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="751a6-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="751a6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="751a6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="751a6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="751a6-133">Request</span></span>
<span data-ttu-id="751a6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="751a6-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="751a6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="751a6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
# <a name="c"></a>[<span data-ttu-id="751a6-136">C#</span><span class="sxs-lookup"><span data-stu-id="751a6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="751a6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="751a6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="751a6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="751a6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="751a6-139">Java</span><span class="sxs-lookup"><span data-stu-id="751a6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="751a6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="751a6-140">Response</span></span>
<span data-ttu-id="751a6-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="751a6-141">Here is an example of the response.</span></span> 

><span data-ttu-id="751a6-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="751a6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
