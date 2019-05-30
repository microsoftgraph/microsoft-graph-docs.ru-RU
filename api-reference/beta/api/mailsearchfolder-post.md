---
title: Создание Маилсеарчфолдер
description: Используйте этот API, чтобы создать новый Маилсеарчфолдер в почтовом ящике указанного пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 2fc7a51675b0bfc559b5ab5c9f7a857c84c43174
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536373"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="5dc4b-103">Создание Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="5dc4b-103">Create mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dc4b-104">Используйте этот API, чтобы создать новый [маилсеарчфолдер](../resources/mailsearchfolder.md) в почтовом ящике указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-104">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="5dc4b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5dc4b-105">Permissions</span></span>

<span data-ttu-id="5dc4b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dc4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5dc4b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5dc4b-108">Permission type</span></span> | <span data-ttu-id="5dc4b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5dc4b-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="5dc4b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5dc4b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5dc4b-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5dc4b-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5dc4b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5dc4b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dc4b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5dc4b-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5dc4b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5dc4b-114">Application</span></span> | <span data-ttu-id="5dc4b-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5dc4b-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dc4b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5dc4b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="5dc4b-117">Укажите родительскую папку в URL-адресе запроса как идентификатор папки или известное имя папки.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="5dc4b-118">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="5dc4b-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5dc4b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5dc4b-119">Request headers</span></span>

| <span data-ttu-id="5dc4b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5dc4b-120">Header</span></span> | <span data-ttu-id="5dc4b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5dc4b-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="5dc4b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5dc4b-122">Authorization</span></span> | <span data-ttu-id="5dc4b-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-123"></span></span> <span data-ttu-id="5dc4b-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-124">Required.</span></span> |
| <span data-ttu-id="5dc4b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5dc4b-125">Content-Type</span></span> | <span data-ttu-id="5dc4b-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-126"></span></span> <span data-ttu-id="5dc4b-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5dc4b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5dc4b-128">Request body</span></span>

<span data-ttu-id="5dc4b-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5dc4b-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="5dc4b-130">Parameter</span></span> | <span data-ttu-id="5dc4b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5dc4b-131">Type</span></span> | <span data-ttu-id="5dc4b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5dc4b-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="5dc4b-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="5dc4b-133">@odata.type</span></span> | <span data-ttu-id="5dc4b-134">String</span><span class="sxs-lookup"><span data-stu-id="5dc4b-134">String</span></span> | <span data-ttu-id="5dc4b-135">Тип создаваемой папки.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-135">The type of folder to be created.</span></span> <span data-ttu-id="5dc4b-136">Задано значение "Microsoft. Graph. Маилсеарчфолдер".</span><span class="sxs-lookup"><span data-stu-id="5dc4b-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="5dc4b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5dc4b-137">displayName</span></span> | <span data-ttu-id="5dc4b-138">String</span><span class="sxs-lookup"><span data-stu-id="5dc4b-138">String</span></span> | <span data-ttu-id="5dc4b-139">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="5dc4b-140">Инклуденестедфолдерс</span><span class="sxs-lookup"><span data-stu-id="5dc4b-140">includeNestedFolders</span></span> | <span data-ttu-id="5dc4b-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dc4b-141">Boolean</span></span> | <span data-ttu-id="5dc4b-142">Способ обхода иерархии папок почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-142">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="5dc4b-143">`true`означает, что следует выполнить глубокий поиск, а `false` это означает, что вместо этого следует выполнить неглубокий Поиск.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-143">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="5dc4b-144">Саурцефолдеридс</span><span class="sxs-lookup"><span data-stu-id="5dc4b-144">sourceFolderIDs</span></span> | <span data-ttu-id="5dc4b-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5dc4b-145">String collection</span></span> | <span data-ttu-id="5dc4b-146">Папки почтовых ящиков, которые должны быть mined.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-146">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="5dc4b-147">Филтеркуери</span><span class="sxs-lookup"><span data-stu-id="5dc4b-147">filterQuery</span></span> | <span data-ttu-id="5dc4b-148">String</span><span class="sxs-lookup"><span data-stu-id="5dc4b-148">String</span></span> | <span data-ttu-id="5dc4b-149">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-149">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="5dc4b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="5dc4b-150">Response</span></span>

<span data-ttu-id="5dc4b-151">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [маилсеарчфолдер](../resources/mailsearchfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-151">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dc4b-152">Пример</span><span class="sxs-lookup"><span data-stu-id="5dc4b-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5dc4b-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="5dc4b-153">Request</span></span>

<span data-ttu-id="5dc4b-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childfolders
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Get MyAnalytics",
  "includeNestedFolders": true,
  "sourceFolderIDs": ["AAMkAGVmMDEzM"],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

#### <a name="response"></a><span data-ttu-id="5dc4b-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="5dc4b-155">Response</span></span>

<span data-ttu-id="5dc4b-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-156">The following is an example of the response.</span></span>

><span data-ttu-id="5dc4b-157">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5dc4b-158">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-158">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 13,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
    "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5dc4b-159">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5dc4b-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5dc4b-160">C#</span><span class="sxs-lookup"><span data-stu-id="5dc4b-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_mailsearchfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5dc4b-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="5dc4b-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_mailsearchfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/mailsearchfolder-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailsearchfolder-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
