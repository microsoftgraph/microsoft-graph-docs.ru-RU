---
title: Удаление страницы
description: Удаление страницы OneNote.
localization_priority: Normal
ms.openlocfilehash: 5721f06f34be48f0c8a3126d82e858aa833d3e77
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853552"
---
# <a name="delete-page"></a><span data-ttu-id="d6f8a-103">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="d6f8a-103">Delete page</span></span>

> <span data-ttu-id="d6f8a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d6f8a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6f8a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6f8a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6f8a-106">Удаление страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="d6f8a-106">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="d6f8a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6f8a-107">Permissions</span></span>
<span data-ttu-id="d6f8a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6f8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6f8a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6f8a-110">Permission type</span></span>      | <span data-ttu-id="d6f8a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6f8a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6f8a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6f8a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d6f8a-113">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6f8a-113">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d6f8a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6f8a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6f8a-115">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6f8a-115">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d6f8a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6f8a-116">Application</span></span> | <span data-ttu-id="d6f8a-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6f8a-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6f8a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6f8a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d6f8a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6f8a-119">Request headers</span></span>
| <span data-ttu-id="d6f8a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d6f8a-120">Name</span></span>       | <span data-ttu-id="d6f8a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d6f8a-121">Type</span></span> | <span data-ttu-id="d6f8a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d6f8a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d6f8a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6f8a-123">Authorization</span></span>  | <span data-ttu-id="d6f8a-124">string</span><span class="sxs-lookup"><span data-stu-id="d6f8a-124">string</span></span>  | <span data-ttu-id="d6f8a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6f8a-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d6f8a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6f8a-127">Response</span></span>

<span data-ttu-id="d6f8a-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d6f8a-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6f8a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d6f8a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6f8a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6f8a-131">Request</span></span>
<span data-ttu-id="d6f8a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6f8a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="d6f8a-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6f8a-133">Response</span></span>
<span data-ttu-id="d6f8a-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d6f8a-134">Here is an example of the response.</span></span>
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
