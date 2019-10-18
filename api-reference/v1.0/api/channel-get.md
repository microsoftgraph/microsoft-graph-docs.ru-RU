---
title: Получение канала
description: Получение свойств и связей канала.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fa95725a6edc1fb3d8cee0502e453de355f38615
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726482"
---
# <a name="get-channel"></a><span data-ttu-id="b8478-103">Получение канала</span><span class="sxs-lookup"><span data-stu-id="b8478-103">Get channel</span></span>



<span data-ttu-id="b8478-104">Получение свойств и связей [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="b8478-104">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8478-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8478-105">Permissions</span></span>
<span data-ttu-id="b8478-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8478-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8478-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8478-108">Permission type</span></span>      | <span data-ttu-id="b8478-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8478-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8478-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8478-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b8478-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8478-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b8478-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8478-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8478-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8478-113">Not supported.</span></span>    |
|<span data-ttu-id="b8478-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8478-114">Application</span></span> | <span data-ttu-id="b8478-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8478-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="b8478-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="b8478-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b8478-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="b8478-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b8478-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8478-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8478-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b8478-119">Optional query parameters</span></span>

<span data-ttu-id="b8478-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b8478-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8478-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8478-121">Request headers</span></span>
| <span data-ttu-id="b8478-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8478-122">Header</span></span>       | <span data-ttu-id="b8478-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b8478-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8478-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8478-124">Authorization</span></span>  | <span data-ttu-id="b8478-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8478-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8478-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8478-127">Request body</span></span>
<span data-ttu-id="b8478-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8478-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8478-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8478-129">Response</span></span>

<span data-ttu-id="b8478-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b8478-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8478-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b8478-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8478-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8478-132">Request</span></span>
<span data-ttu-id="b8478-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8478-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b8478-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8478-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8478-135">C#</span><span class="sxs-lookup"><span data-stu-id="b8478-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8478-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8478-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8478-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8478-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b8478-138">Java</span><span class="sxs-lookup"><span data-stu-id="b8478-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b8478-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8478-139">Response</span></span>
<span data-ttu-id="b8478-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b8478-140">Here is an example of the response.</span></span> 

><span data-ttu-id="b8478-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8478-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
