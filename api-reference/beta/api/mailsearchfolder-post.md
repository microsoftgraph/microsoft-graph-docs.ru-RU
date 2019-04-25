---
title: Создание Маилсеарчфолдер
description: Используйте этот API, чтобы создать новый Маилсеарчфолдер в почтовом ящике указанного пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ef9992e1b0eaee83c39831424215cb9756f895d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540655"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="51474-103">Создание Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="51474-103">Create mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51474-104">Используйте этот API, чтобы создать новый [маилсеарчфолдер](../resources/mailsearchfolder.md) в почтовом ящике указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="51474-104">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="51474-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51474-105">Permissions</span></span>

<span data-ttu-id="51474-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51474-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51474-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51474-108">Permission type</span></span> | <span data-ttu-id="51474-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51474-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="51474-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51474-110">Delegated (work or school account)</span></span> | <span data-ttu-id="51474-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51474-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="51474-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51474-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51474-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51474-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="51474-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51474-114">Application</span></span> | <span data-ttu-id="51474-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51474-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="51474-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51474-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="51474-117">Укажите родительскую папку в URL-АДРЕСе запроса как идентификатор папки или известное имя папки.</span><span class="sxs-lookup"><span data-stu-id="51474-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="51474-118">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="51474-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="51474-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51474-119">Request headers</span></span>

| <span data-ttu-id="51474-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51474-120">Header</span></span> | <span data-ttu-id="51474-121">Значение</span><span class="sxs-lookup"><span data-stu-id="51474-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="51474-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51474-122">Authorization</span></span> | <span data-ttu-id="51474-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="51474-123"></span></span> <span data-ttu-id="51474-124">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="51474-124">Required.</span></span> |
| <span data-ttu-id="51474-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51474-125">Content-Type</span></span> | <span data-ttu-id="51474-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="51474-126"></span></span> <span data-ttu-id="51474-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51474-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51474-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51474-128">Request body</span></span>

<span data-ttu-id="51474-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="51474-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="51474-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="51474-130">Parameter</span></span> | <span data-ttu-id="51474-131">Тип</span><span class="sxs-lookup"><span data-stu-id="51474-131">Type</span></span> | <span data-ttu-id="51474-132">Описание</span><span class="sxs-lookup"><span data-stu-id="51474-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="51474-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="51474-133">@odata.type</span></span> | <span data-ttu-id="51474-134">String</span><span class="sxs-lookup"><span data-stu-id="51474-134">String</span></span> | <span data-ttu-id="51474-135">Тип создаваемой папки.</span><span class="sxs-lookup"><span data-stu-id="51474-135">The type of folder to be created.</span></span> <span data-ttu-id="51474-136">Задано значение "Microsoft. Graph. Маилсеарчфолдер".</span><span class="sxs-lookup"><span data-stu-id="51474-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="51474-137">displayName</span><span class="sxs-lookup"><span data-stu-id="51474-137">displayName</span></span> | <span data-ttu-id="51474-138">String</span><span class="sxs-lookup"><span data-stu-id="51474-138">String</span></span> | <span data-ttu-id="51474-139">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="51474-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="51474-140">Инклуденестедфолдерс</span><span class="sxs-lookup"><span data-stu-id="51474-140">includeNestedFolders</span></span> | <span data-ttu-id="51474-141">Логический</span><span class="sxs-lookup"><span data-stu-id="51474-141">Boolean</span></span> | <span data-ttu-id="51474-142">Способ обхода иерархии папок почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="51474-142">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="51474-143">`true`означает, что следует выполнить глубокий поиск, а `false` это означает, что вместо этого следует выполнить неглубокий Поиск.</span><span class="sxs-lookup"><span data-stu-id="51474-143">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="51474-144">Саурцефолдеридс</span><span class="sxs-lookup"><span data-stu-id="51474-144">sourceFolderIDs</span></span> | <span data-ttu-id="51474-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="51474-145">String collection</span></span> | <span data-ttu-id="51474-146">Папки почтовых ящиков, которые должны быть mined.</span><span class="sxs-lookup"><span data-stu-id="51474-146">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="51474-147">Филтеркуери</span><span class="sxs-lookup"><span data-stu-id="51474-147">filterQuery</span></span> | <span data-ttu-id="51474-148">String</span><span class="sxs-lookup"><span data-stu-id="51474-148">String</span></span> | <span data-ttu-id="51474-149">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="51474-149">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="51474-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="51474-150">Response</span></span>

<span data-ttu-id="51474-151">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [маилсеарчфолдер](../resources/mailsearchfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51474-151">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51474-152">Пример</span><span class="sxs-lookup"><span data-stu-id="51474-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="51474-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="51474-153">Request</span></span>

<span data-ttu-id="51474-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51474-154">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="51474-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="51474-155">Response</span></span>

<span data-ttu-id="51474-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51474-156">The following is an example of the response.</span></span>

><span data-ttu-id="51474-157">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="51474-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="51474-158">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51474-158">All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/mailsearchfolder-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
