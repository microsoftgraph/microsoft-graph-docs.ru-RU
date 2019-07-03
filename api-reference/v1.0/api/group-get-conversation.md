---
title: Получение беседы
description: Удаление объекта conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f437172734a79b052e1863dcbeed928673f86103
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459526"
---
# <a name="get-conversation"></a><span data-ttu-id="77aa5-103">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="77aa5-103">Get conversation</span></span>
<span data-ttu-id="77aa5-104">Удаление объекта [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="77aa5-104">Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="77aa5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77aa5-105">Permissions</span></span>
<span data-ttu-id="77aa5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77aa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77aa5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77aa5-108">Permission type</span></span>      | <span data-ttu-id="77aa5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77aa5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77aa5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77aa5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77aa5-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77aa5-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="77aa5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77aa5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77aa5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77aa5-113">Not supported.</span></span>    |
|<span data-ttu-id="77aa5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77aa5-114">Application</span></span> | <span data-ttu-id="77aa5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77aa5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77aa5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77aa5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77aa5-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="77aa5-117">Optional query parameters</span></span>
<span data-ttu-id="77aa5-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="77aa5-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77aa5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77aa5-119">Request headers</span></span>
| <span data-ttu-id="77aa5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77aa5-120">Header</span></span>       | <span data-ttu-id="77aa5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="77aa5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="77aa5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77aa5-122">Authorization</span></span>  | <span data-ttu-id="77aa5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77aa5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="77aa5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="77aa5-125">Request body</span></span>
<span data-ttu-id="77aa5-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77aa5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77aa5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="77aa5-127">Response</span></span>
<span data-ttu-id="77aa5-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [conversation](../resources/conversation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="77aa5-128">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77aa5-129">Пример</span><span class="sxs-lookup"><span data-stu-id="77aa5-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="77aa5-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="77aa5-130">Request</span></span>
<span data-ttu-id="77aa5-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77aa5-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="77aa5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="77aa5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "get_group_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="77aa5-133">C#</span><span class="sxs-lookup"><span data-stu-id="77aa5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77aa5-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="77aa5-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77aa5-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="77aa5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="77aa5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="77aa5-136">Response</span></span>
<span data-ttu-id="77aa5-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="77aa5-137">The following is an example of the response.</span></span>
><span data-ttu-id="77aa5-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77aa5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 644

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
