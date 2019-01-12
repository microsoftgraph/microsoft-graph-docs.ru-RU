---
title: Список бесед
description: Получение списка бесед в этой группе.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3baae994c3cebdbb7cd1e8049c8c0d1aeefefc8a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967330"
---
# <a name="list-conversations"></a><span data-ttu-id="9da06-103">Список бесед</span><span class="sxs-lookup"><span data-stu-id="9da06-103">List conversations</span></span>
<span data-ttu-id="9da06-104">Получение списка объектов [conversation](../resources/conversation.md) в этой группе.</span><span class="sxs-lookup"><span data-stu-id="9da06-104">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="9da06-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9da06-105">Permissions</span></span>
<span data-ttu-id="9da06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9da06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9da06-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9da06-108">Permission type</span></span>      | <span data-ttu-id="9da06-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9da06-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9da06-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9da06-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9da06-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9da06-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9da06-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9da06-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9da06-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9da06-113">Not supported.</span></span>    |
|<span data-ttu-id="9da06-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9da06-114">Application</span></span> | <span data-ttu-id="9da06-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9da06-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9da06-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9da06-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9da06-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9da06-117">Optional query parameters</span></span>
<span data-ttu-id="9da06-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9da06-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9da06-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9da06-119">Request headers</span></span>
| <span data-ttu-id="9da06-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9da06-120">Header</span></span>       | <span data-ttu-id="9da06-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9da06-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9da06-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9da06-122">Authorization</span></span>  | <span data-ttu-id="9da06-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9da06-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9da06-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9da06-125">Request body</span></span>
<span data-ttu-id="9da06-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9da06-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9da06-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9da06-127">Response</span></span>
<span data-ttu-id="9da06-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversation](../resources/conversation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9da06-128">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9da06-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9da06-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9da06-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9da06-130">Request</span></span>
<span data-ttu-id="9da06-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9da06-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
#### <a name="response"></a><span data-ttu-id="9da06-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="9da06-132">Response</span></span>
<span data-ttu-id="9da06-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9da06-133">The following is an example of the response.</span></span>
><span data-ttu-id="9da06-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9da06-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "preview": "preview-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
