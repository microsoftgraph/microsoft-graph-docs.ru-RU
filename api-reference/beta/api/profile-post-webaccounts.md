---
title: Создание учетной записи
description: Создайте новый объект учетной записи.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: acb3750779bb56ae3a908dcd8cbf497aa357364a
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996485"
---
# <a name="create-webaccount"></a><span data-ttu-id="d3768-103">Создание учетной записи</span><span class="sxs-lookup"><span data-stu-id="d3768-103">Create webAccount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3768-104">Создайте новый объект [учетной записи](../resources/webaccount.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3768-104">Create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d3768-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3768-105">Permissions</span></span>

<span data-ttu-id="d3768-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3768-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3768-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3768-108">Permission type</span></span>                        | <span data-ttu-id="d3768-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3768-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d3768-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3768-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3768-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d3768-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d3768-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3768-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3768-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d3768-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d3768-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3768-114">Application</span></span>                            | <span data-ttu-id="d3768-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3768-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3768-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3768-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/webAccounts
```

## <a name="request-headers"></a><span data-ttu-id="d3768-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3768-117">Request headers</span></span>

| <span data-ttu-id="d3768-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d3768-118">Name</span></span>      |<span data-ttu-id="d3768-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d3768-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d3768-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3768-120">Authorization</span></span>  | <span data-ttu-id="d3768-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3768-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d3768-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3768-123">Content-Type</span></span>   | <span data-ttu-id="d3768-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3768-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3768-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3768-126">Request body</span></span>

<span data-ttu-id="d3768-127">В тексте запроса добавьте представление объекта [учетной записи](../resources/webaccount.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3768-127">In the request body, supply a JSON representation of [webAccount](../resources/webaccount.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d3768-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d3768-128">Response</span></span>

<span data-ttu-id="d3768-129">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [учетной записи](../resources/webaccount.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3768-129">If successful, this method returns `201, Created` response code and a new [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3768-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="d3768-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3768-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3768-131">Request</span></span>

<span data-ttu-id="d3768-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3768-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d3768-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3768-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_webaccount_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/webAccounts
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d3768-134">C#</span><span class="sxs-lookup"><span data-stu-id="d3768-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-webaccount-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3768-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3768-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-webaccount-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d3768-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3768-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-webaccount-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3768-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3768-137">Response</span></span>

<span data-ttu-id="d3768-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d3768-138">The following is an example of the response.</span></span>

> <span data-ttu-id="d3768-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3768-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create webAccount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
