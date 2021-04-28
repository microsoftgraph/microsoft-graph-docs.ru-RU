---
title: 'mailFolder: copy'
description: Копирование папки почты со всем ее содержимым в другую папку почты.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0c40d7bda2c0878a17b0268de8934a1aeda2debb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049522"
---
# <a name="mailfolder-copy"></a><span data-ttu-id="ada47-103">mailFolder: copy</span><span class="sxs-lookup"><span data-stu-id="ada47-103">mailFolder: copy</span></span>

<span data-ttu-id="ada47-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ada47-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ada47-105">Копирование папки почты со всем ее содержимым в другую папку почты.</span><span class="sxs-lookup"><span data-stu-id="ada47-105">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ada47-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ada47-106">Permissions</span></span>

<span data-ttu-id="ada47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ada47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ada47-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ada47-109">Permission type</span></span> | <span data-ttu-id="ada47-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ada47-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="ada47-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ada47-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ada47-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ada47-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ada47-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ada47-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ada47-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ada47-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ada47-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ada47-115">Application</span></span> | <span data-ttu-id="ada47-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ada47-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ada47-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ada47-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="ada47-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ada47-118">Request headers</span></span>
| <span data-ttu-id="ada47-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ada47-119">Header</span></span> | <span data-ttu-id="ada47-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ada47-120">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="ada47-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ada47-121">Authorization</span></span> | <span data-ttu-id="ada47-122">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="ada47-122">`Bearer {token}`.</span></span> <span data-ttu-id="ada47-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ada47-123">Required.</span></span> |
| <span data-ttu-id="ada47-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ada47-124">Content-Type</span></span> | <span data-ttu-id="ada47-125">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="ada47-125">`application/json`.</span></span> <span data-ttu-id="ada47-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ada47-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ada47-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ada47-127">Request body</span></span>

<span data-ttu-id="ada47-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ada47-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ada47-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="ada47-129">Parameter</span></span> | <span data-ttu-id="ada47-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ada47-130">Type</span></span> | <span data-ttu-id="ada47-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ada47-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="ada47-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="ada47-132">destinationId</span></span>|<span data-ttu-id="ada47-133">String</span><span class="sxs-lookup"><span data-stu-id="ada47-133">String</span></span>|<span data-ttu-id="ada47-134">ID папки или хорошо известное имя папки.</span><span class="sxs-lookup"><span data-stu-id="ada47-134">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="ada47-135">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ada47-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="ada47-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ada47-136">Response</span></span>

<span data-ttu-id="ada47-137">В случае успешного использования этот метод возвращает код ответа и ресурс `200 OK` [mailFolder](../resources/mailfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ada47-137">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ada47-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ada47-138">Example</span></span>

<span data-ttu-id="ada47-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ada47-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ada47-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="ada47-140">Request</span></span>
<span data-ttu-id="ada47-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ada47-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ada47-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ada47-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="ada47-143">C#</span><span class="sxs-lookup"><span data-stu-id="ada47-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ada47-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ada47-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ada47-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ada47-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ada47-146">Java</span><span class="sxs-lookup"><span data-stu-id="ada47-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-copy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ada47-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="ada47-147">Response</span></span>

<span data-ttu-id="ada47-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ada47-148">Here is an example of the response.</span></span>

> <span data-ttu-id="ada47-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ada47-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

