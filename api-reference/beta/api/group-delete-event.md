---
title: Удаление события
description: Удаление объекта event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c42fa9942e25150c9cba7e5e2557ae35353c2d76
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524067"
---
# <a name="delete-event"></a><span data-ttu-id="7941e-103">Удаление события</span><span class="sxs-lookup"><span data-stu-id="7941e-103">Delete event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7941e-104">Удаление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="7941e-104">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7941e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7941e-105">Permissions</span></span>
<span data-ttu-id="7941e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7941e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7941e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7941e-108">Permission type</span></span>      | <span data-ttu-id="7941e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7941e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7941e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7941e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7941e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7941e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7941e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7941e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7941e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7941e-113">Not supported.</span></span>    |
|<span data-ttu-id="7941e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7941e-114">Application</span></span> | <span data-ttu-id="7941e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7941e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7941e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7941e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7941e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7941e-117">Request headers</span></span>
| <span data-ttu-id="7941e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7941e-118">Name</span></span>       | <span data-ttu-id="7941e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7941e-119">Type</span></span> | <span data-ttu-id="7941e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7941e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7941e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7941e-121">Authorization</span></span>  | <span data-ttu-id="7941e-122">string</span><span class="sxs-lookup"><span data-stu-id="7941e-122">string</span></span>  | <span data-ttu-id="7941e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7941e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7941e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7941e-125">Request body</span></span>
<span data-ttu-id="7941e-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7941e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7941e-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="7941e-127">Response</span></span>
<span data-ttu-id="7941e-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7941e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7941e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7941e-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7941e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7941e-131">Request</span></span>
<span data-ttu-id="7941e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7941e-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="7941e-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="7941e-133">Response</span></span>
<span data-ttu-id="7941e-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7941e-134">The following is an example of the response.</span></span> 
><span data-ttu-id="7941e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7941e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-event.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
