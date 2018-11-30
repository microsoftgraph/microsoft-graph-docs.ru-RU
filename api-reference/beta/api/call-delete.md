---
title: Удалить вызов
description: Удалите или прервите активного вызова.
ms.openlocfilehash: ed0fb6928806511f92771237acb8ba08c8a162de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077600"
---
# <a name="delete-call"></a><span data-ttu-id="6a7fe-103">Удалить вызов</span><span class="sxs-lookup"><span data-stu-id="6a7fe-103">Delete call</span></span>

> <span data-ttu-id="6a7fe-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6a7fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a7fe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a7fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a7fe-106">Удалите или прервите активного вызова.</span><span class="sxs-lookup"><span data-stu-id="6a7fe-106">Delete or hang up an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a7fe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a7fe-107">Permissions</span></span>

<span data-ttu-id="6a7fe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a7fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a7fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a7fe-110">Permission type</span></span> | <span data-ttu-id="6a7fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a7fe-111">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="6a7fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a7fe-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a7fe-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a7fe-113">Not Supported.</span></span>                         |
| <span data-ttu-id="6a7fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a7fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a7fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a7fe-115">Not Supported.</span></span>                         |
| <span data-ttu-id="6a7fe-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6a7fe-116">Application</span></span>                            | <span data-ttu-id="6a7fe-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6a7fe-117">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="6a7fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a7fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /applications/{id}/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6a7fe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a7fe-119">Request headers</span></span>
| <span data-ttu-id="6a7fe-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6a7fe-120">Name</span></span>          | <span data-ttu-id="6a7fe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6a7fe-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6a7fe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a7fe-122">Authorization</span></span> | <span data-ttu-id="6a7fe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a7fe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a7fe-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a7fe-125">Request body</span></span>
<span data-ttu-id="6a7fe-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a7fe-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a7fe-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a7fe-127">Response</span></span>
<span data-ttu-id="6a7fe-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6a7fe-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a7fe-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6a7fe-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6a7fe-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a7fe-131">Request</span></span>
<span data-ttu-id="6a7fe-132">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a7fe-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="6a7fe-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a7fe-133">Response</span></span>

> <span data-ttu-id="6a7fe-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a7fe-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="6a7fe-136">Уведомления - завершение</span><span class="sxs-lookup"><span data-stu-id="6a7fe-136">Notification - terminating</span></span>

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
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminating"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="6a7fe-137">Уведомления - завершен</span><span class="sxs-lookup"><span data-stu-id="6a7fe-137">Notification - terminated</span></span>

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
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppInitiated"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
