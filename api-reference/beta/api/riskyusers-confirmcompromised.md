---
title: Подтверждение Рискюсер скомпрометированных атак
description: Подтвердите, что объект Рискюсер скомпрометирован.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 1e234ecb92084bc0c180b4b069cfa7f7ce38629a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453886"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="db85d-103">Рискюсер: Конфирмкомпромисед</span><span class="sxs-lookup"><span data-stu-id="db85d-103">riskyUser: confirmCompromised</span></span>

<span data-ttu-id="db85d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="db85d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="db85d-105">**Примечание:** Для API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="db85d-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="db85d-106">Подтвердите, что один или несколько объектов [рискюсер](../resources/riskyuser.md) считаются скомпрометированными.</span><span class="sxs-lookup"><span data-stu-id="db85d-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="db85d-107">Это действие устанавливает высокий уровень риска для целевого пользователя.</span><span class="sxs-lookup"><span data-stu-id="db85d-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="db85d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db85d-108">Permissions</span></span>
<span data-ttu-id="db85d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db85d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db85d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db85d-111">Permission type</span></span>      | <span data-ttu-id="db85d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db85d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db85d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db85d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="db85d-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db85d-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="db85d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db85d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db85d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db85d-116">Not supported.</span></span>    |
|<span data-ttu-id="db85d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db85d-117">Application</span></span> | <span data-ttu-id="db85d-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db85d-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db85d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db85d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="db85d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db85d-120">Request headers</span></span>
| <span data-ttu-id="db85d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="db85d-121">Name</span></span>      |<span data-ttu-id="db85d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="db85d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db85d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db85d-123">Authorization</span></span>  | <span data-ttu-id="db85d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db85d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db85d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db85d-126">Request body</span></span>
<span data-ttu-id="db85d-127">Укажите рискованные идентификаторы пользователей, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="db85d-127">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="db85d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="db85d-128">Response</span></span>

<span data-ttu-id="db85d-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="db85d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db85d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="db85d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db85d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="db85d-132">Request</span></span>
<span data-ttu-id="db85d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db85d-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db85d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="db85d-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="db85d-135">C#</span><span class="sxs-lookup"><span data-stu-id="db85d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db85d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db85d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db85d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db85d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db85d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="db85d-138">Response</span></span>
<span data-ttu-id="db85d-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db85d-139">Here is an example of the response.</span></span>
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
