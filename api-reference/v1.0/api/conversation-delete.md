---
title: Удаление беседы
description: Удаление беседы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: b9c13c996b99874541a287d97a2669daf0a1825b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928369"
---
# <a name="delete-conversation"></a><span data-ttu-id="841c0-103">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="841c0-103">Delete conversation</span></span>

<span data-ttu-id="841c0-104">Удаление беседы.</span><span class="sxs-lookup"><span data-stu-id="841c0-104">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="841c0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="841c0-105">Permissions</span></span>
<span data-ttu-id="841c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="841c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="841c0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="841c0-108">Permission type</span></span>      | <span data-ttu-id="841c0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="841c0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="841c0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="841c0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="841c0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="841c0-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="841c0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="841c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="841c0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="841c0-113">Not supported.</span></span>    |
|<span data-ttu-id="841c0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="841c0-114">Application</span></span> | <span data-ttu-id="841c0-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="841c0-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="841c0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="841c0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="841c0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="841c0-117">Request headers</span></span>
| <span data-ttu-id="841c0-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="841c0-118">Header</span></span>       | <span data-ttu-id="841c0-119">Значение</span><span class="sxs-lookup"><span data-stu-id="841c0-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="841c0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="841c0-120">Authorization</span></span>  | <span data-ttu-id="841c0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="841c0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="841c0-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="841c0-123">Request body</span></span>
<span data-ttu-id="841c0-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="841c0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="841c0-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="841c0-125">Response</span></span>

<span data-ttu-id="841c0-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="841c0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="841c0-128">Пример</span><span class="sxs-lookup"><span data-stu-id="841c0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="841c0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="841c0-129">Request</span></span>
<span data-ttu-id="841c0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="841c0-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="841c0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="841c0-131">Response</span></span>
<span data-ttu-id="841c0-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="841c0-132">Here is an example of the response.</span></span> 
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
