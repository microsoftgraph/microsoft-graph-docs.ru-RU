---
title: Создание mailSearchFolder
description: Этот API используется для создания нового mailSearchFolder в почтовом ящике указанного пользователя.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 902e55bc3c1ab901f06591b379f636f72b04a782
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130664"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="90bb8-103">Создание mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="90bb8-103">Create mailSearchFolder</span></span>

<span data-ttu-id="90bb8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90bb8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90bb8-105">Создайте [новый mailSearchFolder](../resources/mailsearchfolder.md) в почтовом ящике указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="90bb8-105">Create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="90bb8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90bb8-106">Permissions</span></span>

<span data-ttu-id="90bb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90bb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90bb8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90bb8-109">Permission type</span></span> | <span data-ttu-id="90bb8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90bb8-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="90bb8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90bb8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="90bb8-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90bb8-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="90bb8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90bb8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90bb8-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90bb8-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="90bb8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90bb8-115">Application</span></span> | <span data-ttu-id="90bb8-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90bb8-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="90bb8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90bb8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="90bb8-118">Укажите родительская папка в URL-адресе запроса в качестве ИД папки или известного имени папки.</span><span class="sxs-lookup"><span data-stu-id="90bb8-118">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="90bb8-119">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="90bb8-119">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="90bb8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90bb8-120">Request headers</span></span>

| <span data-ttu-id="90bb8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90bb8-121">Header</span></span> | <span data-ttu-id="90bb8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="90bb8-122">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="90bb8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90bb8-123">Authorization</span></span> | <span data-ttu-id="90bb8-124">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="90bb8-124">`Bearer {token}`.</span></span> <span data-ttu-id="90bb8-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="90bb8-125">Required.</span></span> |
| <span data-ttu-id="90bb8-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="90bb8-126">Content-Type</span></span> | <span data-ttu-id="90bb8-127">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="90bb8-127">`application/json`.</span></span> <span data-ttu-id="90bb8-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="90bb8-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90bb8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90bb8-129">Request body</span></span>

<span data-ttu-id="90bb8-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="90bb8-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="90bb8-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="90bb8-131">Parameter</span></span> | <span data-ttu-id="90bb8-132">Тип</span><span class="sxs-lookup"><span data-stu-id="90bb8-132">Type</span></span> | <span data-ttu-id="90bb8-133">Описание</span><span class="sxs-lookup"><span data-stu-id="90bb8-133">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="90bb8-134">@odata.type</span><span class="sxs-lookup"><span data-stu-id="90bb8-134">@odata.type</span></span> | <span data-ttu-id="90bb8-135">String</span><span class="sxs-lookup"><span data-stu-id="90bb8-135">String</span></span> | <span data-ttu-id="90bb8-136">Тип создаемой папки.</span><span class="sxs-lookup"><span data-stu-id="90bb8-136">The type of folder to be created.</span></span> <span data-ttu-id="90bb8-137">Установите "microsoft.graph.mailSearchFolder".</span><span class="sxs-lookup"><span data-stu-id="90bb8-137">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="90bb8-138">displayName</span><span class="sxs-lookup"><span data-stu-id="90bb8-138">displayName</span></span> | <span data-ttu-id="90bb8-139">String</span><span class="sxs-lookup"><span data-stu-id="90bb8-139">String</span></span> | <span data-ttu-id="90bb8-140">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="90bb8-140">The display name of the new folder.</span></span>|
| <span data-ttu-id="90bb8-141">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="90bb8-141">includeNestedFolders</span></span> | <span data-ttu-id="90bb8-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="90bb8-142">Boolean</span></span> | <span data-ttu-id="90bb8-143">Указывает, как должна проходить иерархия папок почтового ящика в поиске.</span><span class="sxs-lookup"><span data-stu-id="90bb8-143">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="90bb8-144">`true`означает, что следует глубоко искать, чтобы включить в иерархию каждой папки, явно указанной в **sourceFolderIds.**</span><span class="sxs-lookup"><span data-stu-id="90bb8-144">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="90bb8-145">`false`означает неглубокий поиск только каждой папки, явно указанной в **sourceFolderIds.**</span><span class="sxs-lookup"><span data-stu-id="90bb8-145">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="90bb8-146">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="90bb8-146">sourceFolderIds</span></span> | <span data-ttu-id="90bb8-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="90bb8-147">String collection</span></span> | <span data-ttu-id="90bb8-148">Папки почтового ящика, которые необходимо миновать.</span><span class="sxs-lookup"><span data-stu-id="90bb8-148">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="90bb8-149">filterQuery</span><span class="sxs-lookup"><span data-stu-id="90bb8-149">filterQuery</span></span> | <span data-ttu-id="90bb8-150">String</span><span class="sxs-lookup"><span data-stu-id="90bb8-150">String</span></span> | <span data-ttu-id="90bb8-151">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="90bb8-151">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="90bb8-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="90bb8-152">Response</span></span>

<span data-ttu-id="90bb8-153">В случае успеха этот метод возвращает код отклика и объект `201 Created` [mailSearchFolder](../resources/mailsearchfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90bb8-153">If successful, this method returns a `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90bb8-154">Пример</span><span class="sxs-lookup"><span data-stu-id="90bb8-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="90bb8-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="90bb8-155">Request</span></span>

<span data-ttu-id="90bb8-156">Ниже приводится пример запроса— он создает папку поиска сообщений, содержащих строку "weekly digest" в теме.</span><span class="sxs-lookup"><span data-stu-id="90bb8-156">The following is an example of the request - it creates a search folder of messages that contain the string "weekly digest" in the subject.</span></span> <span data-ttu-id="90bb8-157">Папка поиска находится в той же папке, к которой применяется указанный запрос фильтра.</span><span class="sxs-lookup"><span data-stu-id="90bb8-157">The search folder is under the same folder on which the specified filter query applies.</span></span>

# <a name="http"></a>[<span data-ttu-id="90bb8-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="90bb8-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADYAAAIBDAAAAA=="],
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders
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
# <a name="c"></a>[<span data-ttu-id="90bb8-159">C#</span><span class="sxs-lookup"><span data-stu-id="90bb8-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90bb8-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90bb8-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90bb8-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90bb8-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90bb8-162">Java</span><span class="sxs-lookup"><span data-stu-id="90bb8-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="90bb8-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="90bb8-163">Response</span></span>

<span data-ttu-id="90bb8-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90bb8-164">The following is an example of the response.</span></span>

><span data-ttu-id="90bb8-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90bb8-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders('AQMkADYAAAIBDAAAAA%3D%3D')/childFolders/$entity",
    "@odata.type": "#microsoft.graph.mailSearchFolder",
    "id": "AAMkADYfRAAAZg1yTAAA=",
    "displayName": "Weekly digests",
    "parentFolderId": "AQMkADYAAAIBDAAAAA==",
    "childFolderCount": 0,
    "unreadItemCount": 0,
    "totalItemCount": 0,
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

