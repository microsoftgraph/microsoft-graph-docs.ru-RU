---
title: Подтверждение скомпрометации riskyUser
description: Подтверждение объекта riskyUser как скомпрометированного.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: ab156960911b1267ea20e7a46f2cc89fbaf9d37f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950530"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="9abb4-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="9abb4-103">riskyUser: confirmCompromised</span></span>

<span data-ttu-id="9abb4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9abb4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="9abb4-105">**Примечание:** API riskyUsers требует лицензии Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="9abb4-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="9abb4-106">Подтвердим, что один или несколько [объектов riskyUser](../resources/riskyuser.md) могут быть скомпрометированы.</span><span class="sxs-lookup"><span data-stu-id="9abb4-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="9abb4-107">Это действие задает высокий уровень риска целевого пользователя.</span><span class="sxs-lookup"><span data-stu-id="9abb4-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="9abb4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9abb4-108">Permissions</span></span>
<span data-ttu-id="9abb4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9abb4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9abb4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9abb4-111">Permission type</span></span>      | <span data-ttu-id="9abb4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9abb4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9abb4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9abb4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9abb4-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9abb4-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="9abb4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9abb4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9abb4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9abb4-116">Not supported.</span></span>    |
|<span data-ttu-id="9abb4-117">Application</span><span class="sxs-lookup"><span data-stu-id="9abb4-117">Application</span></span> | <span data-ttu-id="9abb4-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9abb4-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9abb4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9abb4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
POST /identityProtection/riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="9abb4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9abb4-120">Request headers</span></span>
| <span data-ttu-id="9abb4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9abb4-121">Name</span></span>      |<span data-ttu-id="9abb4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9abb4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9abb4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9abb4-123">Authorization</span></span>  | <span data-ttu-id="9abb4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9abb4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9abb4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9abb4-126">Request body</span></span>
<span data-ttu-id="9abb4-127">Укажите рискованные пользовательские ИД, которые необходимо отклонять в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="9abb4-127">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="9abb4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9abb4-128">Response</span></span>

<span data-ttu-id="9abb4-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9abb4-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="9abb4-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="9abb4-131">Examples</span></span>
### <a name="example-1-confirm-users-as-compromised"></a><span data-ttu-id="9abb4-132">Пример 1. Подтверждение скомпрометации пользователей</span><span class="sxs-lookup"><span data-stu-id="9abb4-132">Example 1: Confirm users as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="9abb4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9abb4-133">Request</span></span>
<span data-ttu-id="9abb4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9abb4-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9abb4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9abb4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser_1"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised
Content-type: application/json

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="9abb4-136">C#</span><span class="sxs-lookup"><span data-stu-id="9abb4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9abb4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9abb4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9abb4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9abb4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9abb4-139">Java</span><span class="sxs-lookup"><span data-stu-id="9abb4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/confirm-riskyuser-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9abb4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9abb4-140">Response</span></span>
<span data-ttu-id="9abb4-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9abb4-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
### <a name="example-2-confirm-a-user-as-compromised"></a><span data-ttu-id="9abb4-142">Пример 2. Подтверждение скомпрометации пользователя</span><span class="sxs-lookup"><span data-stu-id="9abb4-142">Example 2: Confirm a user as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="9abb4-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9abb4-143">Request</span></span>
<span data-ttu-id="9abb4-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9abb4-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9abb4-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="9abb4-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser_2"
}-->
```http
POST https://graph.microsoft.com/beta/identityProtection/riskyUsers/confirmCompromised
Content-type: application/json

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="9abb4-146">C#</span><span class="sxs-lookup"><span data-stu-id="9abb4-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9abb4-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9abb4-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9abb4-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9abb4-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9abb4-149">Java</span><span class="sxs-lookup"><span data-stu-id="9abb4-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/confirm-riskyuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9abb4-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="9abb4-150">Response</span></span>
<span data-ttu-id="9abb4-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9abb4-151">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


