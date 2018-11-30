---
title: Создание mailSearchFolder
description: Используйте этот интерфейс API для создания нового mailSearchFolder в почтовом ящике указанного пользователя.
ms.openlocfilehash: a35827a6b9164c8d4c1c0fe54a1897b2271fc5d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080816"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="f2508-103">Создание mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="f2508-103">Create mailSearchFolder</span></span>

> <span data-ttu-id="f2508-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f2508-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2508-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2508-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2508-106">Используйте этот интерфейс API для создания нового [mailSearchFolder](../resources/mailsearchfolder.md) в почтовом ящике указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f2508-106">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2508-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2508-107">Permissions</span></span>

<span data-ttu-id="f2508-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2508-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2508-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2508-110">Permission type</span></span> | <span data-ttu-id="f2508-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2508-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="f2508-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2508-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2508-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2508-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f2508-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2508-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2508-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2508-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f2508-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2508-116">Application</span></span> | <span data-ttu-id="f2508-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2508-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2508-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2508-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="f2508-119">Укажите родительской папки в URL-АДРЕСЕ запроса как идентификатор папки или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="f2508-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="f2508-120">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="f2508-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2508-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2508-121">Request headers</span></span>

| <span data-ttu-id="f2508-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2508-122">Header</span></span> | <span data-ttu-id="f2508-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f2508-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="f2508-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2508-124">Authorization</span></span> | <span data-ttu-id="f2508-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="f2508-125"></span></span> <span data-ttu-id="f2508-126">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="f2508-126">Required.</span></span> |
| <span data-ttu-id="f2508-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2508-127">Content-Type</span></span> | <span data-ttu-id="f2508-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="f2508-128"></span></span> <span data-ttu-id="f2508-129">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="f2508-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2508-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2508-130">Request body</span></span>

<span data-ttu-id="f2508-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f2508-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f2508-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="f2508-132">Parameter</span></span> | <span data-ttu-id="f2508-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f2508-133">Type</span></span> | <span data-ttu-id="f2508-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f2508-134">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="f2508-135">@odata.type</span><span class="sxs-lookup"><span data-stu-id="f2508-135">@odata.type</span></span> | <span data-ttu-id="f2508-136">String</span><span class="sxs-lookup"><span data-stu-id="f2508-136">String</span></span> | <span data-ttu-id="f2508-137">Тип создать папку.</span><span class="sxs-lookup"><span data-stu-id="f2508-137">The type of folder to be created.</span></span> <span data-ttu-id="f2508-138">Задайте значение «microsoft.graph.mailSearchFolder».</span><span class="sxs-lookup"><span data-stu-id="f2508-138">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="f2508-139">displayName</span><span class="sxs-lookup"><span data-stu-id="f2508-139">displayName</span></span> | <span data-ttu-id="f2508-140">String</span><span class="sxs-lookup"><span data-stu-id="f2508-140">String</span></span> | <span data-ttu-id="f2508-141">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="f2508-141">The display name of the new folder.</span></span>|
| <span data-ttu-id="f2508-142">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="f2508-142">includeNestedFolders</span></span> | <span data-ttu-id="f2508-143">Логический</span><span class="sxs-lookup"><span data-stu-id="f2508-143">Boolean</span></span> | <span data-ttu-id="f2508-144">Как следует обход иерархии папок почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f2508-144">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="f2508-145">`true`означает, что глубокого поиска должны быть в то время как `false` означает, что следует частичного поиска.</span><span class="sxs-lookup"><span data-stu-id="f2508-145">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="f2508-146">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="f2508-146">sourceFolderIDs</span></span> | <span data-ttu-id="f2508-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f2508-147">String collection</span></span> | <span data-ttu-id="f2508-148">Папки почтовых ящиков, которые должны быть получены.</span><span class="sxs-lookup"><span data-stu-id="f2508-148">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="f2508-149">filterQuery</span><span class="sxs-lookup"><span data-stu-id="f2508-149">filterQuery</span></span> | <span data-ttu-id="f2508-150">String</span><span class="sxs-lookup"><span data-stu-id="f2508-150">String</span></span> | <span data-ttu-id="f2508-151">Запросов OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="f2508-151">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="f2508-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2508-152">Response</span></span>

<span data-ttu-id="f2508-153">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [mailSearchFolder](../resources/mailsearchfolder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f2508-153">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2508-154">Пример</span><span class="sxs-lookup"><span data-stu-id="f2508-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f2508-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2508-155">Request</span></span>

<span data-ttu-id="f2508-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2508-156">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="f2508-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2508-157">Response</span></span>

<span data-ttu-id="f2508-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f2508-158">The following is an example of the response.</span></span>

><span data-ttu-id="f2508-159">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="f2508-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f2508-160">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2508-160">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
