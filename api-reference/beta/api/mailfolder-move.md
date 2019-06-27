---
title: 'mailFolder: move'
description: Перемещение папки почты со всем ее содержимым в другую папку почты.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2d7f35549bba93cae00b6f3a184d453271b01451
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266643"
---
# <a name="mailfolder-move"></a><span data-ttu-id="faf0c-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="faf0c-103">mailFolder: move</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="faf0c-104">Перемещение папки почты со всем ее содержимым в другую папку почты.</span><span class="sxs-lookup"><span data-stu-id="faf0c-104">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="faf0c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="faf0c-105">Permissions</span></span>

<span data-ttu-id="faf0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faf0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="faf0c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="faf0c-108">Permission type</span></span> | <span data-ttu-id="faf0c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="faf0c-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="faf0c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="faf0c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="faf0c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="faf0c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="faf0c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="faf0c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="faf0c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="faf0c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="faf0c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="faf0c-114">Application</span></span> | <span data-ttu-id="faf0c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="faf0c-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="faf0c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="faf0c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="faf0c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="faf0c-117">Request headers</span></span>

| <span data-ttu-id="faf0c-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="faf0c-118">Header</span></span> | <span data-ttu-id="faf0c-119">Значение</span><span class="sxs-lookup"><span data-stu-id="faf0c-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="faf0c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="faf0c-120">Authorization</span></span> | <span data-ttu-id="faf0c-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="faf0c-121"></span></span> <span data-ttu-id="faf0c-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="faf0c-122">Required.</span></span> |
| <span data-ttu-id="faf0c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="faf0c-123">Content-Type</span></span> | <span data-ttu-id="faf0c-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="faf0c-124"></span></span> <span data-ttu-id="faf0c-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="faf0c-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="faf0c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="faf0c-126">Request body</span></span>

<span data-ttu-id="faf0c-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="faf0c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="faf0c-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="faf0c-128">Parameter</span></span> | <span data-ttu-id="faf0c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="faf0c-129">Type</span></span> | <span data-ttu-id="faf0c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="faf0c-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="faf0c-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="faf0c-131">destinationId</span></span>|<span data-ttu-id="faf0c-132">String</span><span class="sxs-lookup"><span data-stu-id="faf0c-132">String</span></span>|<span data-ttu-id="faf0c-133">Идентификатор папки или имя известной папки.</span><span class="sxs-lookup"><span data-stu-id="faf0c-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="faf0c-134">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="faf0c-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="faf0c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="faf0c-135">Response</span></span>

<span data-ttu-id="faf0c-136">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="faf0c-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faf0c-137">Пример</span><span class="sxs-lookup"><span data-stu-id="faf0c-137">Example</span></span>

<span data-ttu-id="faf0c-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="faf0c-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="faf0c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="faf0c-139">Request</span></span>

<span data-ttu-id="faf0c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="faf0c-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="faf0c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="faf0c-141">Response</span></span>

<span data-ttu-id="faf0c-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="faf0c-142">Here is an example of the response.</span></span>

> <span data-ttu-id="faf0c-143">**Примечание.**  Представленный здесь объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="faf0c-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="faf0c-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="faf0c-144">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="faf0c-145">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="faf0c-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="faf0c-146">C#</span><span class="sxs-lookup"><span data-stu-id="faf0c-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/mailfolder_move-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="faf0c-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="faf0c-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/mailfolder_move-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="faf0c-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="faf0c-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/mailfolder_move-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/mailfolder-move.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-move.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-move.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
