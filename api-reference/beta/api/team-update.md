---
title: Группа обновления
description: Обновление свойств указанной группы.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 478da815a7bdf5dca15ddba358b5e12c46c1f045
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885292"
---
# <a name="update-team"></a><span data-ttu-id="1d802-103">Группа обновления</span><span class="sxs-lookup"><span data-stu-id="1d802-103">Update team</span></span>

> <span data-ttu-id="1d802-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1d802-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d802-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d802-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d802-106">Обновление свойств указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="1d802-106">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1d802-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d802-107">Permissions</span></span>
<span data-ttu-id="1d802-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d802-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1d802-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d802-110">Permission type</span></span>      | <span data-ttu-id="1d802-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d802-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d802-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d802-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1d802-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d802-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1d802-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d802-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d802-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d802-115">Not supported.</span></span>    |
|<span data-ttu-id="1d802-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d802-116">Application</span></span> | <span data-ttu-id="1d802-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d802-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="1d802-118">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="1d802-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1d802-119">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="1d802-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1d802-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d802-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1d802-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d802-121">Request headers</span></span>
| <span data-ttu-id="1d802-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d802-122">Header</span></span>       | <span data-ttu-id="1d802-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1d802-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1d802-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d802-124">Authorization</span></span>  | <span data-ttu-id="1d802-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d802-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1d802-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d802-127">Content-Type</span></span>  | <span data-ttu-id="1d802-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1d802-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d802-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d802-129">Request body</span></span>
<span data-ttu-id="1d802-130">В тексте запроса укажите представление JSON объекта [группы](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="1d802-130">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1d802-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d802-131">Response</span></span>

<span data-ttu-id="1d802-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1d802-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1d802-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1d802-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1d802-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d802-134">Request</span></span>
<span data-ttu-id="1d802-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d802-135">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="1d802-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d802-136">Response</span></span>
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
