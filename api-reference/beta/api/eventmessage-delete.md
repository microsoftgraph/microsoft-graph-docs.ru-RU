---
title: Удаление объекта eventMessage
description: Удаление объекта eventMessage.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 032e43b603edbcce880ec8b1309b417e72f3bf03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887789"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="be02c-103">Удаление объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="be02c-103">Delete eventMessage</span></span>

> <span data-ttu-id="be02c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="be02c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be02c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be02c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be02c-106">Удаление объекта eventMessage.</span><span class="sxs-lookup"><span data-stu-id="be02c-106">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="be02c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be02c-107">Permissions</span></span>
<span data-ttu-id="be02c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be02c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be02c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be02c-110">Permission type</span></span>      | <span data-ttu-id="be02c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be02c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be02c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be02c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="be02c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be02c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="be02c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be02c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be02c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be02c-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="be02c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be02c-116">Application</span></span> | <span data-ttu-id="be02c-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be02c-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="be02c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be02c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="be02c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be02c-119">Request headers</span></span>
| <span data-ttu-id="be02c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="be02c-120">Name</span></span>       | <span data-ttu-id="be02c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="be02c-121">Type</span></span> | <span data-ttu-id="be02c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="be02c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="be02c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="be02c-123">Authorization</span></span>  | <span data-ttu-id="be02c-124">string</span><span class="sxs-lookup"><span data-stu-id="be02c-124">string</span></span>  | <span data-ttu-id="be02c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be02c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be02c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be02c-127">Request body</span></span>
<span data-ttu-id="be02c-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be02c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be02c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="be02c-129">Response</span></span>

<span data-ttu-id="be02c-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="be02c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be02c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="be02c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be02c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="be02c-133">Request</span></span>
<span data-ttu-id="be02c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be02c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="be02c-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="be02c-135">Response</span></span>
<span data-ttu-id="be02c-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="be02c-136">Here is an example of the response.</span></span> 
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
