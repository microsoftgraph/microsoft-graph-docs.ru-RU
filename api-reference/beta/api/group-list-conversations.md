---
title: Список бесед
description: Получение списка бесед в этой группе.
ms.openlocfilehash: 97351b6b6afb8ed671704e77801d380e59694157
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082081"
---
# <a name="list-conversations"></a><span data-ttu-id="574e2-103">Список бесед</span><span class="sxs-lookup"><span data-stu-id="574e2-103">List conversations</span></span>

> <span data-ttu-id="574e2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="574e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="574e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="574e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="574e2-106">Получение списка объектов [conversation](../resources/conversation.md) в этой группе.</span><span class="sxs-lookup"><span data-stu-id="574e2-106">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="574e2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="574e2-107">Permissions</span></span>
<span data-ttu-id="574e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="574e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="574e2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="574e2-110">Permission type</span></span>      | <span data-ttu-id="574e2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="574e2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="574e2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="574e2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="574e2-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="574e2-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="574e2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="574e2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="574e2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="574e2-115">Not supported.</span></span>    |
|<span data-ttu-id="574e2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="574e2-116">Application</span></span> | <span data-ttu-id="574e2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="574e2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="574e2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="574e2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="574e2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="574e2-119">Optional query parameters</span></span>
<span data-ttu-id="574e2-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="574e2-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="574e2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="574e2-121">Request headers</span></span>
| <span data-ttu-id="574e2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="574e2-122">Header</span></span>       | <span data-ttu-id="574e2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="574e2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="574e2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="574e2-124">Authorization</span></span>  | <span data-ttu-id="574e2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="574e2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="574e2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="574e2-127">Request body</span></span>
<span data-ttu-id="574e2-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="574e2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="574e2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="574e2-129">Response</span></span>
<span data-ttu-id="574e2-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversation](../resources/conversation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="574e2-130">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="574e2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="574e2-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="574e2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="574e2-132">Request</span></span>
<span data-ttu-id="574e2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="574e2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```

#### <a name="response"></a><span data-ttu-id="574e2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="574e2-134">Response</span></span>
<span data-ttu-id="574e2-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="574e2-135">The following is an example of the response.</span></span>
><span data-ttu-id="574e2-136">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="574e2-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="574e2-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="574e2-137">All the properties will be returned from an actual call.</span></span>
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
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
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