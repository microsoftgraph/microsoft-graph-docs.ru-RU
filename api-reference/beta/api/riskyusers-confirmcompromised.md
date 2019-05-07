---
title: Подтверждение Рискюсер скомпрометированных атак
description: Подтвердите, что объект Рискюсер скомпрометирован.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: f0ce7b0a29b90f12104a697bdc38f3297e52676e
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639035"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="91b7e-103">Рискюсер: Конфирмкомпромисед</span><span class="sxs-lookup"><span data-stu-id="91b7e-103">riskyUser: confirmCompromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="91b7e-104">**Примечание:** Для API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="91b7e-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="91b7e-105">Подтвердите, что один или несколько объектов [рискюсер](../resources/riskyuser.md) считаются скомпрометированными.</span><span class="sxs-lookup"><span data-stu-id="91b7e-105">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="91b7e-106">Это действие устанавливает высокий уровень риска для целевого пользователя.</span><span class="sxs-lookup"><span data-stu-id="91b7e-106">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="91b7e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91b7e-107">Permissions</span></span>
<span data-ttu-id="91b7e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91b7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91b7e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91b7e-110">Permission type</span></span>      | <span data-ttu-id="91b7e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91b7e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91b7e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91b7e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="91b7e-113">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="91b7e-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="91b7e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91b7e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91b7e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91b7e-115">Not supported.</span></span>    |
|<span data-ttu-id="91b7e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91b7e-116">Application</span></span> | <span data-ttu-id="91b7e-117">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="91b7e-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91b7e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91b7e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="91b7e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91b7e-119">Request headers</span></span>
| <span data-ttu-id="91b7e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="91b7e-120">Name</span></span>      |<span data-ttu-id="91b7e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="91b7e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91b7e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91b7e-122">Authorization</span></span>  | <span data-ttu-id="91b7e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91b7e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91b7e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91b7e-125">Request body</span></span>
<span data-ttu-id="91b7e-126">Укажите рискованные идентификаторы пользователей, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="91b7e-126">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="91b7e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="91b7e-127">Response</span></span>

<span data-ttu-id="91b7e-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="91b7e-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91b7e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="91b7e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91b7e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="91b7e-131">Request</span></span>
<span data-ttu-id="91b7e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91b7e-132">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="91b7e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="91b7e-133">Response</span></span>
<span data-ttu-id="91b7e-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="91b7e-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="91b7e-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="91b7e-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="91b7e-136">Языках</span><span class="sxs-lookup"><span data-stu-id="91b7e-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/confirm_riskyuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91b7e-137">Язык</span><span class="sxs-lookup"><span data-stu-id="91b7e-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/confirm_riskyuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
