---
title: Удаление объекта eventMessage
description: Удаление объекта eventMessage.
author: angelgolfer-ms
ms.openlocfilehash: 68d9397f1fc595e864d94b87bdb67d766731411a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350220"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="1cb44-103">Удаление объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="1cb44-103">Delete eventMessage</span></span>

> <span data-ttu-id="1cb44-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1cb44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cb44-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cb44-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1cb44-106">Удаление объекта eventMessage.</span><span class="sxs-lookup"><span data-stu-id="1cb44-106">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="1cb44-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1cb44-107">Permissions</span></span>
<span data-ttu-id="1cb44-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cb44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cb44-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cb44-110">Permission type</span></span>      | <span data-ttu-id="1cb44-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cb44-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cb44-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cb44-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1cb44-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cb44-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1cb44-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cb44-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cb44-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cb44-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1cb44-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cb44-116">Application</span></span> | <span data-ttu-id="1cb44-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cb44-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cb44-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cb44-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1cb44-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cb44-119">Request headers</span></span>
| <span data-ttu-id="1cb44-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1cb44-120">Name</span></span>       | <span data-ttu-id="1cb44-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1cb44-121">Type</span></span> | <span data-ttu-id="1cb44-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1cb44-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1cb44-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cb44-123">Authorization</span></span>  | <span data-ttu-id="1cb44-124">string</span><span class="sxs-lookup"><span data-stu-id="1cb44-124">string</span></span>  | <span data-ttu-id="1cb44-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cb44-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cb44-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cb44-127">Request body</span></span>
<span data-ttu-id="1cb44-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1cb44-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cb44-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cb44-129">Response</span></span>

<span data-ttu-id="1cb44-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1cb44-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cb44-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1cb44-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1cb44-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cb44-133">Request</span></span>
<span data-ttu-id="1cb44-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cb44-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="1cb44-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cb44-135">Response</span></span>
<span data-ttu-id="1cb44-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1cb44-136">Here is an example of the response.</span></span> 
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
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->