---
title: Получение беседы
description: Удаление объекта conversation.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ad4df01c2c0518d053145a427c9a79ad983d9972
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681755"
---
# <a name="get-conversation"></a><span data-ttu-id="4ba80-103">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="4ba80-103">Get conversation</span></span>

<span data-ttu-id="4ba80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ba80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ba80-105">Удаление объекта [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="4ba80-105">Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ba80-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ba80-106">Permissions</span></span>
<span data-ttu-id="4ba80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ba80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ba80-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ba80-109">Permission type</span></span>      | <span data-ttu-id="4ba80-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ba80-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ba80-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ba80-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ba80-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ba80-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ba80-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ba80-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ba80-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ba80-114">Not supported.</span></span>    |
|<span data-ttu-id="4ba80-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4ba80-115">Application</span></span> | <span data-ttu-id="4ba80-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ba80-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ba80-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ba80-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ba80-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ba80-118">Optional query parameters</span></span>
<span data-ttu-id="4ba80-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4ba80-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ba80-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ba80-120">Request headers</span></span>
| <span data-ttu-id="4ba80-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ba80-121">Header</span></span>       | <span data-ttu-id="4ba80-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4ba80-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4ba80-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ba80-123">Authorization</span></span>  | <span data-ttu-id="4ba80-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ba80-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ba80-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ba80-126">Request body</span></span>
<span data-ttu-id="4ba80-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ba80-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ba80-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ba80-128">Response</span></span>
<span data-ttu-id="4ba80-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [conversation](../resources/conversation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4ba80-129">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ba80-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4ba80-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4ba80-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ba80-131">Request</span></span>
<span data-ttu-id="4ba80-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ba80-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ba80-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ba80-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_conversation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="c"></a>[<span data-ttu-id="4ba80-134">C#</span><span class="sxs-lookup"><span data-stu-id="4ba80-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ba80-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ba80-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ba80-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ba80-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ba80-137">Java</span><span class="sxs-lookup"><span data-stu-id="4ba80-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4ba80-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ba80-138">Response</span></span>
<span data-ttu-id="4ba80-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4ba80-139">The following is an example of the response.</span></span>
><span data-ttu-id="4ba80-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4ba80-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


