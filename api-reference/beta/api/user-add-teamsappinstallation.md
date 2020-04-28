---
title: Установка приложения для пользователя
description: Установка приложения в личной области указанного пользователя.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4454674ae214f483741da80f1a594f3f0db8fded
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452045"
---
# <a name="install-app-for-user"></a><span data-ttu-id="561b2-103">Установка приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="561b2-103">Install app for user</span></span>

<span data-ttu-id="561b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="561b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="561b2-105">Установка [приложения](../resources/teamsapp.md) в личной области указанного [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="561b2-105">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="561b2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="561b2-106">Permissions</span></span>

<span data-ttu-id="561b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="561b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="561b2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="561b2-109">Permission type</span></span>      | <span data-ttu-id="561b2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="561b2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="561b2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="561b2-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="561b2-112">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="561b2-112">User.ReadWrite.All, Directory.ReadWrite.All</span></span>     |
|<span data-ttu-id="561b2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="561b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="561b2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="561b2-114">Not supported.</span></span>    |
|<span data-ttu-id="561b2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="561b2-115">Application</span></span> | <span data-ttu-id="561b2-116">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="561b2-116">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="561b2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="561b2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="561b2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="561b2-118">Request headers</span></span>

| <span data-ttu-id="561b2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="561b2-119">Header</span></span>       | <span data-ttu-id="561b2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="561b2-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="561b2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="561b2-121">Authorization</span></span>  | <span data-ttu-id="561b2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="561b2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="561b2-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="561b2-124">Request body</span></span>

<span data-ttu-id="561b2-125">В тексте запроса должен содержаться идентификатор существующего приложения каталога, который требуется добавить.</span><span class="sxs-lookup"><span data-stu-id="561b2-125">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="561b2-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="561b2-126">Property</span></span>   | <span data-ttu-id="561b2-127">Тип</span><span class="sxs-lookup"><span data-stu-id="561b2-127">Type</span></span> |<span data-ttu-id="561b2-128">Описание</span><span class="sxs-lookup"><span data-stu-id="561b2-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="561b2-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="561b2-129">teamsApp</span></span>|<span data-ttu-id="561b2-130">String</span><span class="sxs-lookup"><span data-stu-id="561b2-130">String</span></span>|<span data-ttu-id="561b2-131">Идентификатор добавляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="561b2-131">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="561b2-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="561b2-132">Response</span></span>

<span data-ttu-id="561b2-p103">При успешном выполнении этот метод возвращает код отклика `201 Created`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="561b2-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="561b2-135">Пример</span><span class="sxs-lookup"><span data-stu-id="561b2-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="561b2-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="561b2-136">Request</span></span>

<span data-ttu-id="561b2-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="561b2-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="561b2-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="561b2-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="561b2-139">C#</span><span class="sxs-lookup"><span data-stu-id="561b2-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="561b2-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="561b2-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="561b2-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="561b2-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="561b2-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="561b2-142">Response</span></span>

<span data-ttu-id="561b2-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="561b2-143">The following is an example of the response.</span></span>

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
