---
title: Создание mailSearchFolder
description: Используйте этот интерфейс API для создания нового mailSearchFolder в почтовом ящике указанного пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ef9992e1b0eaee83c39831424215cb9756f895d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517731"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="c4722-103">Создание mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="c4722-103">Create mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4722-104">Используйте этот интерфейс API для создания нового [mailSearchFolder](../resources/mailsearchfolder.md) в почтовом ящике указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c4722-104">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4722-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4722-105">Permissions</span></span>

<span data-ttu-id="c4722-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4722-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4722-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4722-108">Permission type</span></span> | <span data-ttu-id="c4722-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4722-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="c4722-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4722-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4722-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4722-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c4722-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4722-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4722-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4722-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c4722-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4722-114">Application</span></span> | <span data-ttu-id="c4722-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4722-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4722-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4722-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="c4722-117">Укажите родительской папки в URL-АДРЕСЕ запроса как идентификатор папки или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="c4722-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="c4722-118">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c4722-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4722-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4722-119">Request headers</span></span>

| <span data-ttu-id="c4722-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4722-120">Header</span></span> | <span data-ttu-id="c4722-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c4722-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="c4722-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4722-122">Authorization</span></span> | <span data-ttu-id="c4722-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="c4722-123"></span></span> <span data-ttu-id="c4722-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4722-124">Required.</span></span> |
| <span data-ttu-id="c4722-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4722-125">Content-Type</span></span> | <span data-ttu-id="c4722-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="c4722-126"></span></span> <span data-ttu-id="c4722-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4722-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4722-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4722-128">Request body</span></span>

<span data-ttu-id="c4722-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c4722-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c4722-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="c4722-130">Parameter</span></span> | <span data-ttu-id="c4722-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c4722-131">Type</span></span> | <span data-ttu-id="c4722-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c4722-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="c4722-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="c4722-133">@odata.type</span></span> | <span data-ttu-id="c4722-134">String</span><span class="sxs-lookup"><span data-stu-id="c4722-134">String</span></span> | <span data-ttu-id="c4722-135">Тип создать папку.</span><span class="sxs-lookup"><span data-stu-id="c4722-135">The type of folder to be created.</span></span> <span data-ttu-id="c4722-136">Задайте значение «microsoft.graph.mailSearchFolder».</span><span class="sxs-lookup"><span data-stu-id="c4722-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="c4722-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c4722-137">displayName</span></span> | <span data-ttu-id="c4722-138">String</span><span class="sxs-lookup"><span data-stu-id="c4722-138">String</span></span> | <span data-ttu-id="c4722-139">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="c4722-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="c4722-140">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="c4722-140">includeNestedFolders</span></span> | <span data-ttu-id="c4722-141">Логическое</span><span class="sxs-lookup"><span data-stu-id="c4722-141">Boolean</span></span> | <span data-ttu-id="c4722-142">Как следует обход иерархии папок почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c4722-142">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="c4722-143">`true`означает, что глубокого поиска должны быть в то время как `false` означает, что следует частичного поиска.</span><span class="sxs-lookup"><span data-stu-id="c4722-143">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="c4722-144">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="c4722-144">sourceFolderIDs</span></span> | <span data-ttu-id="c4722-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c4722-145">String collection</span></span> | <span data-ttu-id="c4722-146">Папки почтовых ящиков, которые должны быть получены.</span><span class="sxs-lookup"><span data-stu-id="c4722-146">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="c4722-147">filterQuery</span><span class="sxs-lookup"><span data-stu-id="c4722-147">filterQuery</span></span> | <span data-ttu-id="c4722-148">String</span><span class="sxs-lookup"><span data-stu-id="c4722-148">String</span></span> | <span data-ttu-id="c4722-149">Запросов OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="c4722-149">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="c4722-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4722-150">Response</span></span>

<span data-ttu-id="c4722-151">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [mailSearchFolder](../resources/mailsearchfolder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c4722-151">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4722-152">Пример</span><span class="sxs-lookup"><span data-stu-id="c4722-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c4722-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4722-153">Request</span></span>

<span data-ttu-id="c4722-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4722-154">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="c4722-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4722-155">Response</span></span>

<span data-ttu-id="c4722-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4722-156">The following is an example of the response.</span></span>

><span data-ttu-id="c4722-157">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c4722-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c4722-158">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4722-158">All the properties will be returned from an actual call.</span></span>
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
