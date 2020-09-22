---
title: 'mailFolder: copy'
description: Копирование папки почты со всем ее содержимым в другую папку почты.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c66a49b062e7d4d4ba9ec953d21120fd397cb2fb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033120"
---
# <a name="mailfolder-copy"></a><span data-ttu-id="1f887-103">mailFolder: copy</span><span class="sxs-lookup"><span data-stu-id="1f887-103">mailFolder: copy</span></span>

<span data-ttu-id="1f887-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f887-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f887-105">Копирование папки почты со всем ее содержимым в другую папку почты.</span><span class="sxs-lookup"><span data-stu-id="1f887-105">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f887-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f887-106">Permissions</span></span>

<span data-ttu-id="1f887-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f887-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f887-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f887-109">Permission type</span></span> | <span data-ttu-id="1f887-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f887-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="1f887-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f887-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1f887-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f887-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1f887-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f887-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f887-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f887-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1f887-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f887-115">Application</span></span> | <span data-ttu-id="1f887-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f887-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f887-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f887-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="1f887-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f887-118">Request headers</span></span>
| <span data-ttu-id="1f887-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f887-119">Header</span></span> | <span data-ttu-id="1f887-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1f887-120">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="1f887-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f887-121">Authorization</span></span> | <span data-ttu-id="1f887-122">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="1f887-122">`Bearer {token}`.</span></span> <span data-ttu-id="1f887-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="1f887-123">Required.</span></span> |
| <span data-ttu-id="1f887-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f887-124">Content-Type</span></span> | <span data-ttu-id="1f887-125">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="1f887-125">`application/json`.</span></span> <span data-ttu-id="1f887-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="1f887-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f887-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1f887-127">Request body</span></span>

<span data-ttu-id="1f887-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1f887-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1f887-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="1f887-129">Parameter</span></span> | <span data-ttu-id="1f887-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1f887-130">Type</span></span> | <span data-ttu-id="1f887-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1f887-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="1f887-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="1f887-132">destinationId</span></span>|<span data-ttu-id="1f887-133">String</span><span class="sxs-lookup"><span data-stu-id="1f887-133">String</span></span>|<span data-ttu-id="1f887-134">Идентификатор папки или имя известной папки.</span><span class="sxs-lookup"><span data-stu-id="1f887-134">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="1f887-135">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="1f887-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="1f887-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f887-136">Response</span></span>

<span data-ttu-id="1f887-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и ресурс [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f887-137">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f887-138">Пример</span><span class="sxs-lookup"><span data-stu-id="1f887-138">Example</span></span>

<span data-ttu-id="1f887-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1f887-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1f887-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f887-140">Request</span></span>
<span data-ttu-id="1f887-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f887-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f887-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f887-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1f887-143">C#</span><span class="sxs-lookup"><span data-stu-id="1f887-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f887-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f887-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f887-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f887-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f887-146">Java</span><span class="sxs-lookup"><span data-stu-id="1f887-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-copy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1f887-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f887-147">Response</span></span>

<span data-ttu-id="1f887-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f887-148">Here is an example of the response.</span></span>

> <span data-ttu-id="1f887-149">**Примечание.**  Представленный здесь объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1f887-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1f887-150">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f887-150">All the properties will be returned from an actual call.</span></span>
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

