---
title: Обновление объекта команды
description: Обновление свойств указанной команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1b4c34a469de41a8fa7695537ca8c69fe6e4fa42
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458434"
---
# <a name="update-team"></a><span data-ttu-id="360ff-103">Обновление объекта команды</span><span class="sxs-lookup"><span data-stu-id="360ff-103">Update team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="360ff-104">Обновление свойств указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="360ff-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="360ff-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="360ff-105">Permissions</span></span>
<span data-ttu-id="360ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="360ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="360ff-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="360ff-108">Permission type</span></span>      | <span data-ttu-id="360ff-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="360ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="360ff-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="360ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="360ff-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="360ff-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="360ff-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="360ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="360ff-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="360ff-113">Not supported.</span></span>    |
|<span data-ttu-id="360ff-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="360ff-114">Application</span></span> | <span data-ttu-id="360ff-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="360ff-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="360ff-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="360ff-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="360ff-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="360ff-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="360ff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="360ff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="360ff-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="360ff-119">Request headers</span></span>
| <span data-ttu-id="360ff-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="360ff-120">Header</span></span>       | <span data-ttu-id="360ff-121">Значение</span><span class="sxs-lookup"><span data-stu-id="360ff-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="360ff-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="360ff-122">Authorization</span></span>  | <span data-ttu-id="360ff-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="360ff-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="360ff-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="360ff-125">Content-Type</span></span>  | <span data-ttu-id="360ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="360ff-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="360ff-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="360ff-127">Request body</span></span>
<span data-ttu-id="360ff-128">В тексте запроса добавьте представление объекта [группы](../resources/team.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="360ff-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="360ff-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="360ff-129">Response</span></span>

<span data-ttu-id="360ff-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="360ff-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="360ff-131">Пример</span><span class="sxs-lookup"><span data-stu-id="360ff-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="360ff-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="360ff-132">Request</span></span>
<span data-ttu-id="360ff-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="360ff-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="360ff-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="360ff-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
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
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="360ff-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="360ff-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="360ff-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="360ff-136">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
