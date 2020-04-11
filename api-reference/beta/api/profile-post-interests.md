---
title: Создание Персонинтерест
description: Создание нового Персонинтерест.
localization_priority: Normal
author: kevinbellinger
ms.prod: People
doc_type: apiPageType
ms.openlocfilehash: f0d4f406004d80121f2cd9ac44b39f303af71861
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229334"
---
# <a name="create-personinterest"></a><span data-ttu-id="26ce4-103">Создание Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="26ce4-103">Create personInterest</span></span>

<span data-ttu-id="26ce4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26ce4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26ce4-105">Создание нового объекта [Персонинтерест] (.. /ресаурцес/персонинтерест.МД].</span><span class="sxs-lookup"><span data-stu-id="26ce4-105">Create a new [personInterest](../resources/personinterest.md].</span></span>

## <a name="permissions"></a><span data-ttu-id="26ce4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26ce4-106">Permissions</span></span>

<span data-ttu-id="26ce4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26ce4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26ce4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26ce4-109">Permission type</span></span>                        | <span data-ttu-id="26ce4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26ce4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26ce4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26ce4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="26ce4-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="26ce4-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="26ce4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26ce4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26ce4-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="26ce4-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="26ce4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26ce4-115">Application</span></span>                            | <span data-ttu-id="26ce4-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26ce4-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="26ce4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26ce4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/interests
```

## <a name="request-headers"></a><span data-ttu-id="26ce4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26ce4-118">Request headers</span></span>

| <span data-ttu-id="26ce4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="26ce4-119">Name</span></span>      |<span data-ttu-id="26ce4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="26ce4-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="26ce4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26ce4-121">Authorization</span></span>  | <span data-ttu-id="26ce4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26ce4-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="26ce4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26ce4-124">Content-Type</span></span>   | <span data-ttu-id="26ce4-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26ce4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26ce4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26ce4-127">Request body</span></span>

<span data-ttu-id="26ce4-128">В тексте запроса добавьте представление объекта [персонинтерест](../resources/personinterest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26ce4-128">In the request body, supply a JSON representation of [personInterest](../resources/personinterest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="26ce4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="26ce4-129">Response</span></span>

<span data-ttu-id="26ce4-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [персонинтерест](../resources/personinterest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26ce4-130">If successful, this method returns a `201 Created` response code and a new [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26ce4-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="26ce4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26ce4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="26ce4-132">Request</span></span>

<span data-ttu-id="26ce4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26ce4-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26ce4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="26ce4-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="26ce4-135">C#</span><span class="sxs-lookup"><span data-stu-id="26ce4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personinterest-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26ce4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26ce4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personinterest-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26ce4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26ce4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personinterest-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26ce4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="26ce4-138">Response</span></span>

<span data-ttu-id="26ce4-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="26ce4-139">The following is an example of the response.</span></span>

> <span data-ttu-id="26ce4-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26ce4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
