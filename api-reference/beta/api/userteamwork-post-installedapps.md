---
title: Установка приложения для пользователя
description: Установка приложения в личной области указанного пользователя.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9a39bc198e742f2b5b1b15cbdbf02a96a980c708
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696284"
---
# <a name="install-app-for-user"></a><span data-ttu-id="00432-103">Установка приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="00432-103">Install app for user</span></span>

<span data-ttu-id="00432-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00432-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00432-105">Установите [приложение в](../resources/teamsapp.md) личной области указанного [пользователя.](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="00432-105">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="00432-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00432-106">Permissions</span></span>

<span data-ttu-id="00432-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00432-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00432-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00432-109">Permission type</span></span>      | <span data-ttu-id="00432-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00432-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00432-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00432-111">Delegated (work or school account)</span></span> | <span data-ttu-id="00432-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="00432-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="00432-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00432-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00432-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00432-114">Not supported.</span></span>    |
|<span data-ttu-id="00432-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="00432-115">Application</span></span> | <span data-ttu-id="00432-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="00432-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00432-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00432-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{user-id | user-principal-name}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="00432-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00432-118">Request headers</span></span>

| <span data-ttu-id="00432-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00432-119">Header</span></span>       | <span data-ttu-id="00432-120">Значение</span><span class="sxs-lookup"><span data-stu-id="00432-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="00432-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00432-121">Authorization</span></span>  | <span data-ttu-id="00432-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00432-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00432-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00432-124">Request body</span></span>

<span data-ttu-id="00432-125">В теле запроса должен быть добавлен ID существующего приложения каталога.</span><span class="sxs-lookup"><span data-stu-id="00432-125">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="00432-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="00432-126">Property</span></span>   | <span data-ttu-id="00432-127">Тип</span><span class="sxs-lookup"><span data-stu-id="00432-127">Type</span></span> |<span data-ttu-id="00432-128">Описание</span><span class="sxs-lookup"><span data-stu-id="00432-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00432-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="00432-129">teamsApp</span></span>|<span data-ttu-id="00432-130">String</span><span class="sxs-lookup"><span data-stu-id="00432-130">String</span></span>|<span data-ttu-id="00432-131">ID приложения для добавления.</span><span class="sxs-lookup"><span data-stu-id="00432-131">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="00432-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="00432-132">Response</span></span>

<span data-ttu-id="00432-p103">При успешном выполнении этот метод возвращает код отклика `201 Created`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="00432-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00432-135">Пример</span><span class="sxs-lookup"><span data-stu-id="00432-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="00432-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="00432-136">Request</span></span>

<span data-ttu-id="00432-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00432-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="00432-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="00432-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="00432-139">C#</span><span class="sxs-lookup"><span data-stu-id="00432-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00432-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00432-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00432-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00432-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00432-142">Java</span><span class="sxs-lookup"><span data-stu-id="00432-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-add-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="00432-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="00432-143">Response</span></span>

<span data-ttu-id="00432-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="00432-144">The following is an example of the response.</span></span>

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


