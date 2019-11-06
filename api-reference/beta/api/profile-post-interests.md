---
title: Создание Персонинтерест
description: Создание нового Персонинтерест.
localization_priority: Normal
author: kevinbellinger
ms.prod: People
doc_type: apiPageType
ms.openlocfilehash: ea7a3df0edcab0ed5b4f5cdf2307f01393772b13
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997832"
---
# <a name="create-personinterest"></a><span data-ttu-id="54fa9-103">Создание Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="54fa9-103">Create personInterest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54fa9-104">Создание нового объекта [Персонинтерест] (.. /ресаурцес/персонинтерест.МД].</span><span class="sxs-lookup"><span data-stu-id="54fa9-104">Create a new [personInterest](../resources/personinterest.md].</span></span>

## <a name="permissions"></a><span data-ttu-id="54fa9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54fa9-105">Permissions</span></span>

<span data-ttu-id="54fa9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54fa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54fa9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54fa9-108">Permission type</span></span>                        | <span data-ttu-id="54fa9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54fa9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="54fa9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54fa9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="54fa9-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="54fa9-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="54fa9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54fa9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54fa9-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="54fa9-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="54fa9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54fa9-114">Application</span></span>                            | <span data-ttu-id="54fa9-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54fa9-115">User.ReadWrite.All</span></span> |
## <a name="http-request"></a><span data-ttu-id="54fa9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54fa9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/interests
```

## <a name="request-headers"></a><span data-ttu-id="54fa9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54fa9-117">Request headers</span></span>

| <span data-ttu-id="54fa9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="54fa9-118">Name</span></span>      |<span data-ttu-id="54fa9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="54fa9-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="54fa9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54fa9-120">Authorization</span></span>  | <span data-ttu-id="54fa9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54fa9-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="54fa9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54fa9-123">Content-Type</span></span>   | <span data-ttu-id="54fa9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54fa9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54fa9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54fa9-126">Request body</span></span>

<span data-ttu-id="54fa9-127">В тексте запроса добавьте представление объекта [персонинтерест](../resources/personinterest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54fa9-127">In the request body, supply a JSON representation of [personInterest](../resources/personinterest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="54fa9-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="54fa9-128">Response</span></span>

<span data-ttu-id="54fa9-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [персонинтерест](../resources/personinterest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="54fa9-129">If successful, this method returns a `201 Created` response code and a new [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54fa9-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="54fa9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54fa9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="54fa9-131">Request</span></span>

<span data-ttu-id="54fa9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54fa9-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="54fa9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="54fa9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personinterest_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/interests
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="54fa9-134">C#</span><span class="sxs-lookup"><span data-stu-id="54fa9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personinterest-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="54fa9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54fa9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personinterest-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="54fa9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54fa9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personinterest-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="54fa9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="54fa9-137">Response</span></span>

<span data-ttu-id="54fa9-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54fa9-138">The following is an example of the response.</span></span>

> <span data-ttu-id="54fa9-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54fa9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personInterest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
