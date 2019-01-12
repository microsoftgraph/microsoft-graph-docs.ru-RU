---
title: Удаление беседы
description: Удаление беседы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: addcbcafb0b19447133a75427d98e3500990f365
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941018"
---
# <a name="delete-conversation"></a><span data-ttu-id="33a4f-103">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="33a4f-103">Delete conversation</span></span>

> <span data-ttu-id="33a4f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="33a4f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33a4f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33a4f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33a4f-106">Удаление беседы.</span><span class="sxs-lookup"><span data-stu-id="33a4f-106">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="33a4f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33a4f-107">Permissions</span></span>
<span data-ttu-id="33a4f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33a4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33a4f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33a4f-110">Permission type</span></span>      | <span data-ttu-id="33a4f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33a4f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33a4f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33a4f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="33a4f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33a4f-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="33a4f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33a4f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33a4f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33a4f-115">Not supported.</span></span>    |
|<span data-ttu-id="33a4f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33a4f-116">Application</span></span> | <span data-ttu-id="33a4f-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33a4f-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33a4f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33a4f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="33a4f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33a4f-119">Request headers</span></span>
| <span data-ttu-id="33a4f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33a4f-120">Header</span></span>       | <span data-ttu-id="33a4f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="33a4f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="33a4f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33a4f-122">Authorization</span></span>  | <span data-ttu-id="33a4f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33a4f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="33a4f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33a4f-125">Request body</span></span>
<span data-ttu-id="33a4f-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33a4f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33a4f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="33a4f-127">Response</span></span>

<span data-ttu-id="33a4f-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="33a4f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33a4f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="33a4f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33a4f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="33a4f-131">Request</span></span>
<span data-ttu-id="33a4f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33a4f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="33a4f-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="33a4f-133">Response</span></span>
<span data-ttu-id="33a4f-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="33a4f-134">Here is an example of the response.</span></span> 
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
