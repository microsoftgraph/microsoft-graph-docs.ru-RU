---
title: Отклонить Рискюсер
description: Отклонение риска для объекта Рискюсер.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 7812235ceecc1304711c715e2aaa6640e684277e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358211"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="b662b-103">Рискюсер: отклонить</span><span class="sxs-lookup"><span data-stu-id="b662b-103">riskyUser: dismiss</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="b662b-104">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="b662b-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="b662b-105">Отклонить риск одного или нескольких объектов [рискюсер](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="b662b-105">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="b662b-106">Это действие задает для уровня риска целевого пользователя значение нет.</span><span class="sxs-lookup"><span data-stu-id="b662b-106">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="b662b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b662b-107">Permissions</span></span>
<span data-ttu-id="b662b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b662b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b662b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b662b-110">Permission type</span></span>      | <span data-ttu-id="b662b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b662b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b662b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b662b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b662b-113">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b662b-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="b662b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b662b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b662b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b662b-115">Not supported.</span></span>    |
|<span data-ttu-id="b662b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b662b-116">Application</span></span> | <span data-ttu-id="b662b-117">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b662b-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b662b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b662b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="b662b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b662b-119">Request headers</span></span>
| <span data-ttu-id="b662b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b662b-120">Name</span></span>      |<span data-ttu-id="b662b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b662b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b662b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b662b-122">Authorization</span></span>  | <span data-ttu-id="b662b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b662b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b662b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b662b-125">Request body</span></span>
<span data-ttu-id="b662b-126">Укажите идентификаторы пользователя, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="b662b-126">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="b662b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b662b-127">Response</span></span>

<span data-ttu-id="b662b-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b662b-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b662b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b662b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b662b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b662b-131">Request</span></span>
<span data-ttu-id="b662b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b662b-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b662b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b662b-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b662b-134">C#</span><span class="sxs-lookup"><span data-stu-id="b662b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b662b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b662b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b662b-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b662b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b662b-137">Java</span><span class="sxs-lookup"><span data-stu-id="b662b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/dismiss-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b662b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b662b-138">Response</span></span>
<span data-ttu-id="b662b-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b662b-139">Here is an example of the response.</span></span>
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
