---
title: Удаление беседы
description: Удаление беседы.
ms.openlocfilehash: 9a6e590470343afd7990d6f24672fe1824c65a90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077601"
---
# <a name="delete-conversation"></a><span data-ttu-id="cca34-103">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="cca34-103">Delete conversation</span></span>

> <span data-ttu-id="cca34-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cca34-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cca34-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cca34-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cca34-106">Удаление беседы.</span><span class="sxs-lookup"><span data-stu-id="cca34-106">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="cca34-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cca34-107">Permissions</span></span>
<span data-ttu-id="cca34-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cca34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cca34-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cca34-110">Permission type</span></span>      | <span data-ttu-id="cca34-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cca34-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cca34-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cca34-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cca34-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cca34-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cca34-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cca34-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cca34-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cca34-115">Not supported.</span></span>    |
|<span data-ttu-id="cca34-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cca34-116">Application</span></span> | <span data-ttu-id="cca34-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cca34-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cca34-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cca34-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cca34-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cca34-119">Request headers</span></span>
| <span data-ttu-id="cca34-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cca34-120">Header</span></span>       | <span data-ttu-id="cca34-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cca34-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cca34-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cca34-122">Authorization</span></span>  | <span data-ttu-id="cca34-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cca34-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cca34-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cca34-125">Request body</span></span>
<span data-ttu-id="cca34-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cca34-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cca34-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="cca34-127">Response</span></span>

<span data-ttu-id="cca34-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cca34-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cca34-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cca34-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cca34-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cca34-131">Request</span></span>
<span data-ttu-id="cca34-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cca34-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="cca34-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="cca34-133">Response</span></span>
<span data-ttu-id="cca34-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cca34-134">Here is an example of the response.</span></span> 
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
