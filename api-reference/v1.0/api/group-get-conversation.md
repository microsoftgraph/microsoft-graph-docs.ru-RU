---
title: Получение беседы
description: Удаление объекта conversation.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: bd434a9c820559d2834776ef934c6fdb6c3056b3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681020"
---
# <a name="get-conversation"></a><span data-ttu-id="ce0e7-103">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="ce0e7-103">Get conversation</span></span>

<span data-ttu-id="ce0e7-104">Пространство имен: microsoft.graph Получить [объект беседы.](../resources/conversation.md)</span><span class="sxs-lookup"><span data-stu-id="ce0e7-104">Namespace: microsoft.graph Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce0e7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce0e7-105">Permissions</span></span>
<span data-ttu-id="ce0e7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce0e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce0e7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce0e7-108">Permission type</span></span>      | <span data-ttu-id="ce0e7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce0e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce0e7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce0e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce0e7-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce0e7-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce0e7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce0e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce0e7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce0e7-113">Not supported.</span></span>    |
|<span data-ttu-id="ce0e7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce0e7-114">Application</span></span> | <span data-ttu-id="ce0e7-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce0e7-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce0e7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce0e7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce0e7-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ce0e7-117">Optional query parameters</span></span>
<span data-ttu-id="ce0e7-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ce0e7-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce0e7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce0e7-119">Request headers</span></span>
| <span data-ttu-id="ce0e7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce0e7-120">Header</span></span>       | <span data-ttu-id="ce0e7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ce0e7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ce0e7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce0e7-122">Authorization</span></span>  | <span data-ttu-id="ce0e7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce0e7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ce0e7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce0e7-125">Request body</span></span>
<span data-ttu-id="ce0e7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce0e7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce0e7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce0e7-127">Response</span></span>
<span data-ttu-id="ce0e7-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [conversation](../resources/conversation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ce0e7-128">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce0e7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ce0e7-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ce0e7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce0e7-130">Request</span></span>
<span data-ttu-id="ce0e7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce0e7-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce0e7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce0e7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "get_group_conversation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="c"></a>[<span data-ttu-id="ce0e7-133">C#</span><span class="sxs-lookup"><span data-stu-id="ce0e7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce0e7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce0e7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce0e7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce0e7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce0e7-136">Java</span><span class="sxs-lookup"><span data-stu-id="ce0e7-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ce0e7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce0e7-137">Response</span></span>
<span data-ttu-id="ce0e7-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ce0e7-138">The following is an example of the response.</span></span>
><span data-ttu-id="ce0e7-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ce0e7-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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

