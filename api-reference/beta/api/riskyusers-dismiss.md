---
title: Отклонить Рискюсер
description: Отклонение риска для объекта Рискюсер.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: cb6d0e5aae8894408c274c4ad628e38552577d3a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453872"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="32a90-103">Рискюсер: отклонить</span><span class="sxs-lookup"><span data-stu-id="32a90-103">riskyUser: dismiss</span></span>

<span data-ttu-id="32a90-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="32a90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="32a90-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="32a90-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="32a90-106">Отклонить риск одного или нескольких объектов [рискюсер](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="32a90-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="32a90-107">Это действие задает для уровня риска целевого пользователя значение нет.</span><span class="sxs-lookup"><span data-stu-id="32a90-107">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="32a90-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32a90-108">Permissions</span></span>
<span data-ttu-id="32a90-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32a90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32a90-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32a90-111">Permission type</span></span>      | <span data-ttu-id="32a90-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32a90-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32a90-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32a90-113">Delegated (work or school account)</span></span> | <span data-ttu-id="32a90-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32a90-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="32a90-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32a90-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32a90-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32a90-116">Not supported.</span></span>    |
|<span data-ttu-id="32a90-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32a90-117">Application</span></span> | <span data-ttu-id="32a90-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32a90-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32a90-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32a90-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="32a90-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32a90-120">Request headers</span></span>
| <span data-ttu-id="32a90-121">Имя</span><span class="sxs-lookup"><span data-stu-id="32a90-121">Name</span></span>      |<span data-ttu-id="32a90-122">Описание</span><span class="sxs-lookup"><span data-stu-id="32a90-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="32a90-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32a90-123">Authorization</span></span>  | <span data-ttu-id="32a90-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32a90-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32a90-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32a90-126">Request body</span></span>
<span data-ttu-id="32a90-127">Укажите идентификаторы пользователя, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="32a90-127">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="32a90-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="32a90-128">Response</span></span>

<span data-ttu-id="32a90-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="32a90-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="32a90-131">Пример</span><span class="sxs-lookup"><span data-stu-id="32a90-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32a90-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="32a90-132">Request</span></span>
<span data-ttu-id="32a90-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32a90-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="32a90-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="32a90-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="32a90-135">C#</span><span class="sxs-lookup"><span data-stu-id="32a90-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32a90-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32a90-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32a90-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32a90-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="32a90-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="32a90-138">Response</span></span>
<span data-ttu-id="32a90-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="32a90-139">Here is an example of the response.</span></span>
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
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
