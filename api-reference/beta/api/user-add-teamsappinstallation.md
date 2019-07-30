---
title: Установка приложения для пользователя
description: Установка приложения в личной области указанного пользователя.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 08c0339c7d8923a5d6988245d8b2f488197c82ba
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931463"
---
# <a name="install-app-for-user"></a><span data-ttu-id="003f8-103">Установка приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="003f8-103">Install app for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="003f8-104">Установка [приложения](../resources/teamsapp.md) в личной области указанного [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="003f8-104">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="003f8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="003f8-105">Permissions</span></span>

<span data-ttu-id="003f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="003f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="003f8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="003f8-108">Permission type</span></span>      | <span data-ttu-id="003f8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="003f8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="003f8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="003f8-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="003f8-111">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="003f8-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>     |
|<span data-ttu-id="003f8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="003f8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="003f8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="003f8-113">Not supported.</span></span>    |
|<span data-ttu-id="003f8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="003f8-114">Application</span></span> | <span data-ttu-id="003f8-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="003f8-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="003f8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="003f8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="003f8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="003f8-117">Request headers</span></span>

| <span data-ttu-id="003f8-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="003f8-118">Header</span></span>       | <span data-ttu-id="003f8-119">Значение</span><span class="sxs-lookup"><span data-stu-id="003f8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="003f8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="003f8-120">Authorization</span></span>  | <span data-ttu-id="003f8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="003f8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="003f8-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="003f8-123">Request body</span></span>

<span data-ttu-id="003f8-124">В тексте запроса должен содержаться идентификатор существующего приложения каталога, который требуется добавить.</span><span class="sxs-lookup"><span data-stu-id="003f8-124">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="003f8-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="003f8-125">Property</span></span>   | <span data-ttu-id="003f8-126">Тип</span><span class="sxs-lookup"><span data-stu-id="003f8-126">Type</span></span> |<span data-ttu-id="003f8-127">Описание</span><span class="sxs-lookup"><span data-stu-id="003f8-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="003f8-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="003f8-128">teamsApp</span></span>|<span data-ttu-id="003f8-129">String</span><span class="sxs-lookup"><span data-stu-id="003f8-129">String</span></span>|<span data-ttu-id="003f8-130">Идентификатор добавляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="003f8-130">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="003f8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="003f8-131">Response</span></span>

<span data-ttu-id="003f8-p103">При успешном выполнении этот метод возвращает код отклика `201 Created`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="003f8-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="003f8-134">Пример</span><span class="sxs-lookup"><span data-stu-id="003f8-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="003f8-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="003f8-135">Request</span></span>

<span data-ttu-id="003f8-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="003f8-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="003f8-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="003f8-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="003f8-138">C#</span><span class="sxs-lookup"><span data-stu-id="003f8-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="003f8-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="003f8-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="003f8-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="003f8-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="003f8-141">Java</span><span class="sxs-lookup"><span data-stu-id="003f8-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-add-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="003f8-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="003f8-142">Response</span></span>

<span data-ttu-id="003f8-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="003f8-143">The following is an example of the response.</span></span>

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
