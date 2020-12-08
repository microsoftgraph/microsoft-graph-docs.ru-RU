---
title: Получение разговора между пользователем и teamsApp
description: Получение одного сеанса разговора между указанным пользователем и приложением Teams.
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f4d7d9e6534b13746824a2d7a0e4b19d826acb41
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597286"
---
# <a name="get-chat-between-user-and-teamsapp"></a><span data-ttu-id="c0c02-103">Получение разговора между пользователем и teamsApp</span><span class="sxs-lookup"><span data-stu-id="c0c02-103">Get chat between user and teamsApp</span></span>

<span data-ttu-id="c0c02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0c02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0c02-105">Получение [чата](../resources/chat.md) для указанного [пользователя](../resources/user.md) и [приложения Teams](../resources/teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="c0c02-105">Retrieve the [chat](../resources/chat.md) of the specified [user](../resources/user.md) and [Teams app](../resources/teamsapp.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="c0c02-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0c02-106">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps/{id}/chat
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0c02-107">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c0c02-107">Optional query parameters</span></span>

<span data-ttu-id="c0c02-108">Этот метод поддерживает `$select` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c0c02-108">This method supports the `$select` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0c02-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0c02-109">Request headers</span></span>

| <span data-ttu-id="c0c02-110">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0c02-110">Header</span></span>       | <span data-ttu-id="c0c02-111">Значение</span><span class="sxs-lookup"><span data-stu-id="c0c02-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c0c02-112">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0c02-112">Authorization</span></span>  | <span data-ttu-id="c0c02-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0c02-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0c02-115">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0c02-115">Request body</span></span>

<span data-ttu-id="c0c02-116">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0c02-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0c02-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0c02-117">Response</span></span>

<span data-ttu-id="c0c02-118">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и экземпляр объекта [Chat](../resources/chat.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c0c02-118">If successful, this method returns a `200 OK` response code and an instance of [chat](../resources/chat.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0c02-119">Примеры</span><span class="sxs-lookup"><span data-stu-id="c0c02-119">Examples</span></span>

### <a name="example-1-list-one-on-one-chats-between-the-specified-user-and-the-teams-app"></a><span data-ttu-id="c0c02-120">Пример 1: список бесед одного пользователя между указанным пользователем и приложением Teams</span><span class="sxs-lookup"><span data-stu-id="c0c02-120">Example 1: List one-on-one chats between the specified user and the Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="c0c02-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0c02-121">Request</span></span>

<span data-ttu-id="c0c02-122">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0c02-122">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_chat_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}/chat
```

#### <a name="response"></a><span data-ttu-id="c0c02-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0c02-123">Response</span></span>

<span data-ttu-id="c0c02-124">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c0c02-124">The following is an example of the response.</span></span>
><span data-ttu-id="c0c02-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0c02-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_chat_teamsApps",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#chats/$entity",
   "id":"19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c@unq.gbl.spaces"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User chat teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
