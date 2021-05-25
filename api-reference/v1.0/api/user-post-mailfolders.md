---
title: Создание объекта MailFolder
description: С помощью этого API можно создать папку почты в корневой папке почтового ящика пользователя.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a60f7166337933a3ee8897f9817c6adb148bd05c
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629401"
---
# <a name="create-mailfolder"></a><span data-ttu-id="9cff5-103">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="9cff5-103">Create MailFolder</span></span>

<span data-ttu-id="9cff5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cff5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9cff5-105">С помощью этого API можно создать папку почты в корневой папке почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="9cff5-105">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>

<span data-ttu-id="9cff5-106">Если предполагается, что новая папка будет скрыта, необходимо настроить свойство **isHidden** для `true` создания.</span><span class="sxs-lookup"><span data-stu-id="9cff5-106">If you intend a new folder to be hidden, you must set the **isHidden** property to `true` on creation.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cff5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9cff5-107">Permissions</span></span>
<span data-ttu-id="9cff5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cff5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cff5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cff5-110">Permission type</span></span>      | <span data-ttu-id="9cff5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cff5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cff5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cff5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9cff5-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cff5-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9cff5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cff5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cff5-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cff5-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9cff5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cff5-116">Application</span></span> | <span data-ttu-id="9cff5-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cff5-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cff5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cff5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="9cff5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9cff5-119">Request headers</span></span>
| <span data-ttu-id="9cff5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9cff5-120">Header</span></span>       | <span data-ttu-id="9cff5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9cff5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9cff5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cff5-122">Authorization</span></span>  | <span data-ttu-id="9cff5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cff5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9cff5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9cff5-125">Content-Type</span></span>  | <span data-ttu-id="9cff5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cff5-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9cff5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9cff5-127">Request body</span></span>
<span data-ttu-id="9cff5-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9cff5-128">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="9cff5-129">**displayName** и **isHidden** являются единственными свойствами для объекта [mailFolder.](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="9cff5-129">**displayName** and **isHidden** are the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="9cff5-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="9cff5-130">Parameter</span></span>    | <span data-ttu-id="9cff5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9cff5-131">Type</span></span>   |<span data-ttu-id="9cff5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9cff5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cff5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9cff5-133">displayName</span></span>|<span data-ttu-id="9cff5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9cff5-134">String</span></span>|<span data-ttu-id="9cff5-135">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="9cff5-135">The display name of the new folder.</span></span>|
|<span data-ttu-id="9cff5-136">isHidden</span><span class="sxs-lookup"><span data-stu-id="9cff5-136">isHidden</span></span>|<span data-ttu-id="9cff5-137">Логический</span><span class="sxs-lookup"><span data-stu-id="9cff5-137">Boolean</span></span>|<span data-ttu-id="9cff5-138">Указывает, скрыта ли новая папка.</span><span class="sxs-lookup"><span data-stu-id="9cff5-138">Indicates whether the new folder is hidden.</span></span> <span data-ttu-id="9cff5-139">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="9cff5-139">The default value is `false`.</span></span> <span data-ttu-id="9cff5-140">Настройка свойства необязательна.</span><span class="sxs-lookup"><span data-stu-id="9cff5-140">Setting the property is optional.</span></span> <span data-ttu-id="9cff5-141">После набора невозможно обновить это свойство.</span><span class="sxs-lookup"><span data-stu-id="9cff5-141">Once set, you cannot update this property.</span></span> <span data-ttu-id="9cff5-142">Дополнительные сведения см. в [папках "Скрытая почта"](../resources/mailfolder.md#hidden-mail-folders)</span><span class="sxs-lookup"><span data-stu-id="9cff5-142">See more information in [Hidden mail folders](../resources/mailfolder.md#hidden-mail-folders)</span></span>|

## <a name="response"></a><span data-ttu-id="9cff5-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cff5-143">Response</span></span>

<span data-ttu-id="9cff5-144">В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [mailFolder](../resources/mailfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9cff5-144">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cff5-145">Пример</span><span class="sxs-lookup"><span data-stu-id="9cff5-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="9cff5-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cff5-146">Request</span></span>
<span data-ttu-id="9cff5-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cff5-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9cff5-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cff5-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "Clutter",
  "isHidden": true
}
```
# <a name="c"></a>[<span data-ttu-id="9cff5-149">C#</span><span class="sxs-lookup"><span data-stu-id="9cff5-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cff5-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cff5-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cff5-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cff5-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cff5-152">Java</span><span class="sxs-lookup"><span data-stu-id="9cff5-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9cff5-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cff5-153">Response</span></span>
<span data-ttu-id="9cff5-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9cff5-154">Here is an example of the response.</span></span> 

><span data-ttu-id="9cff5-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9cff5-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 179

{
  "displayName": "Clutter",
  "parentFolderId": "AQMkADlmOGQwZmU3LWVjOWMtNDhiYgAtODcxNy1",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "hN2Y5OGRhNGYwODEALgAAA0DAKbvJvFhJgcT3lZpkhNQBAA1",
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

