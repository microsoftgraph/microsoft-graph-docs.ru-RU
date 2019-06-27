---
title: Создание объекта MailFolder
description: Используйте этот API для создания нового дочернего элемента mailFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f181f2716aa56dc9d27f0dbc2259157a0d04b28f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266649"
---
# <a name="create-mailfolder"></a><span data-ttu-id="dcf06-103">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="dcf06-103">Create mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcf06-104">Используйте этот API для создания нового дочернего элемента [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="dcf06-104">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcf06-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dcf06-105">Permissions</span></span>

<span data-ttu-id="dcf06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcf06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcf06-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcf06-108">Permission type</span></span> | <span data-ttu-id="dcf06-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcf06-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="dcf06-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcf06-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dcf06-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcf06-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dcf06-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcf06-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcf06-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcf06-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dcf06-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dcf06-114">Application</span></span> | <span data-ttu-id="dcf06-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcf06-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcf06-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcf06-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="dcf06-117">Укажите родительскую папку в URL-адресе запроса как идентификатор папки или известное имя папки.</span><span class="sxs-lookup"><span data-stu-id="dcf06-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="dcf06-118">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="dcf06-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcf06-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dcf06-119">Request headers</span></span>

| <span data-ttu-id="dcf06-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dcf06-120">Header</span></span> | <span data-ttu-id="dcf06-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dcf06-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="dcf06-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dcf06-122">Authorization</span></span> | <span data-ttu-id="dcf06-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="dcf06-123"></span></span> <span data-ttu-id="dcf06-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dcf06-124">Required.</span></span> |
| <span data-ttu-id="dcf06-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dcf06-125">Content-Type</span></span> | <span data-ttu-id="dcf06-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="dcf06-126"></span></span> <span data-ttu-id="dcf06-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dcf06-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcf06-128">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="dcf06-128">Request body</span></span>

<span data-ttu-id="dcf06-p105">Предоставьте в тексте запроса объект JSON с указанными ниже параметрами. **displayName** — это единственное доступное для записи свойство объекта [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="dcf06-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="dcf06-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="dcf06-131">Parameter</span></span> | <span data-ttu-id="dcf06-132">Тип</span><span class="sxs-lookup"><span data-stu-id="dcf06-132">Type</span></span> | <span data-ttu-id="dcf06-133">Описание</span><span class="sxs-lookup"><span data-stu-id="dcf06-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="dcf06-134">displayName</span><span class="sxs-lookup"><span data-stu-id="dcf06-134">displayName</span></span>|<span data-ttu-id="dcf06-135">String</span><span class="sxs-lookup"><span data-stu-id="dcf06-135">String</span></span>|<span data-ttu-id="dcf06-136">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="dcf06-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="dcf06-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="dcf06-137">Response</span></span>

<span data-ttu-id="dcf06-138">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dcf06-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcf06-139">Пример</span><span class="sxs-lookup"><span data-stu-id="dcf06-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dcf06-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcf06-140">Request</span></span>

<span data-ttu-id="dcf06-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcf06-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

#### <a name="response"></a><span data-ttu-id="dcf06-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcf06-142">Response</span></span>

<span data-ttu-id="dcf06-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dcf06-143">The following is an example of the response.</span></span>

> <span data-ttu-id="dcf06-144">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dcf06-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dcf06-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dcf06-145">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="dcf06-146">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="dcf06-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dcf06-147">C#</span><span class="sxs-lookup"><span data-stu-id="dcf06-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcf06-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="dcf06-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_mailfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dcf06-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dcf06-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_mailfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-post-childfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-post-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-post-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
