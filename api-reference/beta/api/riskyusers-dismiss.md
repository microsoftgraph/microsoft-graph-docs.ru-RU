---
title: Отклонить Рискюсер
description: Отклонение риска для объекта Рискюсер.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: b88070f32a021f1d79aa85c091cadc52f2f600ea
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264990"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="a1a03-103">Рискюсер: отклонить</span><span class="sxs-lookup"><span data-stu-id="a1a03-103">riskyUser: dismiss</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="a1a03-104">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="a1a03-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="a1a03-105">Отклонить риск одного или нескольких объектов [рискюсер](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="a1a03-105">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="a1a03-106">Это действие задает для уровня риска целевого пользователя значение нет.</span><span class="sxs-lookup"><span data-stu-id="a1a03-106">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1a03-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1a03-107">Permissions</span></span>
<span data-ttu-id="a1a03-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1a03-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1a03-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1a03-110">Permission type</span></span>      | <span data-ttu-id="a1a03-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1a03-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1a03-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1a03-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a1a03-113">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a1a03-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="a1a03-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1a03-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1a03-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1a03-115">Not supported.</span></span>    |
|<span data-ttu-id="a1a03-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1a03-116">Application</span></span> | <span data-ttu-id="a1a03-117">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a1a03-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1a03-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1a03-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="a1a03-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1a03-119">Request headers</span></span>
| <span data-ttu-id="a1a03-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a1a03-120">Name</span></span>      |<span data-ttu-id="a1a03-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a1a03-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a1a03-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1a03-122">Authorization</span></span>  | <span data-ttu-id="a1a03-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1a03-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1a03-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1a03-125">Request body</span></span>
<span data-ttu-id="a1a03-126">Укажите идентификаторы пользователя, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="a1a03-126">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="a1a03-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1a03-127">Response</span></span>

<span data-ttu-id="a1a03-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a1a03-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a1a03-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a1a03-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1a03-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1a03-131">Request</span></span>
<span data-ttu-id="a1a03-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1a03-132">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="a1a03-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1a03-133">Response</span></span>
<span data-ttu-id="a1a03-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a1a03-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a1a03-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a1a03-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a1a03-136">C#</span><span class="sxs-lookup"><span data-stu-id="a1a03-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/dismiss_riskyuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a1a03-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a1a03-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/dismiss_riskyuser-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a1a03-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a1a03-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/dismiss_riskyuser-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-dismiss.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/riskyusers-dismiss.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-dismiss.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
