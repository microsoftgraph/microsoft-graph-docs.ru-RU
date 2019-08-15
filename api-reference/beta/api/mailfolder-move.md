---
title: 'mailFolder: move'
description: Перемещение папки почты со всем ее содержимым в другую папку почты.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 16d855afbce2e23a1d1fee9a9d9af3a4ac516775
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415255"
---
# <a name="mailfolder-move"></a><span data-ttu-id="b8459-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="b8459-103">mailFolder: move</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8459-104">Перемещение папки почты со всем ее содержимым в другую папку почты.</span><span class="sxs-lookup"><span data-stu-id="b8459-104">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8459-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8459-105">Permissions</span></span>

<span data-ttu-id="b8459-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8459-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8459-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8459-108">Permission type</span></span> | <span data-ttu-id="b8459-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8459-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="b8459-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8459-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b8459-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8459-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b8459-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8459-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8459-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8459-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b8459-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8459-114">Application</span></span> | <span data-ttu-id="b8459-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8459-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8459-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8459-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="b8459-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8459-117">Request headers</span></span>

| <span data-ttu-id="b8459-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8459-118">Header</span></span> | <span data-ttu-id="b8459-119">Значение</span><span class="sxs-lookup"><span data-stu-id="b8459-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="b8459-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8459-120">Authorization</span></span> | <span data-ttu-id="b8459-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="b8459-121"></span></span> <span data-ttu-id="b8459-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b8459-122">Required.</span></span> |
| <span data-ttu-id="b8459-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8459-123">Content-Type</span></span> | <span data-ttu-id="b8459-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="b8459-124"></span></span> <span data-ttu-id="b8459-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b8459-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8459-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8459-126">Request body</span></span>

<span data-ttu-id="b8459-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b8459-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b8459-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="b8459-128">Parameter</span></span> | <span data-ttu-id="b8459-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b8459-129">Type</span></span> | <span data-ttu-id="b8459-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b8459-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="b8459-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="b8459-131">destinationId</span></span>|<span data-ttu-id="b8459-132">String</span><span class="sxs-lookup"><span data-stu-id="b8459-132">String</span></span>|<span data-ttu-id="b8459-133">Идентификатор папки или имя известной папки.</span><span class="sxs-lookup"><span data-stu-id="b8459-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="b8459-134">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="b8459-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="b8459-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8459-135">Response</span></span>

<span data-ttu-id="b8459-136">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b8459-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8459-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b8459-137">Example</span></span>

<span data-ttu-id="b8459-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b8459-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b8459-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8459-139">Request</span></span>

<span data-ttu-id="b8459-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8459-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b8459-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8459-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8459-142">C#</span><span class="sxs-lookup"><span data-stu-id="b8459-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-move-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8459-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8459-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-move-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8459-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b8459-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-move-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b8459-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8459-145">Response</span></span>

<span data-ttu-id="b8459-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b8459-146">Here is an example of the response.</span></span>

> <span data-ttu-id="b8459-147">**Примечание.**  Представленный здесь объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b8459-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b8459-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8459-148">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
