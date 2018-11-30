---
title: Группа обновления
description: Обновление свойств указанной группы.
ms.openlocfilehash: 9d07fd687facc96c1bc4a93c37cb492b321518e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076078"
---
# <a name="update-team"></a><span data-ttu-id="8763e-103">Группа обновления</span><span class="sxs-lookup"><span data-stu-id="8763e-103">Update team</span></span>

> <span data-ttu-id="8763e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8763e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8763e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8763e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8763e-106">Обновление свойств указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="8763e-106">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8763e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8763e-107">Permissions</span></span>
<span data-ttu-id="8763e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8763e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8763e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8763e-110">Permission type</span></span>      | <span data-ttu-id="8763e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8763e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8763e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8763e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8763e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8763e-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8763e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8763e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8763e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8763e-115">Not supported.</span></span>    |
|<span data-ttu-id="8763e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8763e-116">Application</span></span> | <span data-ttu-id="8763e-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8763e-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="8763e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8763e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8763e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8763e-119">Request headers</span></span>
| <span data-ttu-id="8763e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8763e-120">Header</span></span>       | <span data-ttu-id="8763e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8763e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8763e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8763e-122">Authorization</span></span>  | <span data-ttu-id="8763e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8763e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8763e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8763e-125">Content-Type</span></span>  | <span data-ttu-id="8763e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8763e-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8763e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8763e-127">Request body</span></span>
<span data-ttu-id="8763e-128">В тексте запроса укажите представление JSON объекта [группы](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="8763e-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8763e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8763e-129">Response</span></span>

<span data-ttu-id="8763e-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8763e-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8763e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8763e-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8763e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8763e-132">Request</span></span>
<span data-ttu-id="8763e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8763e-133">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="8763e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8763e-134">Response</span></span>
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
