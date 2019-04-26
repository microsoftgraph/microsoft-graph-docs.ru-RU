---
title: Обновление объекта команды
description: Обновление свойств указанной команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6dd8e38261cb2e64c3717ea3bee26ca96bd8958
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548994"
---
# <a name="update-team"></a><span data-ttu-id="3ff7c-103">Обновление объекта команды</span><span class="sxs-lookup"><span data-stu-id="3ff7c-103">Update team</span></span>



<span data-ttu-id="3ff7c-104">Обновление свойств указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="3ff7c-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3ff7c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ff7c-105">Permissions</span></span>
<span data-ttu-id="3ff7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ff7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3ff7c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ff7c-108">Permission type</span></span>      | <span data-ttu-id="3ff7c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ff7c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ff7c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ff7c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ff7c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ff7c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3ff7c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ff7c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ff7c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ff7c-113">Not supported.</span></span>    |
|<span data-ttu-id="3ff7c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ff7c-114">Application</span></span> | <span data-ttu-id="3ff7c-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ff7c-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="3ff7c-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="3ff7c-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3ff7c-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="3ff7c-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3ff7c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ff7c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3ff7c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ff7c-119">Request headers</span></span>
| <span data-ttu-id="3ff7c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ff7c-120">Header</span></span>       | <span data-ttu-id="3ff7c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3ff7c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3ff7c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ff7c-122">Authorization</span></span>  | <span data-ttu-id="3ff7c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ff7c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3ff7c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ff7c-125">Content-Type</span></span>  | <span data-ttu-id="3ff7c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ff7c-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3ff7c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ff7c-127">Request body</span></span>
<span data-ttu-id="3ff7c-128">В тексте запроса добавьте представление объекта [группы](../resources/team.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ff7c-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3ff7c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ff7c-129">Response</span></span>

<span data-ttu-id="3ff7c-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3ff7c-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3ff7c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3ff7c-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3ff7c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ff7c-132">Request</span></span>
<span data-ttu-id="3ff7c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ff7c-133">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="3ff7c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ff7c-134">Response</span></span>
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
