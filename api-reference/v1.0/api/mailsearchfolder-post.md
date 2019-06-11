---
title: Создание Маилсеарчфолдер
description: Используйте этот API, чтобы создать новый Маилсеарчфолдер в почтовом ящике указанного пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 55cd832b5fb6a90e919890fb05553384e58807db
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2019
ms.locfileid: "34818687"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="d3622-103">Создание Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="d3622-103">Create mailSearchFolder</span></span>

<span data-ttu-id="d3622-104">Создайте новый [маилсеарчфолдер](../resources/mailsearchfolder.md) в почтовом ящике указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3622-104">Create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3622-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3622-105">Permissions</span></span>

<span data-ttu-id="d3622-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3622-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3622-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3622-108">Permission type</span></span> | <span data-ttu-id="d3622-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3622-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="d3622-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3622-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d3622-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3622-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d3622-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3622-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3622-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3622-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d3622-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3622-114">Application</span></span> | <span data-ttu-id="d3622-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3622-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3622-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3622-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="d3622-117">Укажите родительскую папку в URL-адресе запроса как идентификатор папки или известное имя папки.</span><span class="sxs-lookup"><span data-stu-id="d3622-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="d3622-118">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="d3622-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3622-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3622-119">Request headers</span></span>

| <span data-ttu-id="d3622-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3622-120">Header</span></span> | <span data-ttu-id="d3622-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d3622-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="d3622-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3622-122">Authorization</span></span> | <span data-ttu-id="d3622-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="d3622-123"></span></span> <span data-ttu-id="d3622-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d3622-124">Required.</span></span> |
| <span data-ttu-id="d3622-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3622-125">Content-Type</span></span> | <span data-ttu-id="d3622-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="d3622-126"></span></span> <span data-ttu-id="d3622-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d3622-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3622-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3622-128">Request body</span></span>

<span data-ttu-id="d3622-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d3622-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d3622-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="d3622-130">Parameter</span></span> | <span data-ttu-id="d3622-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d3622-131">Type</span></span> | <span data-ttu-id="d3622-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d3622-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="d3622-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="d3622-133">@odata.type</span></span> | <span data-ttu-id="d3622-134">String</span><span class="sxs-lookup"><span data-stu-id="d3622-134">String</span></span> | <span data-ttu-id="d3622-135">Тип создаваемой папки.</span><span class="sxs-lookup"><span data-stu-id="d3622-135">The type of folder to be created.</span></span> <span data-ttu-id="d3622-136">Задано значение "Microsoft. Graph. Маилсеарчфолдер".</span><span class="sxs-lookup"><span data-stu-id="d3622-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="d3622-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d3622-137">displayName</span></span> | <span data-ttu-id="d3622-138">String</span><span class="sxs-lookup"><span data-stu-id="d3622-138">String</span></span> | <span data-ttu-id="d3622-139">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="d3622-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="d3622-140">Инклуденестедфолдерс</span><span class="sxs-lookup"><span data-stu-id="d3622-140">includeNestedFolders</span></span> | <span data-ttu-id="d3622-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3622-141">Boolean</span></span> | <span data-ttu-id="d3622-142">Указывает, как должна проходить иерархия папок почтовых ящиков в поиске.</span><span class="sxs-lookup"><span data-stu-id="d3622-142">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="d3622-143">`true`означает, что необходимо выполнить глубокий поиск, чтобы включить дочерние папки в иерархию каждой папки, явно указанной в **саурцефолдеридс**.</span><span class="sxs-lookup"><span data-stu-id="d3622-143">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="d3622-144">`false`означает неглубокий Поиск только тех папок, которые явно указаны в **саурцефолдеридс**.</span><span class="sxs-lookup"><span data-stu-id="d3622-144">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="d3622-145">Саурцефолдеридс</span><span class="sxs-lookup"><span data-stu-id="d3622-145">sourceFolderIds</span></span> | <span data-ttu-id="d3622-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d3622-146">String collection</span></span> | <span data-ttu-id="d3622-147">Папки почтовых ящиков, которые должны быть mined.</span><span class="sxs-lookup"><span data-stu-id="d3622-147">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="d3622-148">Филтеркуери</span><span class="sxs-lookup"><span data-stu-id="d3622-148">filterQuery</span></span> | <span data-ttu-id="d3622-149">String</span><span class="sxs-lookup"><span data-stu-id="d3622-149">String</span></span> | <span data-ttu-id="d3622-150">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="d3622-150">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="d3622-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3622-151">Response</span></span>

<span data-ttu-id="d3622-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [маилсеарчфолдер](../resources/mailsearchfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3622-152">If successful, this method returns a `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3622-153">Пример</span><span class="sxs-lookup"><span data-stu-id="d3622-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d3622-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3622-154">Request</span></span>

<span data-ttu-id="d3622-155">Ниже приведен пример запроса, который создает папку поиска для сообщений, содержащих строку "Еженедельная сводка" в теме.</span><span class="sxs-lookup"><span data-stu-id="d3622-155">The following is an example of the request - it creates a search folder of messages that contain the string "weekly digest" in the subject.</span></span> <span data-ttu-id="d3622-156">Папка поиска находится в той же папке, в которой применяется указанный запрос фильтра.</span><span class="sxs-lookup"><span data-stu-id="d3622-156">The search folder is under the same folder on which the specified filter query applies.</span></span>
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

#### <a name="response"></a><span data-ttu-id="d3622-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3622-157">Response</span></span>

<span data-ttu-id="d3622-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d3622-158">The following is an example of the response.</span></span>

><span data-ttu-id="d3622-159">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d3622-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d3622-160">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3622-160">All the properties will be returned from an actual call.</span></span>
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
