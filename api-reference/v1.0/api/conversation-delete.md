---
title: Удаление беседы
description: Удаление беседы.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: a8cd0f470a47c6b2f6c75bf2f057b60af8138867
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821667"
---
# <a name="delete-conversation"></a><span data-ttu-id="250c1-103">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="250c1-103">Delete conversation</span></span>

<span data-ttu-id="250c1-104">Удаление беседы.</span><span class="sxs-lookup"><span data-stu-id="250c1-104">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="250c1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="250c1-105">Permissions</span></span>
<span data-ttu-id="250c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="250c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="250c1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="250c1-108">Permission type</span></span>      | <span data-ttu-id="250c1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="250c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="250c1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="250c1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="250c1-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="250c1-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="250c1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="250c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="250c1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="250c1-113">Not supported.</span></span>    |
|<span data-ttu-id="250c1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="250c1-114">Application</span></span> | <span data-ttu-id="250c1-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="250c1-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="250c1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="250c1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="250c1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="250c1-117">Request headers</span></span>
| <span data-ttu-id="250c1-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="250c1-118">Header</span></span>       | <span data-ttu-id="250c1-119">Значение</span><span class="sxs-lookup"><span data-stu-id="250c1-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="250c1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="250c1-120">Authorization</span></span>  | <span data-ttu-id="250c1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="250c1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="250c1-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="250c1-123">Request body</span></span>
<span data-ttu-id="250c1-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="250c1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="250c1-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="250c1-125">Response</span></span>

<span data-ttu-id="250c1-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="250c1-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="250c1-128">Пример</span><span class="sxs-lookup"><span data-stu-id="250c1-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="250c1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="250c1-129">Request</span></span>
<span data-ttu-id="250c1-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="250c1-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="250c1-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="250c1-131">Response</span></span>
<span data-ttu-id="250c1-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="250c1-132">Here is an example of the response.</span></span> 
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
