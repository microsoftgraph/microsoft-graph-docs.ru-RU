---
title: Получение беседы
description: Удаление объекта conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 6617126b47af0a0810b2dcb0bd83de7a68f60a8d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33615021"
---
# <a name="get-conversation"></a><span data-ttu-id="f9d2f-103">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="f9d2f-103">Get conversation</span></span>
<span data-ttu-id="f9d2f-104">Удаление объекта [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="f9d2f-104">Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9d2f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9d2f-105">Permissions</span></span>
<span data-ttu-id="f9d2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9d2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9d2f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9d2f-108">Permission type</span></span>      | <span data-ttu-id="f9d2f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9d2f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9d2f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9d2f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f9d2f-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9d2f-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f9d2f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9d2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9d2f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9d2f-113">Not supported.</span></span>    |
|<span data-ttu-id="f9d2f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9d2f-114">Application</span></span> | <span data-ttu-id="f9d2f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9d2f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9d2f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9d2f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9d2f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f9d2f-117">Optional query parameters</span></span>
<span data-ttu-id="f9d2f-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f9d2f-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9d2f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9d2f-119">Request headers</span></span>
| <span data-ttu-id="f9d2f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9d2f-120">Header</span></span>       | <span data-ttu-id="f9d2f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f9d2f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f9d2f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9d2f-122">Authorization</span></span>  | <span data-ttu-id="f9d2f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9d2f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9d2f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9d2f-125">Request body</span></span>
<span data-ttu-id="f9d2f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9d2f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9d2f-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9d2f-127">Response</span></span>
<span data-ttu-id="f9d2f-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [conversation](../resources/conversation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f9d2f-128">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9d2f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f9d2f-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f9d2f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9d2f-130">Request</span></span>
<span data-ttu-id="f9d2f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9d2f-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "get_group_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="f9d2f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9d2f-132">Response</span></span>
<span data-ttu-id="f9d2f-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f9d2f-133">The following is an example of the response.</span></span>
><span data-ttu-id="f9d2f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9d2f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f9d2f-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="f9d2f-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f9d2f-137">Языках</span><span class="sxs-lookup"><span data-stu-id="f9d2f-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9d2f-138">Язык</span><span class="sxs-lookup"><span data-stu-id="f9d2f-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_conversation-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-get-conversation.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-get-conversation.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
