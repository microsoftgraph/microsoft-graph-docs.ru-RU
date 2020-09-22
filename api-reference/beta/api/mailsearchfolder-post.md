---
title: Создание Маилсеарчфолдер
description: Используйте этот API, чтобы создать новый Маилсеарчфолдер в почтовом ящике указанного пользователя.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ffa9f15cfabc5811a42bb17aea818b101e0a9f71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027715"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="f671e-103">Создание Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="f671e-103">Create mailSearchFolder</span></span>

<span data-ttu-id="f671e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f671e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f671e-105">Создайте новый [маилсеарчфолдер](../resources/mailsearchfolder.md) в почтовом ящике указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f671e-105">Create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="f671e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f671e-106">Permissions</span></span>

<span data-ttu-id="f671e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f671e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f671e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f671e-109">Permission type</span></span> | <span data-ttu-id="f671e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f671e-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="f671e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f671e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f671e-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f671e-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f671e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f671e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f671e-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f671e-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f671e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f671e-115">Application</span></span> | <span data-ttu-id="f671e-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f671e-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f671e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f671e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="f671e-118">Укажите родительскую папку в URL-адресе запроса как идентификатор папки или известное имя папки.</span><span class="sxs-lookup"><span data-stu-id="f671e-118">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="f671e-119">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="f671e-119">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f671e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f671e-120">Request headers</span></span>

| <span data-ttu-id="f671e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f671e-121">Header</span></span> | <span data-ttu-id="f671e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f671e-122">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="f671e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f671e-123">Authorization</span></span> | <span data-ttu-id="f671e-124">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="f671e-124">`Bearer {token}`.</span></span> <span data-ttu-id="f671e-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f671e-125">Required.</span></span> |
| <span data-ttu-id="f671e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f671e-126">Content-Type</span></span> | <span data-ttu-id="f671e-127">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="f671e-127">`application/json`.</span></span> <span data-ttu-id="f671e-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f671e-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f671e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f671e-129">Request body</span></span>

<span data-ttu-id="f671e-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f671e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f671e-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="f671e-131">Parameter</span></span> | <span data-ttu-id="f671e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f671e-132">Type</span></span> | <span data-ttu-id="f671e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f671e-133">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="f671e-134">@odata.type</span><span class="sxs-lookup"><span data-stu-id="f671e-134">@odata.type</span></span> | <span data-ttu-id="f671e-135">String</span><span class="sxs-lookup"><span data-stu-id="f671e-135">String</span></span> | <span data-ttu-id="f671e-136">Тип создаваемой папки.</span><span class="sxs-lookup"><span data-stu-id="f671e-136">The type of folder to be created.</span></span> <span data-ttu-id="f671e-137">Задано значение "Microsoft. Graph. Маилсеарчфолдер".</span><span class="sxs-lookup"><span data-stu-id="f671e-137">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="f671e-138">displayName</span><span class="sxs-lookup"><span data-stu-id="f671e-138">displayName</span></span> | <span data-ttu-id="f671e-139">String</span><span class="sxs-lookup"><span data-stu-id="f671e-139">String</span></span> | <span data-ttu-id="f671e-140">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="f671e-140">The display name of the new folder.</span></span>|
| <span data-ttu-id="f671e-141">инклуденестедфолдерс</span><span class="sxs-lookup"><span data-stu-id="f671e-141">includeNestedFolders</span></span> | <span data-ttu-id="f671e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f671e-142">Boolean</span></span> | <span data-ttu-id="f671e-143">Указывает, как должна проходить иерархия папок почтовых ящиков в поиске.</span><span class="sxs-lookup"><span data-stu-id="f671e-143">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="f671e-144">`true` означает, что необходимо выполнить глубокий поиск, чтобы включить дочерние папки в иерархию каждой папки, явно указанной в **саурцефолдеридс**.</span><span class="sxs-lookup"><span data-stu-id="f671e-144">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="f671e-145">`false` означает неглубокий Поиск только тех папок, которые явно указаны в **саурцефолдеридс**.</span><span class="sxs-lookup"><span data-stu-id="f671e-145">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="f671e-146">саурцефолдеридс</span><span class="sxs-lookup"><span data-stu-id="f671e-146">sourceFolderIds</span></span> | <span data-ttu-id="f671e-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f671e-147">String collection</span></span> | <span data-ttu-id="f671e-148">Папки почтовых ящиков, которые должны быть mined.</span><span class="sxs-lookup"><span data-stu-id="f671e-148">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="f671e-149">филтеркуери</span><span class="sxs-lookup"><span data-stu-id="f671e-149">filterQuery</span></span> | <span data-ttu-id="f671e-150">String</span><span class="sxs-lookup"><span data-stu-id="f671e-150">String</span></span> | <span data-ttu-id="f671e-151">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="f671e-151">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="f671e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="f671e-152">Response</span></span>

<span data-ttu-id="f671e-153">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [маилсеарчфолдер](../resources/mailsearchfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f671e-153">If successful, this method returns a `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f671e-154">Пример</span><span class="sxs-lookup"><span data-stu-id="f671e-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f671e-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="f671e-155">Request</span></span>

<span data-ttu-id="f671e-156">Ниже приведен пример запроса, который создает папку поиска для сообщений, содержащих строку "Еженедельная сводка" в теме.</span><span class="sxs-lookup"><span data-stu-id="f671e-156">The following is an example of the request - it creates a search folder of messages that contain the string "weekly digest" in the subject.</span></span> <span data-ttu-id="f671e-157">Папка поиска находится в той же папке, в которой применяется указанный запрос фильтра.</span><span class="sxs-lookup"><span data-stu-id="f671e-157">The search folder is under the same folder on which the specified filter query applies.</span></span>

# <a name="http"></a>[<span data-ttu-id="f671e-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="f671e-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f671e-159">C#</span><span class="sxs-lookup"><span data-stu-id="f671e-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f671e-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f671e-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f671e-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f671e-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f671e-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="f671e-162">Response</span></span>

<span data-ttu-id="f671e-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f671e-163">The following is an example of the response.</span></span>

><span data-ttu-id="f671e-164">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f671e-164">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f671e-165">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f671e-165">All the properties will be returned from an actual call.</span></span>
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


