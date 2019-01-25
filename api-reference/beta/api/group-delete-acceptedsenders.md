---
title: Удаление объекта acceptedSender
description: 'Удаление пользователя или группы из списка acceptedSenders. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a3406c028990b7b5989036f4173cf86f257b4f03
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520692"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="f05c3-103">Удаление объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="f05c3-103">Remove acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f05c3-104">Удаление пользователя или группы из списка acceptedSenders.</span><span class="sxs-lookup"><span data-stu-id="f05c3-104">Remove a user or group from the acceptedSenders list.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f05c3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f05c3-105">Permissions</span></span>
<span data-ttu-id="f05c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f05c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f05c3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f05c3-108">Permission type</span></span>                        | <span data-ttu-id="f05c3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f05c3-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="f05c3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f05c3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f05c3-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f05c3-111">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="f05c3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f05c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f05c3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f05c3-113">Not supported.</span></span>|
| <span data-ttu-id="f05c3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f05c3-114">Application</span></span>                            | <span data-ttu-id="f05c3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f05c3-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f05c3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f05c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id=<id>
```

## <a name="request-headers"></a><span data-ttu-id="f05c3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f05c3-117">Request headers</span></span>
| <span data-ttu-id="f05c3-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f05c3-118">Header</span></span>         | <span data-ttu-id="f05c3-119">Значение</span><span class="sxs-lookup"><span data-stu-id="f05c3-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="f05c3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f05c3-120">Authorization</span></span>  | <span data-ttu-id="f05c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f05c3-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="f05c3-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f05c3-123">Request body</span></span>
<span data-ttu-id="f05c3-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f05c3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f05c3-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="f05c3-125">Response</span></span>
<span data-ttu-id="f05c3-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f05c3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f05c3-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f05c3-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f05c3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f05c3-129">Request</span></span>
<span data-ttu-id="f05c3-130">Ниже представлено несколько примеров запроса.</span><span class="sxs-lookup"><span data-stu-id="f05c3-130">The following are a couple of examples of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}

DELETE https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="f05c3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f05c3-131">Response</span></span>
<span data-ttu-id="f05c3-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f05c3-132">The following is an example of the response.</span></span> 

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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-acceptedsenders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
