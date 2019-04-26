---
title: Удаление outlookTaskGroup
description: Удаление указанного outlookTaskGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 82e7b1d71bc57e9eb54232e108fed8ad230dfe9a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337826"
---
# <a name="delete-outlooktaskgroup"></a><span data-ttu-id="f76c8-103">Удаление outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="f76c8-103">Delete outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f76c8-104">Удаление указанного [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="f76c8-104">Delete the specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="f76c8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f76c8-105">Permissions</span></span>
<span data-ttu-id="f76c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f76c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f76c8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f76c8-108">Permission type</span></span>      | <span data-ttu-id="f76c8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f76c8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f76c8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f76c8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f76c8-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f76c8-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f76c8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f76c8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f76c8-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f76c8-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f76c8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f76c8-114">Application</span></span> | <span data-ttu-id="f76c8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f76c8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f76c8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f76c8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskGroups/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f76c8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f76c8-117">Request headers</span></span>
| <span data-ttu-id="f76c8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f76c8-118">Name</span></span>       | <span data-ttu-id="f76c8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f76c8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f76c8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f76c8-120">Authorization</span></span>  | <span data-ttu-id="f76c8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f76c8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f76c8-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f76c8-123">Request body</span></span>
<span data-ttu-id="f76c8-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f76c8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f76c8-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="f76c8-125">Response</span></span>

<span data-ttu-id="f76c8-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f76c8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f76c8-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f76c8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f76c8-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f76c8-129">Request</span></span>
<span data-ttu-id="f76c8-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f76c8-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=
```
##### <a name="response"></a><span data-ttu-id="f76c8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f76c8-131">Response</span></span>
<span data-ttu-id="f76c8-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f76c8-132">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
