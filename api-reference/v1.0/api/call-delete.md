---
title: Удаление звонка
description: Удаление или разрыв активного вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 708ff1466b86be842e751c3a79cf17dbf1ad64bd
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913606"
---
# <a name="delete-call"></a><span data-ttu-id="68479-103">Удаление звонка</span><span class="sxs-lookup"><span data-stu-id="68479-103">Delete call</span></span>

<span data-ttu-id="68479-104">Удаление или разрыв активного вызова.</span><span class="sxs-lookup"><span data-stu-id="68479-104">Delete or hang up an active call.</span></span> <span data-ttu-id="68479-105">Для звонков по группам это приведет к удалению только той стороны звонка, а базовый вызов групп будет продолжаться.</span><span class="sxs-lookup"><span data-stu-id="68479-105">For group calls, this will only delete your call leg and the underlying group call will still continue.</span></span>

## <a name="permissions"></a><span data-ttu-id="68479-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68479-106">Permissions</span></span>

| <span data-ttu-id="68479-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68479-107">Permission type</span></span> | <span data-ttu-id="68479-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68479-108">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="68479-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68479-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="68479-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68479-110">Not Supported.</span></span>                         |
| <span data-ttu-id="68479-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68479-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68479-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68479-112">Not Supported.</span></span>                         |
| <span data-ttu-id="68479-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68479-113">Application</span></span>                            | <span data-ttu-id="68479-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="68479-114">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="68479-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68479-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /communications/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="68479-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68479-116">Request headers</span></span>
| <span data-ttu-id="68479-117">Имя</span><span class="sxs-lookup"><span data-stu-id="68479-117">Name</span></span>          | <span data-ttu-id="68479-118">Описание</span><span class="sxs-lookup"><span data-stu-id="68479-118">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="68479-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68479-119">Authorization</span></span> | <span data-ttu-id="68479-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68479-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68479-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68479-122">Request body</span></span>
<span data-ttu-id="68479-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68479-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68479-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="68479-124">Response</span></span>
<span data-ttu-id="68479-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="68479-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68479-127">Пример</span><span class="sxs-lookup"><span data-stu-id="68479-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="68479-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="68479-128">Request</span></span>
<span data-ttu-id="68479-129">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68479-129">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="68479-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="68479-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="68479-131">C#</span><span class="sxs-lookup"><span data-stu-id="68479-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68479-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68479-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="68479-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68479-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="68479-134">Java</span><span class="sxs-lookup"><span data-stu-id="68479-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="68479-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="68479-135">Response</span></span>

> <span data-ttu-id="68479-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68479-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="68479-138">Уведомление — завершение</span><span class="sxs-lookup"><span data-stu-id="68479-138">Notification - terminating</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="68479-139">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="68479-139">Notification - terminated</span></span>

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
