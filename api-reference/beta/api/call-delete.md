---
title: Удаление вызова
description: Удаление или подвешить активный вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: dbdaf4a0332c52e932031da29e0427c3b054763b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948597"
---
# <a name="delete-call"></a><span data-ttu-id="19064-103">Удаление вызова</span><span class="sxs-lookup"><span data-stu-id="19064-103">Delete call</span></span>

<span data-ttu-id="19064-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19064-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19064-105">Удаление или подвешить активный вызов.</span><span class="sxs-lookup"><span data-stu-id="19064-105">Delete or hang up an active call.</span></span> <span data-ttu-id="19064-106">Для групповых вызовов это удаляет только ногу вызова, а в основном групповой вызов будет по-прежнему продолжаться.</span><span class="sxs-lookup"><span data-stu-id="19064-106">For group calls, this will only delete your call leg and the underlying group call will still continue.</span></span>

## <a name="permissions"></a><span data-ttu-id="19064-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19064-107">Permissions</span></span>

| <span data-ttu-id="19064-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19064-108">Permission type</span></span> | <span data-ttu-id="19064-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19064-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="19064-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19064-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="19064-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19064-111">Not Supported.</span></span>                         |
| <span data-ttu-id="19064-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19064-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19064-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19064-113">Not Supported.</span></span>                         |
| <span data-ttu-id="19064-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="19064-114">Application</span></span>                            | <span data-ttu-id="19064-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="19064-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="19064-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19064-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /communications/calls/{id}
```
> <span data-ttu-id="19064-117">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="19064-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="19064-118">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="19064-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19064-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19064-119">Request headers</span></span>
| <span data-ttu-id="19064-120">Имя</span><span class="sxs-lookup"><span data-stu-id="19064-120">Name</span></span>          | <span data-ttu-id="19064-121">Описание</span><span class="sxs-lookup"><span data-stu-id="19064-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="19064-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19064-122">Authorization</span></span> | <span data-ttu-id="19064-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19064-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19064-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19064-125">Request body</span></span>
<span data-ttu-id="19064-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19064-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19064-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="19064-127">Response</span></span>
<span data-ttu-id="19064-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="19064-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19064-130">Пример</span><span class="sxs-lookup"><span data-stu-id="19064-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="19064-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="19064-131">Request</span></span>
<span data-ttu-id="19064-132">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19064-132">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="19064-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="19064-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call-1"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="c"></a>[<span data-ttu-id="19064-134">C#</span><span class="sxs-lookup"><span data-stu-id="19064-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19064-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19064-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19064-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19064-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19064-137">Java</span><span class="sxs-lookup"><span data-stu-id="19064-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="19064-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="19064-138">Response</span></span>

> <span data-ttu-id="19064-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19064-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="19064-141">Уведомление — прекращение</span><span class="sxs-lookup"><span data-stu-id="19064-141">Notification - terminating</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="19064-142">Уведомление — прекращено</span><span class="sxs-lookup"><span data-stu-id="19064-142">Notification - terminated</span></span>

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


