---
title: Создание Итемфоне
description: Используйте этот API для создания нового Итемфоне.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 07d19b6c773f1b92a295f0c1e3471942dda45696
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996541"
---
# <a name="create-itemphonenumber"></a><span data-ttu-id="d0492-103">Создание Итемфоненумбер</span><span class="sxs-lookup"><span data-stu-id="d0492-103">Create itemPhoneNumber</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0492-104">Используйте этот API, чтобы создать новый объект [итемфоне](../resources/itemphone.md) .</span><span class="sxs-lookup"><span data-stu-id="d0492-104">Use this API to create a new [itemPhone](../resources/itemphone.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0492-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0492-105">Permissions</span></span>

<span data-ttu-id="d0492-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0492-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0492-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0492-108">Permission type</span></span>                        | <span data-ttu-id="d0492-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0492-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d0492-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0492-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0492-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d0492-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d0492-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0492-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0492-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d0492-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d0492-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0492-114">Application</span></span>                            | <span data-ttu-id="d0492-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0492-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0492-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0492-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/phones
```

## <a name="request-headers"></a><span data-ttu-id="d0492-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0492-117">Request headers</span></span>

| <span data-ttu-id="d0492-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d0492-118">Name</span></span>      |<span data-ttu-id="d0492-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d0492-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d0492-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0492-120">Authorization</span></span>  | <span data-ttu-id="d0492-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0492-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d0492-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0492-123">Content-Type</span></span>   | <span data-ttu-id="d0492-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0492-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0492-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0492-126">Request body</span></span>

<span data-ttu-id="d0492-127">В тексте запроса добавьте представление объекта [итемфоне](../resources/itemphone.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0492-127">In the request body, supply a JSON representation of [itemPhone](../resources/itemphone.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d0492-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0492-128">Response</span></span>

<span data-ttu-id="d0492-129">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [итемфоне](../resources/itemphone.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d0492-129">If successful, this method returns `201, Created` response code and a new [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0492-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="d0492-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0492-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0492-131">Request</span></span>

<span data-ttu-id="d0492-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0492-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d0492-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0492-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d0492-134">C#</span><span class="sxs-lookup"><span data-stu-id="d0492-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itemphone-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0492-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0492-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itemphone-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d0492-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0492-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itemphone-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0492-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0492-137">Response</span></span>

<span data-ttu-id="d0492-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d0492-138">The following is an example of the response.</span></span>

> <span data-ttu-id="d0492-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0492-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
