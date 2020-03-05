---
title: Создание Итемфоне
description: Используйте этот API для создания нового Итемфоне.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c9bea0e4f8824a4b2d968c1421e772490add4683
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455079"
---
# <a name="create-itemphonenumber"></a><span data-ttu-id="bfb6c-103">Создание Итемфоненумбер</span><span class="sxs-lookup"><span data-stu-id="bfb6c-103">Create itemPhoneNumber</span></span>

<span data-ttu-id="bfb6c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bfb6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfb6c-105">Используйте этот API, чтобы создать новый объект [итемфоне](../resources/itemphone.md) .</span><span class="sxs-lookup"><span data-stu-id="bfb6c-105">Use this API to create a new [itemPhone](../resources/itemphone.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfb6c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bfb6c-106">Permissions</span></span>

<span data-ttu-id="bfb6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfb6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bfb6c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfb6c-109">Permission type</span></span>                        | <span data-ttu-id="bfb6c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfb6c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bfb6c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfb6c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bfb6c-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bfb6c-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="bfb6c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfb6c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfb6c-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bfb6c-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="bfb6c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfb6c-115">Application</span></span>                            | <span data-ttu-id="bfb6c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfb6c-116">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfb6c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfb6c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/phones
```

## <a name="request-headers"></a><span data-ttu-id="bfb6c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfb6c-118">Request headers</span></span>

| <span data-ttu-id="bfb6c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bfb6c-119">Name</span></span>      |<span data-ttu-id="bfb6c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bfb6c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bfb6c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfb6c-121">Authorization</span></span>  | <span data-ttu-id="bfb6c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="bfb6c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bfb6c-124">Content-Type</span></span>   | <span data-ttu-id="bfb6c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfb6c-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfb6c-127">Request body</span></span>

<span data-ttu-id="bfb6c-128">В тексте запроса добавьте представление объекта [итемфоне](../resources/itemphone.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-128">In the request body, supply a JSON representation of [itemPhone](../resources/itemphone.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bfb6c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfb6c-129">Response</span></span>

<span data-ttu-id="bfb6c-130">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [итемфоне](../resources/itemphone.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-130">If successful, this method returns `201, Created` response code and a new [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bfb6c-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="bfb6c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bfb6c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfb6c-132">Request</span></span>

<span data-ttu-id="bfb6c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bfb6c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfb6c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemphone_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/phones
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```
# <a name="c"></a>[<span data-ttu-id="bfb6c-135">C#</span><span class="sxs-lookup"><span data-stu-id="bfb6c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itemphone-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfb6c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfb6c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itemphone-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfb6c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfb6c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itemphone-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bfb6c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfb6c-138">Response</span></span>

<span data-ttu-id="bfb6c-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-139">The following is an example of the response.</span></span>

> <span data-ttu-id="bfb6c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create itemPhone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
