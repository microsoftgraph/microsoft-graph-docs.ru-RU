---
title: Получение беседы
description: Получение свойств и связей объекта беседы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 08059625838d6a60489820b2369768c6a3fca071
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931722"
---
# <a name="get-conversation"></a><span data-ttu-id="fe4f4-103">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="fe4f4-103">Get conversation</span></span>

> <span data-ttu-id="fe4f4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fe4f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe4f4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe4f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe4f4-106">Получение свойств и связей объекта беседы.</span><span class="sxs-lookup"><span data-stu-id="fe4f4-106">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe4f4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe4f4-107">Permissions</span></span>
<span data-ttu-id="fe4f4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe4f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe4f4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe4f4-110">Permission type</span></span>      | <span data-ttu-id="fe4f4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe4f4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe4f4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe4f4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fe4f4-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe4f4-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="fe4f4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe4f4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe4f4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe4f4-115">Not supported.</span></span>    |
|<span data-ttu-id="fe4f4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe4f4-116">Application</span></span> | <span data-ttu-id="fe4f4-117">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe4f4-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe4f4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe4f4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="fe4f4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fe4f4-119">Optional query parameters</span></span>
<span data-ttu-id="fe4f4-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fe4f4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fe4f4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe4f4-121">Request headers</span></span>
| <span data-ttu-id="fe4f4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe4f4-122">Header</span></span>       | <span data-ttu-id="fe4f4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fe4f4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fe4f4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe4f4-124">Authorization</span></span>  | <span data-ttu-id="fe4f4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe4f4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe4f4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe4f4-127">Request body</span></span>
<span data-ttu-id="fe4f4-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe4f4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe4f4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe4f4-129">Response</span></span>

<span data-ttu-id="fe4f4-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversation](../resources/conversation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe4f4-130">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe4f4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fe4f4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe4f4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe4f4-132">Request</span></span>
<span data-ttu-id="fe4f4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe4f4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="fe4f4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe4f4-134">Response</span></span>
<span data-ttu-id="fe4f4-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fe4f4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
