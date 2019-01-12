---
title: Удаление страницы
description: Удаление страницы OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ec70039fe28f4a625043f678d40deff917577848
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979658"
---
# <a name="delete-page"></a><span data-ttu-id="4eae1-103">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="4eae1-103">Delete page</span></span>

> <span data-ttu-id="4eae1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4eae1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4eae1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eae1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4eae1-106">Удаление страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="4eae1-106">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="4eae1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4eae1-107">Permissions</span></span>
<span data-ttu-id="4eae1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eae1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eae1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4eae1-110">Permission type</span></span>      | <span data-ttu-id="4eae1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4eae1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4eae1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4eae1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4eae1-113">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eae1-113">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4eae1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4eae1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4eae1-115">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4eae1-115">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4eae1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4eae1-116">Application</span></span> | <span data-ttu-id="4eae1-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eae1-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4eae1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4eae1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4eae1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4eae1-119">Request headers</span></span>
| <span data-ttu-id="4eae1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4eae1-120">Name</span></span>       | <span data-ttu-id="4eae1-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4eae1-121">Type</span></span> | <span data-ttu-id="4eae1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4eae1-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4eae1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eae1-123">Authorization</span></span>  | <span data-ttu-id="4eae1-124">string</span><span class="sxs-lookup"><span data-stu-id="4eae1-124">string</span></span>  | <span data-ttu-id="4eae1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4eae1-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4eae1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eae1-127">Response</span></span>

<span data-ttu-id="4eae1-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4eae1-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eae1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4eae1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4eae1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4eae1-131">Request</span></span>
<span data-ttu-id="4eae1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4eae1-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="4eae1-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="4eae1-133">Response</span></span>
<span data-ttu-id="4eae1-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4eae1-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
