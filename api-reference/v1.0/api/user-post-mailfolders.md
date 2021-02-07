---
title: Создание объекта MailFolder
description: С помощью этого API можно создать папку почты в корневой папке почтового ящика пользователя.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 434e3ae114f0514ad002939aa1a39f82b0c31455
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137223"
---
# <a name="create-mailfolder"></a><span data-ttu-id="b4c33-103">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="b4c33-103">Create MailFolder</span></span>

<span data-ttu-id="b4c33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4c33-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b4c33-105">С помощью этого API можно создать папку почты в корневой папке почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4c33-105">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="b4c33-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4c33-106">Permissions</span></span>
<span data-ttu-id="b4c33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4c33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4c33-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4c33-109">Permission type</span></span>      | <span data-ttu-id="b4c33-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4c33-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4c33-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4c33-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b4c33-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4c33-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b4c33-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4c33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4c33-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4c33-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b4c33-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4c33-115">Application</span></span> | <span data-ttu-id="b4c33-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4c33-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4c33-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4c33-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="b4c33-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4c33-118">Request headers</span></span>
| <span data-ttu-id="b4c33-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4c33-119">Header</span></span>       | <span data-ttu-id="b4c33-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b4c33-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b4c33-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4c33-121">Authorization</span></span>  | <span data-ttu-id="b4c33-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4c33-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b4c33-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4c33-124">Content-Type</span></span>  | <span data-ttu-id="b4c33-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b4c33-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4c33-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4c33-126">Request body</span></span>
<span data-ttu-id="b4c33-p103">Предоставьте в тексте запроса объект JSON с указанными ниже параметрами. **displayName** — это единственное доступное для записи свойство объекта [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="b4c33-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="b4c33-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="b4c33-129">Parameter</span></span>    | <span data-ttu-id="b4c33-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b4c33-130">Type</span></span>   |<span data-ttu-id="b4c33-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b4c33-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4c33-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b4c33-132">displayName</span></span>|<span data-ttu-id="b4c33-133">String</span><span class="sxs-lookup"><span data-stu-id="b4c33-133">String</span></span>|<span data-ttu-id="b4c33-134">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="b4c33-134">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="b4c33-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4c33-135">Response</span></span>

<span data-ttu-id="b4c33-136">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [MailFolder](../resources/mailfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b4c33-136">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4c33-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b4c33-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4c33-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4c33-138">Request</span></span>
<span data-ttu-id="b4c33-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4c33-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b4c33-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4c33-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "Clutter"
}
```
# <a name="c"></a>[<span data-ttu-id="b4c33-141">C#</span><span class="sxs-lookup"><span data-stu-id="b4c33-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4c33-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4c33-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4c33-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4c33-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4c33-144">Java</span><span class="sxs-lookup"><span data-stu-id="b4c33-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b4c33-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4c33-145">Response</span></span>
<span data-ttu-id="b4c33-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4c33-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "hN2Y5OGRhNGYwODEALgAAA0DAKbvJvFhJgcT3lZpkhNQBAA1"
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

