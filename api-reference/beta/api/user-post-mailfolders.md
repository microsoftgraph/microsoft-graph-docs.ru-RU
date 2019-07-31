---
title: Создание объекта MailFolder
description: С помощью этого API можно создать папку почты в корневой папке почтового ящика пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4a98e962cc7b0897c9cdd0a934adcfc08d6a3e2e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996128"
---
# <a name="create-mailfolder"></a><span data-ttu-id="ff7f5-103">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="ff7f5-103">Create MailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff7f5-104">С помощью этого API можно создать папку почты в корневой папке почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="ff7f5-104">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff7f5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff7f5-105">Permissions</span></span>
<span data-ttu-id="ff7f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff7f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff7f5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff7f5-108">Permission type</span></span>      | <span data-ttu-id="ff7f5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff7f5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff7f5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff7f5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff7f5-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff7f5-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ff7f5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff7f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff7f5-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff7f5-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ff7f5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff7f5-114">Application</span></span> | <span data-ttu-id="ff7f5-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff7f5-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff7f5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff7f5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="ff7f5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff7f5-117">Request headers</span></span>
| <span data-ttu-id="ff7f5-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff7f5-118">Header</span></span>       | <span data-ttu-id="ff7f5-119">Значение</span><span class="sxs-lookup"><span data-stu-id="ff7f5-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ff7f5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff7f5-120">Authorization</span></span>  | <span data-ttu-id="ff7f5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff7f5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ff7f5-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff7f5-123">Content-Type</span></span>  | <span data-ttu-id="ff7f5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ff7f5-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff7f5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff7f5-125">Request body</span></span>
<span data-ttu-id="ff7f5-p103">Предоставьте в тексте запроса объект JSON с указанными ниже параметрами. **displayName** — это единственное доступное для записи свойство объекта [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ff7f5-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="ff7f5-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="ff7f5-128">Parameter</span></span>    | <span data-ttu-id="ff7f5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ff7f5-129">Type</span></span>   |<span data-ttu-id="ff7f5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ff7f5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff7f5-131">displayName</span><span class="sxs-lookup"><span data-stu-id="ff7f5-131">displayName</span></span>|<span data-ttu-id="ff7f5-132">String</span><span class="sxs-lookup"><span data-stu-id="ff7f5-132">String</span></span>|<span data-ttu-id="ff7f5-133">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="ff7f5-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="ff7f5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff7f5-134">Response</span></span>

<span data-ttu-id="ff7f5-135">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [MailFolder](../resources/mailfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ff7f5-135">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff7f5-136">Пример</span><span class="sxs-lookup"><span data-stu-id="ff7f5-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff7f5-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff7f5-137">Request</span></span>
<span data-ttu-id="ff7f5-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff7f5-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff7f5-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff7f5-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff7f5-140">C#</span><span class="sxs-lookup"><span data-stu-id="ff7f5-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff7f5-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff7f5-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff7f5-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ff7f5-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ff7f5-143">Java</span><span class="sxs-lookup"><span data-stu-id="ff7f5-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ff7f5-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff7f5-144">Response</span></span>
<span data-ttu-id="ff7f5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff7f5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
