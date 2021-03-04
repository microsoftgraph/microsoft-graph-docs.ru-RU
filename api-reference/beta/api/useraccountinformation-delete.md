---
title: Удаление userAccountInformation
description: Удаление объекта userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9f922b7ed4f55b6f7a4ad4b80b6b0c9bb2125052
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433533"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="18f2f-103">Удаление userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="18f2f-103">Delete userAccountInformation</span></span>

<span data-ttu-id="18f2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18f2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18f2f-105">Удаление [объекта userAccountInformation](../resources/useraccountinformation.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="18f2f-105">Delete an [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18f2f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18f2f-106">Permissions</span></span>

<span data-ttu-id="18f2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18f2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18f2f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18f2f-109">Permission type</span></span>                        | <span data-ttu-id="18f2f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18f2f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="18f2f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18f2f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="18f2f-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f2f-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="18f2f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18f2f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18f2f-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f2f-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="18f2f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18f2f-115">Application</span></span>                            | <span data-ttu-id="18f2f-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f2f-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="18f2f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18f2f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/account/{id}
DELETE /users/{id | userPrincipalName}/profile/account/{id}
```

## <a name="request-headers"></a><span data-ttu-id="18f2f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18f2f-118">Request headers</span></span>

| <span data-ttu-id="18f2f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="18f2f-119">Name</span></span>           | <span data-ttu-id="18f2f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="18f2f-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="18f2f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18f2f-121">Authorization</span></span>  | <span data-ttu-id="18f2f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18f2f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18f2f-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18f2f-124">Request body</span></span>

<span data-ttu-id="18f2f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18f2f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18f2f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="18f2f-126">Response</span></span>

<span data-ttu-id="18f2f-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="18f2f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18f2f-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="18f2f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="18f2f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="18f2f-130">Request</span></span>

<span data-ttu-id="18f2f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18f2f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18f2f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="18f2f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/account/{id}
```
# <a name="c"></a>[<span data-ttu-id="18f2f-133">C#</span><span class="sxs-lookup"><span data-stu-id="18f2f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-useraccountinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18f2f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18f2f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-useraccountinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18f2f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18f2f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-useraccountinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18f2f-136">Java</span><span class="sxs-lookup"><span data-stu-id="18f2f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-useraccountinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18f2f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="18f2f-137">Response</span></span>

<span data-ttu-id="18f2f-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="18f2f-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

