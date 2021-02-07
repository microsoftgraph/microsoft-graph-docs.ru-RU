---
title: Создание объекта MailFolder
description: С помощью этого API можно создать дочернюю папку почты.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2b83a9776e39c6bf58e2d42ebd7eaf04a30cb481
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131723"
---
# <a name="create-mailfolder"></a><span data-ttu-id="11e76-103">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="11e76-103">Create MailFolder</span></span>

<span data-ttu-id="11e76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11e76-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11e76-105">С помощью этого API можно создать дочернюю папку почты.</span><span class="sxs-lookup"><span data-stu-id="11e76-105">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="11e76-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11e76-106">Permissions</span></span>

<span data-ttu-id="11e76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11e76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11e76-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11e76-109">Permission type</span></span> | <span data-ttu-id="11e76-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11e76-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="11e76-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11e76-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11e76-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11e76-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="11e76-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11e76-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11e76-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11e76-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="11e76-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11e76-115">Application</span></span> | <span data-ttu-id="11e76-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11e76-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="11e76-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11e76-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="11e76-118">Укажите родительская папка в URL-адресе запроса в качестве ИД папки или известного имени папки.</span><span class="sxs-lookup"><span data-stu-id="11e76-118">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="11e76-119">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="11e76-119">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="11e76-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11e76-120">Request headers</span></span>

| <span data-ttu-id="11e76-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11e76-121">Header</span></span> | <span data-ttu-id="11e76-122">Значение</span><span class="sxs-lookup"><span data-stu-id="11e76-122">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="11e76-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11e76-123">Authorization</span></span> | <span data-ttu-id="11e76-124">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="11e76-124">`Bearer {token}`.</span></span> <span data-ttu-id="11e76-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="11e76-125">Required.</span></span> |
| <span data-ttu-id="11e76-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11e76-126">Content-Type</span></span> | <span data-ttu-id="11e76-127">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="11e76-127">`application/json`.</span></span> <span data-ttu-id="11e76-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="11e76-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11e76-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11e76-129">Request body</span></span>

<span data-ttu-id="11e76-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="11e76-130">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="11e76-131">**displayName** — это единственное свойство, списамое для объекта [mailFolder.](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="11e76-131">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="11e76-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="11e76-132">Parameter</span></span> | <span data-ttu-id="11e76-133">Тип</span><span class="sxs-lookup"><span data-stu-id="11e76-133">Type</span></span> | <span data-ttu-id="11e76-134">Описание</span><span class="sxs-lookup"><span data-stu-id="11e76-134">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="11e76-135">displayName</span><span class="sxs-lookup"><span data-stu-id="11e76-135">displayName</span></span>|<span data-ttu-id="11e76-136">String</span><span class="sxs-lookup"><span data-stu-id="11e76-136">String</span></span>|<span data-ttu-id="11e76-137">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="11e76-137">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="11e76-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="11e76-138">Response</span></span>

<span data-ttu-id="11e76-139">В случае успеха этот метод возвращает код отклика и ресурс `201 Created` [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="11e76-139">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11e76-140">Пример</span><span class="sxs-lookup"><span data-stu-id="11e76-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="11e76-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="11e76-141">Request</span></span>

<span data-ttu-id="11e76-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11e76-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11e76-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="11e76-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
# <a name="c"></a>[<span data-ttu-id="11e76-144">C#</span><span class="sxs-lookup"><span data-stu-id="11e76-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11e76-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11e76-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11e76-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e76-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11e76-147">Java</span><span class="sxs-lookup"><span data-stu-id="11e76-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="11e76-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="11e76-148">Response</span></span>
<span data-ttu-id="11e76-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11e76-149">Here is an example of the response.</span></span>

> <span data-ttu-id="11e76-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11e76-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

