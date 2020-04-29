---
title: Обновление объекта команды
description: Обновление свойств указанной команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9a1c283ade37a396723a60980a5f5565f2e781a1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509480"
---
# <a name="update-team"></a><span data-ttu-id="6bf66-103">Обновление объекта команды</span><span class="sxs-lookup"><span data-stu-id="6bf66-103">Update team</span></span>

<span data-ttu-id="6bf66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bf66-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="6bf66-105">Обновление свойств указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="6bf66-105">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6bf66-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6bf66-106">Permissions</span></span>
<span data-ttu-id="6bf66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bf66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6bf66-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bf66-109">Permission type</span></span>      | <span data-ttu-id="6bf66-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bf66-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bf66-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bf66-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6bf66-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bf66-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6bf66-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bf66-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bf66-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bf66-114">Not supported.</span></span>    |
|<span data-ttu-id="6bf66-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6bf66-115">Application</span></span> | <span data-ttu-id="6bf66-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bf66-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="6bf66-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="6bf66-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6bf66-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="6bf66-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6bf66-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bf66-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6bf66-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bf66-120">Request headers</span></span>
| <span data-ttu-id="6bf66-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6bf66-121">Header</span></span>       | <span data-ttu-id="6bf66-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6bf66-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6bf66-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6bf66-123">Authorization</span></span>  | <span data-ttu-id="6bf66-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6bf66-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6bf66-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6bf66-126">Content-Type</span></span>  | <span data-ttu-id="6bf66-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6bf66-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6bf66-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6bf66-128">Request body</span></span>
<span data-ttu-id="6bf66-129">В тексте запроса добавьте представление объекта [группы](../resources/team.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bf66-129">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6bf66-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bf66-130">Response</span></span>

<span data-ttu-id="6bf66-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6bf66-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6bf66-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6bf66-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6bf66-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bf66-133">Request</span></span>
<span data-ttu-id="6bf66-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bf66-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6bf66-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bf66-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}
Content-type: application/json
Content-length: 211

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="6bf66-136">C#</span><span class="sxs-lookup"><span data-stu-id="6bf66-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6bf66-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bf66-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6bf66-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6bf66-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6bf66-139">Java</span><span class="sxs-lookup"><span data-stu-id="6bf66-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6bf66-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bf66-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
