---
title: Удаление звонка
description: Удаление или разрыв активного вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aa1d0111085fa48f6c6186e764d19210a9f10ae2
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792417"
---
# <a name="delete-call"></a><span data-ttu-id="7b5ab-103">Удаление звонка</span><span class="sxs-lookup"><span data-stu-id="7b5ab-103">Delete call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b5ab-104">Удаление или разрыв активного вызова.</span><span class="sxs-lookup"><span data-stu-id="7b5ab-104">Delete or hang up an active call.</span></span> <span data-ttu-id="7b5ab-105">При вызове с использованием многосторонних вызовов это приведет к удалению только этой стороны; Базовый вызов по-прежнему будет продолжаться.</span><span class="sxs-lookup"><span data-stu-id="7b5ab-105">For multiparty calls, this will only delete your call leg; the underlying multiparty call will still continue.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b5ab-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b5ab-106">Permissions</span></span>

<span data-ttu-id="7b5ab-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b5ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b5ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b5ab-109">Permission type</span></span> | <span data-ttu-id="7b5ab-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b5ab-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="7b5ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b5ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b5ab-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b5ab-112">Not Supported.</span></span>                         |
| <span data-ttu-id="7b5ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b5ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b5ab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b5ab-114">Not Supported.</span></span>                         |
| <span data-ttu-id="7b5ab-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7b5ab-115">Application</span></span>                            | <span data-ttu-id="7b5ab-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7b5ab-116">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="7b5ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b5ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7b5ab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b5ab-118">Request headers</span></span>
| <span data-ttu-id="7b5ab-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7b5ab-119">Name</span></span>          | <span data-ttu-id="7b5ab-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7b5ab-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7b5ab-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b5ab-121">Authorization</span></span> | <span data-ttu-id="7b5ab-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b5ab-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b5ab-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b5ab-124">Request body</span></span>
<span data-ttu-id="7b5ab-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b5ab-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b5ab-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b5ab-126">Response</span></span>
<span data-ttu-id="7b5ab-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7b5ab-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b5ab-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7b5ab-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7b5ab-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b5ab-130">Request</span></span>
<span data-ttu-id="7b5ab-131">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b5ab-131">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7b5ab-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b5ab-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7b5ab-133">C#</span><span class="sxs-lookup"><span data-stu-id="7b5ab-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7b5ab-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b5ab-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7b5ab-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7b5ab-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7b5ab-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b5ab-136">Response</span></span>

> <span data-ttu-id="7b5ab-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b5ab-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="7b5ab-139">Уведомление — завершение</span><span class="sxs-lookup"><span data-stu-id="7b5ab-139">Notification - terminating</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminating"
      }
    }
  ]
}
  
```

##### <a name="notification---terminated"></a><span data-ttu-id="7b5ab-140">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="7b5ab-140">Notification - terminated</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": "0"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
