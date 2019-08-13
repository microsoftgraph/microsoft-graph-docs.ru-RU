---
title: Перечисление каналов
description: Получение списка каналов в команде.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2723c18d964cd29a11da54ddd2356dc28824ab8d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317447"
---
# <a name="list-channels"></a><span data-ttu-id="17fcd-103">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="17fcd-103">List channels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17fcd-104">Получение списка [каналов](../resources/channel.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="17fcd-104">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="17fcd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17fcd-105">Permissions</span></span>
<span data-ttu-id="17fcd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17fcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="17fcd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17fcd-108">Permission type</span></span>      | <span data-ttu-id="17fcd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17fcd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17fcd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17fcd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17fcd-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17fcd-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="17fcd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17fcd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17fcd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17fcd-113">Not supported.</span></span>    |
|<span data-ttu-id="17fcd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17fcd-114">Application</span></span> | <span data-ttu-id="17fcd-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17fcd-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="17fcd-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="17fcd-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="17fcd-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="17fcd-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="17fcd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17fcd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17fcd-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="17fcd-119">Optional query parameters</span></span>
<span data-ttu-id="17fcd-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="17fcd-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17fcd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17fcd-121">Request headers</span></span>
| <span data-ttu-id="17fcd-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17fcd-122">Header</span></span>       | <span data-ttu-id="17fcd-123">Значение</span><span class="sxs-lookup"><span data-stu-id="17fcd-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="17fcd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17fcd-124">Authorization</span></span>  | <span data-ttu-id="17fcd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17fcd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="17fcd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17fcd-127">Request body</span></span>
<span data-ttu-id="17fcd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="17fcd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17fcd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="17fcd-129">Response</span></span>

<span data-ttu-id="17fcd-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17fcd-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17fcd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="17fcd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17fcd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="17fcd-132">Request</span></span>
<span data-ttu-id="17fcd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17fcd-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="17fcd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="17fcd-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="17fcd-135">C#</span><span class="sxs-lookup"><span data-stu-id="17fcd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17fcd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17fcd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="17fcd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17fcd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="17fcd-138">Java</span><span class="sxs-lookup"><span data-stu-id="17fcd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="17fcd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="17fcd-139">Response</span></span>
<span data-ttu-id="17fcd-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17fcd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
