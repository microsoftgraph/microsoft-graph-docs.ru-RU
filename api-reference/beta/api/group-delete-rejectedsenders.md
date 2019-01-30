---
title: Удаление объекта rejectedSender
description: Удаление пользователя или группы из списка rejectedSenders.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: e8b5a0a6a0c6a4f72805845f7c7c579043c05c0e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643946"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="8513a-103">Удаление объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="8513a-103">Remove rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8513a-104">Удаление пользователя или группы из списка rejectedSenders.</span><span class="sxs-lookup"><span data-stu-id="8513a-104">Remove a user or group from the rejectedSenders list.</span></span>

## <a name="permissions"></a><span data-ttu-id="8513a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8513a-105">Permissions</span></span>
<span data-ttu-id="8513a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8513a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8513a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8513a-108">Permission type</span></span>                        | <span data-ttu-id="8513a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8513a-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="8513a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8513a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8513a-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8513a-111">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="8513a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8513a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8513a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8513a-113">Not supported.</span></span> |
| <span data-ttu-id="8513a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8513a-114">Application</span></span>                            | <span data-ttu-id="8513a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8513a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8513a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8513a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=<id>
```

## <a name="request-headers"></a><span data-ttu-id="8513a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8513a-117">Request headers</span></span>

| <span data-ttu-id="8513a-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8513a-118">Header</span></span>         | <span data-ttu-id="8513a-119">Значение</span><span class="sxs-lookup"><span data-stu-id="8513a-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="8513a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8513a-120">Authorization</span></span>  | <span data-ttu-id="8513a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8513a-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="8513a-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8513a-123">Request body</span></span>
<span data-ttu-id="8513a-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8513a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8513a-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8513a-125">Response</span></span>
<span data-ttu-id="8513a-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8513a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8513a-128">Пример</span><span class="sxs-lookup"><span data-stu-id="8513a-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8513a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8513a-129">Request</span></span>
<span data-ttu-id="8513a-130">Ниже представлено несколько примеров запроса.</span><span class="sxs-lookup"><span data-stu-id="8513a-130">The following are a couple of examples of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "remove_rejectedSender_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}

DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="8513a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8513a-131">Response</span></span>
<span data-ttu-id="8513a-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8513a-132">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
