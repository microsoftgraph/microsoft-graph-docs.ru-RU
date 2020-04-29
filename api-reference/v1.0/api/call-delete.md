---
title: Удаление звонка
description: Удаление или разрыв активного вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d509120cd29a2d2229e3dd157bb8162bb6ba38f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518730"
---
# <a name="delete-call"></a><span data-ttu-id="35164-103">Удаление звонка</span><span class="sxs-lookup"><span data-stu-id="35164-103">Delete call</span></span>

<span data-ttu-id="35164-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35164-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35164-105">Удаление или разрыв активного вызова.</span><span class="sxs-lookup"><span data-stu-id="35164-105">Delete or hang up an active call.</span></span> <span data-ttu-id="35164-106">Для звонков по группам это приведет к удалению только той стороны звонка, а базовый вызов групп будет продолжаться.</span><span class="sxs-lookup"><span data-stu-id="35164-106">For group calls, this will only delete your call leg and the underlying group call will still continue.</span></span>

## <a name="permissions"></a><span data-ttu-id="35164-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35164-107">Permissions</span></span>

| <span data-ttu-id="35164-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35164-108">Permission type</span></span> | <span data-ttu-id="35164-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35164-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="35164-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35164-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="35164-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35164-111">Not Supported.</span></span>                         |
| <span data-ttu-id="35164-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35164-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35164-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35164-113">Not Supported.</span></span>                         |
| <span data-ttu-id="35164-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35164-114">Application</span></span>                            | <span data-ttu-id="35164-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="35164-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="35164-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35164-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /communications/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="35164-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35164-117">Request headers</span></span>
| <span data-ttu-id="35164-118">Имя</span><span class="sxs-lookup"><span data-stu-id="35164-118">Name</span></span>          | <span data-ttu-id="35164-119">Описание</span><span class="sxs-lookup"><span data-stu-id="35164-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="35164-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35164-120">Authorization</span></span> | <span data-ttu-id="35164-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35164-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35164-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35164-123">Request body</span></span>
<span data-ttu-id="35164-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35164-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35164-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="35164-125">Response</span></span>
<span data-ttu-id="35164-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="35164-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35164-128">Пример</span><span class="sxs-lookup"><span data-stu-id="35164-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="35164-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="35164-129">Request</span></span>
<span data-ttu-id="35164-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35164-130">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="35164-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="35164-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="c"></a>[<span data-ttu-id="35164-132">C#</span><span class="sxs-lookup"><span data-stu-id="35164-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35164-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35164-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35164-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35164-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35164-135">Java</span><span class="sxs-lookup"><span data-stu-id="35164-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="35164-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="35164-136">Response</span></span>

> <span data-ttu-id="35164-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35164-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="35164-139">Уведомление — завершение</span><span class="sxs-lookup"><span data-stu-id="35164-139">Notification - terminating</span></span>

```http
POST https://bot.contoso.com/api/calls
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
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminating"
      }
    }
  ]
}
  
```

##### <a name="notification---terminated"></a><span data-ttu-id="35164-140">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="35164-140">Notification - terminated</span></span>

```http
POST https://bot.contoso.com/api/calls
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
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
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
