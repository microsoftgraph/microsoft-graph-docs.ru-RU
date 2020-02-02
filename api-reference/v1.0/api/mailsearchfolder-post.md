---
title: Создание Маилсеарчфолдер
description: Используйте этот API, чтобы создать новый Маилсеарчфолдер в почтовом ящике указанного пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3a4e24e41e4e8f8001d2350f0c0bf8959c5afabc
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2020
ms.locfileid: "41652195"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="1e131-103">Создание Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="1e131-103">Create mailSearchFolder</span></span>

<span data-ttu-id="1e131-104">Создайте новый [маилсеарчфолдер](../resources/mailsearchfolder.md) в почтовом ящике указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="1e131-104">Create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e131-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e131-105">Permissions</span></span>

<span data-ttu-id="1e131-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e131-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1e131-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e131-108">Permission type</span></span> | <span data-ttu-id="1e131-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e131-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="1e131-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e131-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e131-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e131-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1e131-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e131-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e131-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e131-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1e131-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e131-114">Application</span></span> | <span data-ttu-id="1e131-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e131-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e131-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e131-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="1e131-117">Укажите родительскую папку в URL-адресе запроса как идентификатор папки или известное имя папки.</span><span class="sxs-lookup"><span data-stu-id="1e131-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="1e131-118">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="1e131-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e131-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e131-119">Request headers</span></span>

| <span data-ttu-id="1e131-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e131-120">Header</span></span> | <span data-ttu-id="1e131-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1e131-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="1e131-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e131-122">Authorization</span></span> | <span data-ttu-id="1e131-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="1e131-123">`Bearer {token}`.</span></span> <span data-ttu-id="1e131-124">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="1e131-124">Required.</span></span> |
| <span data-ttu-id="1e131-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1e131-125">Content-Type</span></span> | <span data-ttu-id="1e131-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="1e131-126">`application/json`.</span></span> <span data-ttu-id="1e131-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="1e131-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e131-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e131-128">Request body</span></span>

<span data-ttu-id="1e131-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1e131-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1e131-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="1e131-130">Parameter</span></span> | <span data-ttu-id="1e131-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1e131-131">Type</span></span> | <span data-ttu-id="1e131-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1e131-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="1e131-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="1e131-133">@odata.type</span></span> | <span data-ttu-id="1e131-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1e131-134">String</span></span> | <span data-ttu-id="1e131-135">Тип создаваемой папки.</span><span class="sxs-lookup"><span data-stu-id="1e131-135">The type of folder to be created.</span></span> <span data-ttu-id="1e131-136">Задано значение "Microsoft. Graph. Маилсеарчфолдер".</span><span class="sxs-lookup"><span data-stu-id="1e131-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="1e131-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1e131-137">displayName</span></span> | <span data-ttu-id="1e131-138">Строка</span><span class="sxs-lookup"><span data-stu-id="1e131-138">String</span></span> | <span data-ttu-id="1e131-139">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="1e131-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="1e131-140">инклуденестедфолдерс</span><span class="sxs-lookup"><span data-stu-id="1e131-140">includeNestedFolders</span></span> | <span data-ttu-id="1e131-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e131-141">Boolean</span></span> | <span data-ttu-id="1e131-142">Указывает, как должна проходить иерархия папок почтовых ящиков в поиске.</span><span class="sxs-lookup"><span data-stu-id="1e131-142">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="1e131-143">`true`означает, что необходимо выполнить глубокий поиск, чтобы включить дочерние папки в иерархию каждой папки, явно указанной в **саурцефолдеридс**.</span><span class="sxs-lookup"><span data-stu-id="1e131-143">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="1e131-144">`false`означает неглубокий Поиск только тех папок, которые явно указаны в **саурцефолдеридс**.</span><span class="sxs-lookup"><span data-stu-id="1e131-144">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="1e131-145">саурцефолдеридс</span><span class="sxs-lookup"><span data-stu-id="1e131-145">sourceFolderIds</span></span> | <span data-ttu-id="1e131-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1e131-146">String collection</span></span> | <span data-ttu-id="1e131-147">Папки почтовых ящиков, которые должны быть mined.</span><span class="sxs-lookup"><span data-stu-id="1e131-147">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="1e131-148">филтеркуери</span><span class="sxs-lookup"><span data-stu-id="1e131-148">filterQuery</span></span> | <span data-ttu-id="1e131-149">Строка</span><span class="sxs-lookup"><span data-stu-id="1e131-149">String</span></span> | <span data-ttu-id="1e131-150">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="1e131-150">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="1e131-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e131-151">Response</span></span>

<span data-ttu-id="1e131-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [маилсеарчфолдер](../resources/mailsearchfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e131-152">If successful, this method returns a `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e131-153">Пример</span><span class="sxs-lookup"><span data-stu-id="1e131-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1e131-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e131-154">Request</span></span>

<span data-ttu-id="1e131-155">Ниже приведен пример запроса, который создает папку поиска для сообщений, содержащих строку "Еженедельная сводка" в теме.</span><span class="sxs-lookup"><span data-stu-id="1e131-155">The following is an example of the request - it creates a search folder of messages that contain the string "weekly digest" in the subject.</span></span> <span data-ttu-id="1e131-156">Папка поиска находится в той же папке, в которой применяется указанный запрос фильтра.</span><span class="sxs-lookup"><span data-stu-id="1e131-156">The search folder is under the same folder on which the specified filter query applies.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1e131-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e131-157">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1e131-158">C#</span><span class="sxs-lookup"><span data-stu-id="1e131-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e131-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e131-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1e131-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e131-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1e131-161">Java</span><span class="sxs-lookup"><span data-stu-id="1e131-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1e131-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e131-162">Response</span></span>

<span data-ttu-id="1e131-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1e131-163">The following is an example of the response.</span></span>

><span data-ttu-id="1e131-164">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1e131-164">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1e131-165">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e131-165">All the properties will be returned from an actual call.</span></span>
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
