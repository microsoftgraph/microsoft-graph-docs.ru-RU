---
title: Создание объекта mailFolder
description: Используйте этот API для создания нового почтового ящика для детей.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8d79b9817332c7aea773ad9062efd3a4718dd197
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049256"
---
# <a name="create-mailfolder"></a><span data-ttu-id="d3757-103">Создание объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="d3757-103">Create mailFolder</span></span>

<span data-ttu-id="d3757-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3757-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3757-105">Используйте этот API для создания нового [почтового ящика для детей.](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="d3757-105">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d3757-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3757-106">Permissions</span></span>

<span data-ttu-id="d3757-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3757-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3757-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3757-109">Permission type</span></span> | <span data-ttu-id="d3757-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3757-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="d3757-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3757-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d3757-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3757-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d3757-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3757-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3757-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3757-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d3757-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3757-115">Application</span></span> | <span data-ttu-id="d3757-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3757-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3757-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3757-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="d3757-118">Укажите родительную папку в URL-адресе запроса в качестве ИД папки или имени известной папки.</span><span class="sxs-lookup"><span data-stu-id="d3757-118">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="d3757-119">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="d3757-119">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3757-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3757-120">Request headers</span></span>

| <span data-ttu-id="d3757-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3757-121">Header</span></span> | <span data-ttu-id="d3757-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d3757-122">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="d3757-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3757-123">Authorization</span></span> | <span data-ttu-id="d3757-124">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="d3757-124">`Bearer {token}`.</span></span> <span data-ttu-id="d3757-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d3757-125">Required.</span></span> |
| <span data-ttu-id="d3757-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3757-126">Content-Type</span></span> | <span data-ttu-id="d3757-127">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="d3757-127">`application/json`.</span></span> <span data-ttu-id="d3757-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d3757-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3757-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3757-129">Request body</span></span>

<span data-ttu-id="d3757-p105">Предоставьте в тексте запроса объект JSON с указанными ниже параметрами. **displayName** — это единственное доступное для записи свойство объекта [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="d3757-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="d3757-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="d3757-132">Parameter</span></span> | <span data-ttu-id="d3757-133">Тип</span><span class="sxs-lookup"><span data-stu-id="d3757-133">Type</span></span> | <span data-ttu-id="d3757-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d3757-134">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="d3757-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d3757-135">displayName</span></span>|<span data-ttu-id="d3757-136">String</span><span class="sxs-lookup"><span data-stu-id="d3757-136">String</span></span>|<span data-ttu-id="d3757-137">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="d3757-137">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="d3757-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="d3757-138">Response</span></span>

<span data-ttu-id="d3757-139">В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [mailFolder](../resources/mailfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d3757-139">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3757-140">Пример</span><span class="sxs-lookup"><span data-stu-id="d3757-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d3757-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3757-141">Request</span></span>

<span data-ttu-id="d3757-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3757-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3757-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3757-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d3757-144">C#</span><span class="sxs-lookup"><span data-stu-id="d3757-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3757-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3757-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3757-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3757-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3757-147">Java</span><span class="sxs-lookup"><span data-stu-id="d3757-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d3757-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3757-148">Response</span></span>

<span data-ttu-id="d3757-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d3757-149">The following is an example of the response.</span></span>

> <span data-ttu-id="d3757-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d3757-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Create mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


