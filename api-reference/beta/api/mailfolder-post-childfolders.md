---
title: Создание mailFolder
description: Используйте этот API для создания нового дочернего элемента mailFolder.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 250c5097afc35222a18f17a342ecb2a70a12d0f3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443374"
---
# <a name="create-mailfolder"></a><span data-ttu-id="bdfce-103">Создание mailFolder</span><span class="sxs-lookup"><span data-stu-id="bdfce-103">Create mailFolder</span></span>

<span data-ttu-id="bdfce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdfce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdfce-105">Используйте этот API для создания нового дочернего элемента [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="bdfce-105">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdfce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdfce-106">Permissions</span></span>

<span data-ttu-id="bdfce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdfce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdfce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdfce-109">Permission type</span></span> | <span data-ttu-id="bdfce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdfce-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="bdfce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdfce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bdfce-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdfce-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bdfce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdfce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdfce-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdfce-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bdfce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdfce-115">Application</span></span> | <span data-ttu-id="bdfce-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdfce-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdfce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdfce-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="bdfce-118">Укажите родительскую папку в URL-адресе запроса как идентификатор папки или известное имя папки.</span><span class="sxs-lookup"><span data-stu-id="bdfce-118">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="bdfce-119">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="bdfce-119">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bdfce-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdfce-120">Request headers</span></span>

| <span data-ttu-id="bdfce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdfce-121">Header</span></span> | <span data-ttu-id="bdfce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bdfce-122">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="bdfce-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdfce-123">Authorization</span></span> | <span data-ttu-id="bdfce-124">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="bdfce-124">`Bearer {token}`.</span></span> <span data-ttu-id="bdfce-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="bdfce-125">Required.</span></span> |
| <span data-ttu-id="bdfce-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bdfce-126">Content-Type</span></span> | <span data-ttu-id="bdfce-127">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="bdfce-127">`application/json`.</span></span> <span data-ttu-id="bdfce-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="bdfce-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdfce-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bdfce-129">Request body</span></span>

<span data-ttu-id="bdfce-p105">Предоставьте в тексте запроса объект JSON с указанными ниже параметрами. **displayName** — это единственное доступное для записи свойство объекта [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="bdfce-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="bdfce-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="bdfce-132">Parameter</span></span> | <span data-ttu-id="bdfce-133">Тип</span><span class="sxs-lookup"><span data-stu-id="bdfce-133">Type</span></span> | <span data-ttu-id="bdfce-134">Описание</span><span class="sxs-lookup"><span data-stu-id="bdfce-134">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="bdfce-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bdfce-135">displayName</span></span>|<span data-ttu-id="bdfce-136">String</span><span class="sxs-lookup"><span data-stu-id="bdfce-136">String</span></span>|<span data-ttu-id="bdfce-137">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="bdfce-137">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="bdfce-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdfce-138">Response</span></span>

<span data-ttu-id="bdfce-139">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bdfce-139">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdfce-140">Пример</span><span class="sxs-lookup"><span data-stu-id="bdfce-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bdfce-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdfce-141">Request</span></span>

<span data-ttu-id="bdfce-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdfce-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bdfce-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdfce-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
# <a name="c"></a>[<span data-ttu-id="bdfce-144">C#</span><span class="sxs-lookup"><span data-stu-id="bdfce-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bdfce-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdfce-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bdfce-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdfce-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bdfce-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdfce-147">Response</span></span>

<span data-ttu-id="bdfce-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bdfce-148">The following is an example of the response.</span></span>

> <span data-ttu-id="bdfce-149">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bdfce-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bdfce-150">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdfce-150">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
