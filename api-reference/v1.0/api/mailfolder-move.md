---
title: 'mailFolder: move'
description: Перемещение папки почты со всем ее содержимым в другую папку почты.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 743153a623dcd4768f32e450643ba95eb4fea7c5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467339"
---
# <a name="mailfolder-move"></a><span data-ttu-id="7dda7-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="7dda7-103">mailFolder: move</span></span>

<span data-ttu-id="7dda7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dda7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7dda7-105">Перемещение папки почты со всем ее содержимым в другую папку почты.</span><span class="sxs-lookup"><span data-stu-id="7dda7-105">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dda7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7dda7-106">Permissions</span></span>

<span data-ttu-id="7dda7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dda7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7dda7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7dda7-109">Permission type</span></span> | <span data-ttu-id="7dda7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7dda7-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="7dda7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7dda7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7dda7-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7dda7-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7dda7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7dda7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dda7-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7dda7-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7dda7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7dda7-115">Application</span></span> | <span data-ttu-id="7dda7-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7dda7-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dda7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7dda7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="7dda7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7dda7-118">Request headers</span></span>

| <span data-ttu-id="7dda7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7dda7-119">Header</span></span> | <span data-ttu-id="7dda7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7dda7-120">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="7dda7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7dda7-121">Authorization</span></span> | <span data-ttu-id="7dda7-122">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="7dda7-122">`Bearer {token}`.</span></span> <span data-ttu-id="7dda7-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7dda7-123">Required.</span></span> |
| <span data-ttu-id="7dda7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7dda7-124">Content-Type</span></span> | <span data-ttu-id="7dda7-125">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="7dda7-125">`application/json`.</span></span> <span data-ttu-id="7dda7-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7dda7-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dda7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7dda7-127">Request body</span></span>

<span data-ttu-id="7dda7-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7dda7-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7dda7-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="7dda7-129">Parameter</span></span> | <span data-ttu-id="7dda7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7dda7-130">Type</span></span> | <span data-ttu-id="7dda7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7dda7-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="7dda7-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="7dda7-132">destinationId</span></span>|<span data-ttu-id="7dda7-133">String</span><span class="sxs-lookup"><span data-stu-id="7dda7-133">String</span></span>|<span data-ttu-id="7dda7-134">Идентификатор папки или имя известной папки.</span><span class="sxs-lookup"><span data-stu-id="7dda7-134">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="7dda7-135">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="7dda7-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="7dda7-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7dda7-136">Response</span></span>

<span data-ttu-id="7dda7-137">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и ресурс [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7dda7-137">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dda7-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7dda7-138">Example</span></span>

<span data-ttu-id="7dda7-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7dda7-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7dda7-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dda7-140">Request</span></span>

<span data-ttu-id="7dda7-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dda7-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7dda7-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dda7-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="7dda7-143">C#</span><span class="sxs-lookup"><span data-stu-id="7dda7-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-move-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dda7-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dda7-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-move-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dda7-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dda7-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-move-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7dda7-146">Java</span><span class="sxs-lookup"><span data-stu-id="7dda7-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-move-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7dda7-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dda7-147">Response</span></span>

<span data-ttu-id="7dda7-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dda7-148">Here is an example of the response.</span></span>

> <span data-ttu-id="7dda7-149">**Примечание.**  Представленный здесь объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7dda7-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7dda7-150">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dda7-150">All the properties will be returned from an actual call.</span></span>
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
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
