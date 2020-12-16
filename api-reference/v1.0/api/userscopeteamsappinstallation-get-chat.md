---
title: Получить 1:1 чат между указанным пользователем и приложением Teams
description: Извлечение чата по одному между указанным пользователем и приложением Teams.
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7d6d4d7c2c0862cc5e0f3335fede8f940381b538
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689479"
---
# <a name="get-one-on-one-chat-between-the-specified-user-and-teams-app"></a><span data-ttu-id="f6506-103">Получить один-на-один чат между указанным пользователем и приложением Teams</span><span class="sxs-lookup"><span data-stu-id="f6506-103">Get one-on-one chat between the specified user and Teams app</span></span>

<span data-ttu-id="f6506-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6506-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f6506-105">[Извлечение чата](../resources/chat.md) указанного [пользователя и](../resources/user.md) [приложения Teams.](../resources/teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6506-105">Retrieve the [chat](../resources/chat.md) of the specified [user](../resources/user.md) and [Teams app](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6506-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6506-106">Permissions</span></span>

<span data-ttu-id="f6506-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6506-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6506-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6506-109">Permission type</span></span>      | <span data-ttu-id="f6506-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6506-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6506-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6506-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6506-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="f6506-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="f6506-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6506-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6506-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6506-114">Not supported.</span></span>    |
|<span data-ttu-id="f6506-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f6506-115">Application</span></span> | <span data-ttu-id="f6506-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="f6506-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6506-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6506-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id}/teamwork/installedApps/{app-installation-id}/chat
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6506-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6506-118">Optional query parameters</span></span>

<span data-ttu-id="f6506-119">Этот метод поддерживает параметр `$select` [запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f6506-119">This method supports the `$select` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6506-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6506-120">Request headers</span></span>

| <span data-ttu-id="f6506-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6506-121">Header</span></span>       | <span data-ttu-id="f6506-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f6506-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f6506-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6506-123">Authorization</span></span>  | <span data-ttu-id="f6506-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6506-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6506-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6506-126">Request body</span></span>

<span data-ttu-id="f6506-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6506-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6506-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6506-128">Response</span></span>

<span data-ttu-id="f6506-129">В случае успеха этот метод возвращает код отклика и экземпляр объекта `200 OK` [чата](../resources/chat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6506-129">If successful, this method returns a `200 OK` response code and an instance of [chat](../resources/chat.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f6506-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="f6506-130">Examples</span></span>

### <a name="example-1-list-one-on-one-chats-between-the-specified-user-and-the-teams-app"></a><span data-ttu-id="f6506-131">Пример 1. Список чаты по одному между указанным пользователем и приложением Teams</span><span class="sxs-lookup"><span data-stu-id="f6506-131">Example 1: List one-on-one chats between the specified user and the Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="f6506-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6506-132">Request</span></span>

<span data-ttu-id="f6506-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6506-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f6506-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6506-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_chat_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c/teamwork/installedApps/ZjMyYjgzYmItNGZjOC00ZGI3LWI3ZjUtNzZjZGJiYjhhYTFjIyMyMmY3M2JiZS1mNjdhLTRkZWEtYmQ1NC01NGNhYzcxOGNiMmI=/chat
```
# <a name="c"></a>[<span data-ttu-id="f6506-135">C#</span><span class="sxs-lookup"><span data-stu-id="f6506-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-chat-teamsapps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6506-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6506-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-chat-teamsapps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6506-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6506-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-chat-teamsapps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6506-138">Java</span><span class="sxs-lookup"><span data-stu-id="f6506-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-chat-teamsapps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f6506-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6506-139">Response</span></span>

<span data-ttu-id="f6506-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6506-140">The following is an example of the response.</span></span>
><span data-ttu-id="f6506-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6506-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
   "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats/$entity",
   "id": "19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c@unq.gbl.spaces"
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
