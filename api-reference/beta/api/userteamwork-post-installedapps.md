---
title: Установка приложения для пользователя
description: Установка приложения в личной области указанного пользователя.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 37591c37f09b07baa88a47f707e0a910a0a7de40
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607756"
---
# <a name="install-app-for-user"></a><span data-ttu-id="b0b9b-103">Установка приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="b0b9b-103">Install app for user</span></span>

<span data-ttu-id="b0b9b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0b9b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0b9b-105">Установка [приложения](../resources/teamsapp.md) в личной области указанного [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="b0b9b-105">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0b9b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0b9b-106">Permissions</span></span>

<span data-ttu-id="b0b9b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0b9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0b9b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0b9b-109">Permission type</span></span>      | <span data-ttu-id="b0b9b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0b9b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0b9b-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0b9b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b0b9b-112">Теамсаппинсталлатион. Реадвритеселффорусер, Теамсаппинсталлатион. Реадвритефорусер</span><span class="sxs-lookup"><span data-stu-id="b0b9b-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="b0b9b-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0b9b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0b9b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0b9b-114">Not supported.</span></span>    |
|<span data-ttu-id="b0b9b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b0b9b-115">Application</span></span> | <span data-ttu-id="b0b9b-116">Теамсаппинсталлатион. Реадвритеселффорусер. ALL, Теамсаппинсталлатион. Реадвритефорусер. ALL</span><span class="sxs-lookup"><span data-stu-id="b0b9b-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0b9b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0b9b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{user-id}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="b0b9b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0b9b-118">Request headers</span></span>

| <span data-ttu-id="b0b9b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0b9b-119">Header</span></span>       | <span data-ttu-id="b0b9b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b0b9b-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b0b9b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0b9b-121">Authorization</span></span>  | <span data-ttu-id="b0b9b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0b9b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b0b9b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0b9b-124">Request body</span></span>

<span data-ttu-id="b0b9b-125">В тексте запроса должен содержаться идентификатор существующего приложения каталога, который требуется добавить.</span><span class="sxs-lookup"><span data-stu-id="b0b9b-125">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="b0b9b-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0b9b-126">Property</span></span>   | <span data-ttu-id="b0b9b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b0b9b-127">Type</span></span> |<span data-ttu-id="b0b9b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b0b9b-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0b9b-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b0b9b-129">teamsApp</span></span>|<span data-ttu-id="b0b9b-130">String</span><span class="sxs-lookup"><span data-stu-id="b0b9b-130">String</span></span>|<span data-ttu-id="b0b9b-131">Идентификатор добавляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="b0b9b-131">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="b0b9b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0b9b-132">Response</span></span>

<span data-ttu-id="b0b9b-p103">При успешном выполнении этот метод возвращает код отклика `201 Created`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b0b9b-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0b9b-135">Пример</span><span class="sxs-lookup"><span data-stu-id="b0b9b-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0b9b-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0b9b-136">Request</span></span>

<span data-ttu-id="b0b9b-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0b9b-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0b9b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0b9b-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->
```http
POST https://graph.microsoft.com/beta/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="c"></a>[<span data-ttu-id="b0b9b-139">C#</span><span class="sxs-lookup"><span data-stu-id="b0b9b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0b9b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0b9b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0b9b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0b9b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0b9b-142">Java</span><span class="sxs-lookup"><span data-stu-id="b0b9b-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-add-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b0b9b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0b9b-143">Response</span></span>

<span data-ttu-id="b0b9b-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b0b9b-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User add teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


