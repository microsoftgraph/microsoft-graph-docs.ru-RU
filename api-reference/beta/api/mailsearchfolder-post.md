---
title: Создание mailSearchFolder
description: Используйте этот API для создания нового mailSearchFolder в указанном почтовом ящике пользователя.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9899276551b09c7e4a4da6e6b92f046d594d5ad5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051146"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="3a8d4-103">Создание mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="3a8d4-103">Create mailSearchFolder</span></span>

<span data-ttu-id="3a8d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a8d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a8d4-105">Создайте [новую mailSearchFolder](../resources/mailsearchfolder.md) в указанном почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-105">Create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a8d4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a8d4-106">Permissions</span></span>

<span data-ttu-id="3a8d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a8d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a8d4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a8d4-109">Permission type</span></span> | <span data-ttu-id="3a8d4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a8d4-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="3a8d4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a8d4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3a8d4-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a8d4-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3a8d4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a8d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a8d4-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a8d4-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3a8d4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a8d4-115">Application</span></span> | <span data-ttu-id="3a8d4-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a8d4-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a8d4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a8d4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="3a8d4-118">Укажите родительную папку в URL-адресе запроса в качестве ИД папки или имени известной папки.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-118">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="3a8d4-119">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="3a8d4-119">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a8d4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a8d4-120">Request headers</span></span>

| <span data-ttu-id="3a8d4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a8d4-121">Header</span></span> | <span data-ttu-id="3a8d4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a8d4-122">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="3a8d4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a8d4-123">Authorization</span></span> | <span data-ttu-id="3a8d4-124">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-124">`Bearer {token}`.</span></span> <span data-ttu-id="3a8d4-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-125">Required.</span></span> |
| <span data-ttu-id="3a8d4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a8d4-126">Content-Type</span></span> | <span data-ttu-id="3a8d4-127">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-127">`application/json`.</span></span> <span data-ttu-id="3a8d4-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a8d4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a8d4-129">Request body</span></span>

<span data-ttu-id="3a8d4-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3a8d4-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="3a8d4-131">Parameter</span></span> | <span data-ttu-id="3a8d4-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3a8d4-132">Type</span></span> | <span data-ttu-id="3a8d4-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3a8d4-133">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="3a8d4-134">@odata.type</span><span class="sxs-lookup"><span data-stu-id="3a8d4-134">@odata.type</span></span> | <span data-ttu-id="3a8d4-135">String</span><span class="sxs-lookup"><span data-stu-id="3a8d4-135">String</span></span> | <span data-ttu-id="3a8d4-136">Тип создаемой папки.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-136">The type of folder to be created.</span></span> <span data-ttu-id="3a8d4-137">Установите "microsoft.graph.mailSearchFolder".</span><span class="sxs-lookup"><span data-stu-id="3a8d4-137">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="3a8d4-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3a8d4-138">displayName</span></span> | <span data-ttu-id="3a8d4-139">String</span><span class="sxs-lookup"><span data-stu-id="3a8d4-139">String</span></span> | <span data-ttu-id="3a8d4-140">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-140">The display name of the new folder.</span></span>|
| <span data-ttu-id="3a8d4-141">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="3a8d4-141">includeNestedFolders</span></span> | <span data-ttu-id="3a8d4-142">Логический</span><span class="sxs-lookup"><span data-stu-id="3a8d4-142">Boolean</span></span> | <span data-ttu-id="3a8d4-143">Указывает, как должна проходить иерархия папок почтовых ящиков в поиске.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-143">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="3a8d4-144">`true` означает, что следует сделать глубокий поиск, чтобы включить детские папки в иерархию каждой папки, явно указанной в **sourceFolderIds**.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-144">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="3a8d4-145">`false`означает неглубокий поиск только каждой из папок, явно указанных в **sourceFolderIds.**</span><span class="sxs-lookup"><span data-stu-id="3a8d4-145">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="3a8d4-146">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="3a8d4-146">sourceFolderIds</span></span> | <span data-ttu-id="3a8d4-147">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="3a8d4-147">String collection</span></span> | <span data-ttu-id="3a8d4-148">Папки почтовых ящиков, которые необходимо добыть.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-148">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="3a8d4-149">filterQuery</span><span class="sxs-lookup"><span data-stu-id="3a8d4-149">filterQuery</span></span> | <span data-ttu-id="3a8d4-150">String</span><span class="sxs-lookup"><span data-stu-id="3a8d4-150">String</span></span> | <span data-ttu-id="3a8d4-151">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-151">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="3a8d4-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a8d4-152">Response</span></span>

<span data-ttu-id="3a8d4-153">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект mailSearchFolder](../resources/mailsearchfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-153">If successful, this method returns a `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a8d4-154">Пример</span><span class="sxs-lookup"><span data-stu-id="3a8d4-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3a8d4-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a8d4-155">Request</span></span>

<span data-ttu-id="3a8d4-156">Ниже приводится пример запроса — он создает папку поиска сообщений, содержащих строку "еженедельный дайджест" в субъекте.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-156">The following is an example of the request - it creates a search folder of messages that contain the string "weekly digest" in the subject.</span></span> <span data-ttu-id="3a8d4-157">Папка поиска находится в той же папке, в которой применяется указанный запрос фильтра.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-157">The search folder is under the same folder on which the specified filter query applies.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a8d4-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a8d4-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADYAAAIBDAAAAA=="],
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Weekly digests",
  "includeNestedFolders": true,
  "sourceFolderIds": ["AQMkADYAAAIBDAAAAA=="],
  "filterQuery": "contains(subject, 'weekly digest')"
}
```
# <a name="c"></a>[<span data-ttu-id="3a8d4-159">C#</span><span class="sxs-lookup"><span data-stu-id="3a8d4-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a8d4-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a8d4-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a8d4-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a8d4-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a8d4-162">Java</span><span class="sxs-lookup"><span data-stu-id="3a8d4-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3a8d4-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a8d4-163">Response</span></span>

<span data-ttu-id="3a8d4-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-164">The following is an example of the response.</span></span>

><span data-ttu-id="3a8d4-165">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3a8d4-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders('AQMkADYAAAIBDAAAAA%3D%3D')/childFolders/$entity",
    "@odata.type": "#microsoft.graph.mailSearchFolder",
    "id": "AAMkADYfRAAAZg1yTAAA=",
    "displayName": "Weekly digests",
    "parentFolderId": "AQMkADYAAAIBDAAAAA==",
    "childFolderCount": 0,
    "unreadItemCount": 0,
    "totalItemCount": 0,
    "wellKnownName": null,
    "isSupported": true,
    "includeNestedFolders": true,
    "sourceFolderIds": [
        "AQMkADYAAAIBDAAAAA=="
    ],
    "filterQuery": "contains(subject, 'weekly digest')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


