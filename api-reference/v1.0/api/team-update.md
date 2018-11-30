---
title: Группа обновления
description: Обновление свойств указанной группы.
ms.openlocfilehash: 27cbf8f571752a27fb68727fe2695a0250f5dc75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024727"
---
# <a name="update-team"></a><span data-ttu-id="81aed-103">Группа обновления</span><span class="sxs-lookup"><span data-stu-id="81aed-103">Update team</span></span>



<span data-ttu-id="81aed-104">Обновление свойств указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="81aed-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="81aed-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81aed-105">Permissions</span></span>
<span data-ttu-id="81aed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81aed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="81aed-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81aed-108">Permission type</span></span>      | <span data-ttu-id="81aed-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81aed-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81aed-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81aed-110">Delegated (work or school account)</span></span> | <span data-ttu-id="81aed-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81aed-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="81aed-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81aed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81aed-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81aed-113">Not supported.</span></span>    |
|<span data-ttu-id="81aed-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81aed-114">Application</span></span> | <span data-ttu-id="81aed-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81aed-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="81aed-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81aed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="81aed-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81aed-117">Request headers</span></span>
| <span data-ttu-id="81aed-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81aed-118">Header</span></span>       | <span data-ttu-id="81aed-119">Значение</span><span class="sxs-lookup"><span data-stu-id="81aed-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="81aed-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81aed-120">Authorization</span></span>  | <span data-ttu-id="81aed-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81aed-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="81aed-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81aed-123">Content-Type</span></span>  | <span data-ttu-id="81aed-124">application/json</span><span class="sxs-lookup"><span data-stu-id="81aed-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="81aed-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81aed-125">Request body</span></span>
<span data-ttu-id="81aed-126">В тексте запроса укажите представление JSON объекта [группы](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="81aed-126">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="81aed-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="81aed-127">Response</span></span>

<span data-ttu-id="81aed-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="81aed-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="81aed-129">Пример</span><span class="sxs-lookup"><span data-stu-id="81aed-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="81aed-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="81aed-130">Request</span></span>
<span data-ttu-id="81aed-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81aed-131">The following is an example of the request.</span></span>
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
  }
}
```
#### <a name="response"></a><span data-ttu-id="81aed-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="81aed-132">Response</span></span>
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
  "tocPath": ""
}-->
