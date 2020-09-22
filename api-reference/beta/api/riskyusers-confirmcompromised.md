---
title: Подтверждение Рискюсер скомпрометированных атак
description: Подтвердите, что объект Рискюсер скомпрометирован.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 9954565c2be8b239671d74e55e875ea2b01c229b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085342"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="8977c-103">Рискюсер: Конфирмкомпромисед</span><span class="sxs-lookup"><span data-stu-id="8977c-103">riskyUser: confirmCompromised</span></span>

<span data-ttu-id="8977c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8977c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="8977c-105">**Примечание:** Для API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="8977c-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="8977c-106">Подтвердите, что один или несколько объектов [рискюсер](../resources/riskyuser.md) считаются скомпрометированными.</span><span class="sxs-lookup"><span data-stu-id="8977c-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="8977c-107">Это действие устанавливает высокий уровень риска для целевого пользователя.</span><span class="sxs-lookup"><span data-stu-id="8977c-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="8977c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8977c-108">Permissions</span></span>
<span data-ttu-id="8977c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8977c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8977c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8977c-111">Permission type</span></span>      | <span data-ttu-id="8977c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8977c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8977c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8977c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8977c-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8977c-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="8977c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8977c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8977c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8977c-116">Not supported.</span></span>    |
|<span data-ttu-id="8977c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8977c-117">Application</span></span> | <span data-ttu-id="8977c-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8977c-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8977c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8977c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
POST /identityProtection/riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="8977c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8977c-120">Request headers</span></span>
| <span data-ttu-id="8977c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8977c-121">Name</span></span>      |<span data-ttu-id="8977c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8977c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8977c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8977c-123">Authorization</span></span>  | <span data-ttu-id="8977c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8977c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8977c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8977c-126">Request body</span></span>
<span data-ttu-id="8977c-127">Укажите рискованные идентификаторы пользователей, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="8977c-127">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="8977c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8977c-128">Response</span></span>

<span data-ttu-id="8977c-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8977c-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="8977c-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8977c-131">Examples</span></span>
### <a name="example-1-confirm-users-as-compromised"></a><span data-ttu-id="8977c-132">Пример 1: подтверждение раскрытого пользователя</span><span class="sxs-lookup"><span data-stu-id="8977c-132">Example 1: Confirm users as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="8977c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8977c-133">Request</span></span>
<span data-ttu-id="8977c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8977c-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8977c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8977c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
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
# <a name="c"></a>[<span data-ttu-id="8977c-136">C#</span><span class="sxs-lookup"><span data-stu-id="8977c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8977c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8977c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8977c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8977c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8977c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8977c-139">Response</span></span>
<span data-ttu-id="8977c-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8977c-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
### <a name="example-2-confirm-a-user-as-compromised"></a><span data-ttu-id="8977c-141">Пример 2: подтверждение раскрытого пользователя</span><span class="sxs-lookup"><span data-stu-id="8977c-141">Example 2: Confirm a user as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="8977c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8977c-142">Request</span></span>
<span data-ttu-id="8977c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8977c-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8977c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="8977c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
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
# <a name="c"></a>[<span data-ttu-id="8977c-145">C#</span><span class="sxs-lookup"><span data-stu-id="8977c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8977c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8977c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8977c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8977c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8977c-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8977c-148">Response</span></span>
<span data-ttu-id="8977c-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8977c-149">Here is an example of the response.</span></span>
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


