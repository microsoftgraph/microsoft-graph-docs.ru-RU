---
title: Удаление страницы
description: Удаление страницы OneNote.
localization_priority: Normal
ms.openlocfilehash: fc2a4a9e809cb3a335c795a27cb5ffe35487a880
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810012"
---
# <a name="delete-page"></a><span data-ttu-id="90cbb-103">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="90cbb-103">Delete page</span></span>

<span data-ttu-id="90cbb-104">Удаление страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="90cbb-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="90cbb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90cbb-105">Permissions</span></span>
<span data-ttu-id="90cbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90cbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90cbb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90cbb-108">Permission type</span></span>      | <span data-ttu-id="90cbb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90cbb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90cbb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90cbb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90cbb-111">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90cbb-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="90cbb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90cbb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90cbb-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90cbb-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="90cbb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90cbb-114">Application</span></span> | <span data-ttu-id="90cbb-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90cbb-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90cbb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90cbb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="90cbb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90cbb-117">Request headers</span></span>
| <span data-ttu-id="90cbb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="90cbb-118">Name</span></span>       | <span data-ttu-id="90cbb-119">Тип</span><span class="sxs-lookup"><span data-stu-id="90cbb-119">Type</span></span> | <span data-ttu-id="90cbb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="90cbb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="90cbb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="90cbb-121">Authorization</span></span>  | <span data-ttu-id="90cbb-122">string</span><span class="sxs-lookup"><span data-stu-id="90cbb-122">string</span></span>  | <span data-ttu-id="90cbb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90cbb-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="90cbb-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="90cbb-125">Response</span></span>

<span data-ttu-id="90cbb-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="90cbb-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90cbb-128">Пример</span><span class="sxs-lookup"><span data-stu-id="90cbb-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90cbb-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="90cbb-129">Request</span></span>
<span data-ttu-id="90cbb-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90cbb-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="90cbb-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="90cbb-131">Response</span></span>
<span data-ttu-id="90cbb-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90cbb-132">Here is an example of the response.</span></span>
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
