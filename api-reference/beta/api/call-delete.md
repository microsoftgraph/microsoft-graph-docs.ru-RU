---
title: Удаление звонка
description: Удаление или разрыв активного вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6eb30d8e92fe99e06467c01104d8742d090a8a18
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328113"
---
# <a name="delete-call"></a><span data-ttu-id="42484-103">Удаление звонка</span><span class="sxs-lookup"><span data-stu-id="42484-103">Delete call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42484-104">Удаление или разрыв активного вызова.</span><span class="sxs-lookup"><span data-stu-id="42484-104">Delete or hang up an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="42484-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42484-105">Permissions</span></span>

<span data-ttu-id="42484-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42484-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42484-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42484-108">Permission type</span></span> | <span data-ttu-id="42484-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42484-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="42484-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42484-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="42484-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42484-111">Not Supported.</span></span>                         |
| <span data-ttu-id="42484-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42484-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42484-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42484-113">Not Supported.</span></span>                         |
| <span data-ttu-id="42484-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="42484-114">Application</span></span>                            | <span data-ttu-id="42484-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="42484-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="42484-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42484-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /applications/{id}/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="42484-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42484-117">Request headers</span></span>
| <span data-ttu-id="42484-118">Имя</span><span class="sxs-lookup"><span data-stu-id="42484-118">Name</span></span>          | <span data-ttu-id="42484-119">Описание</span><span class="sxs-lookup"><span data-stu-id="42484-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="42484-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42484-120">Authorization</span></span> | <span data-ttu-id="42484-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42484-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42484-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42484-123">Request body</span></span>
<span data-ttu-id="42484-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42484-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42484-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="42484-125">Response</span></span>
<span data-ttu-id="42484-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="42484-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42484-128">Пример</span><span class="sxs-lookup"><span data-stu-id="42484-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="42484-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="42484-129">Request</span></span>
<span data-ttu-id="42484-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42484-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="42484-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="42484-131">Response</span></span>

> <span data-ttu-id="42484-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42484-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="42484-134">Уведомление — завершение</span><span class="sxs-lookup"><span data-stu-id="42484-134">Notification - terminating</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="42484-135">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="42484-135">Notification - terminated</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
