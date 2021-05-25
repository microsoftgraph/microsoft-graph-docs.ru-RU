---
title: Создание дочерней папки
description: С помощью этого API можно создать дочернюю папку почты.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4d8d43e4bb3840fa248ab6b1f1109dc2061ff695
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629142"
---
# <a name="create-child-folder"></a><span data-ttu-id="71223-103">Создание дочерней папки</span><span class="sxs-lookup"><span data-stu-id="71223-103">Create child folder</span></span>

<span data-ttu-id="71223-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71223-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71223-105">Используйте этот API для создания нового [почтового ящика для детей.](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="71223-105">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

<span data-ttu-id="71223-106">Если предполагается, что новая папка будет скрыта, необходимо настроить свойство **isHidden** для `true` создания.</span><span class="sxs-lookup"><span data-stu-id="71223-106">If you intend a new folder to be hidden, you must set the **isHidden** property to `true` on creation.</span></span>

## <a name="permissions"></a><span data-ttu-id="71223-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71223-107">Permissions</span></span>

<span data-ttu-id="71223-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71223-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71223-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71223-110">Permission type</span></span> | <span data-ttu-id="71223-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71223-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="71223-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71223-112">Delegated (work or school account)</span></span> | <span data-ttu-id="71223-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71223-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="71223-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71223-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71223-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71223-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="71223-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71223-116">Application</span></span> | <span data-ttu-id="71223-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71223-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="71223-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71223-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="71223-119">Укажите родительную папку в URL-адресе запроса в качестве ИД папки или имени известной папки.</span><span class="sxs-lookup"><span data-stu-id="71223-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="71223-120">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="71223-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="71223-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71223-121">Request headers</span></span>

| <span data-ttu-id="71223-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71223-122">Header</span></span> | <span data-ttu-id="71223-123">Значение</span><span class="sxs-lookup"><span data-stu-id="71223-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="71223-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71223-124">Authorization</span></span> | <span data-ttu-id="71223-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="71223-125">`Bearer {token}`.</span></span> <span data-ttu-id="71223-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="71223-126">Required.</span></span> |
| <span data-ttu-id="71223-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71223-127">Content-Type</span></span> | <span data-ttu-id="71223-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="71223-128">`application/json`.</span></span> <span data-ttu-id="71223-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="71223-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71223-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71223-130">Request body</span></span>

<span data-ttu-id="71223-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="71223-131">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="71223-132">**displayName** и **isHidden** являются единственными свойствами для объекта [mailFolder.](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="71223-132">**displayName** and **isHidden** are the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="71223-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="71223-133">Parameter</span></span> | <span data-ttu-id="71223-134">Тип</span><span class="sxs-lookup"><span data-stu-id="71223-134">Type</span></span> | <span data-ttu-id="71223-135">Описание</span><span class="sxs-lookup"><span data-stu-id="71223-135">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="71223-136">displayName</span><span class="sxs-lookup"><span data-stu-id="71223-136">displayName</span></span>|<span data-ttu-id="71223-137">Строка</span><span class="sxs-lookup"><span data-stu-id="71223-137">String</span></span>|<span data-ttu-id="71223-138">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="71223-138">The display name of the new folder.</span></span>|
|<span data-ttu-id="71223-139">isHidden</span><span class="sxs-lookup"><span data-stu-id="71223-139">isHidden</span></span>|<span data-ttu-id="71223-140">Логический</span><span class="sxs-lookup"><span data-stu-id="71223-140">Boolean</span></span>|<span data-ttu-id="71223-141">Указывает, скрыта ли новая папка.</span><span class="sxs-lookup"><span data-stu-id="71223-141">Indicates whether the new folder is hidden.</span></span> <span data-ttu-id="71223-142">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="71223-142">The default value is `false`.</span></span> <span data-ttu-id="71223-143">Настройка свойства необязательна.</span><span class="sxs-lookup"><span data-stu-id="71223-143">Setting the property is optional.</span></span> <span data-ttu-id="71223-144">После набора невозможно обновить это свойство.</span><span class="sxs-lookup"><span data-stu-id="71223-144">Once set, you cannot update this property.</span></span> <span data-ttu-id="71223-145">Дополнительные сведения см. в [папках "Скрытая почта"](../resources/mailfolder.md#hidden-mail-folders)</span><span class="sxs-lookup"><span data-stu-id="71223-145">See more information in [Hidden mail folders](../resources/mailfolder.md#hidden-mail-folders)</span></span>|

## <a name="response"></a><span data-ttu-id="71223-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="71223-146">Response</span></span>

<span data-ttu-id="71223-147">В случае успешного использования этот метод возвращает код ответа и ресурс `201 Created` [mailFolder](../resources/mailfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="71223-147">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71223-148">Пример</span><span class="sxs-lookup"><span data-stu-id="71223-148">Example</span></span>

##### <a name="request"></a><span data-ttu-id="71223-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="71223-149">Request</span></span>

<span data-ttu-id="71223-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71223-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71223-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="71223-151">HTTP</span></span>](#tab/http)
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
  "isHidden": true
}
```
# <a name="c"></a>[<span data-ttu-id="71223-152">C#</span><span class="sxs-lookup"><span data-stu-id="71223-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71223-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71223-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71223-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71223-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71223-155">Java</span><span class="sxs-lookup"><span data-stu-id="71223-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="71223-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="71223-156">Response</span></span>
<span data-ttu-id="71223-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71223-157">Here is an example of the response.</span></span>

> <span data-ttu-id="71223-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="71223-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "id": "id-value",
  "isHidden": true
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

