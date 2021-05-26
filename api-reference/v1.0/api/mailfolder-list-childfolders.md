---
title: Список childFolders
description: 'Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете перейти к верхнему уровню '
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 73a812b9f1b3899d52d112649ceebb0c594b8489
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666486"
---
# <a name="list-childfolders"></a><span data-ttu-id="32f06-104">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="32f06-104">List childFolders</span></span>

<span data-ttu-id="32f06-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32f06-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32f06-p102">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/mailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="32f06-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

<span data-ttu-id="32f06-108">По умолчанию эта операция не возвращает скрытые папки.</span><span class="sxs-lookup"><span data-stu-id="32f06-108">By default, this operation does not return hidden folders.</span></span> <span data-ttu-id="32f06-109">Используйте параметр запроса _includeHiddenFolders_, чтобы включить их в отклик.</span><span class="sxs-lookup"><span data-stu-id="32f06-109">Use a query parameter _includeHiddenFolders_ to include them in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="32f06-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32f06-110">Permissions</span></span>
<span data-ttu-id="32f06-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32f06-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32f06-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32f06-113">Permission type</span></span>      | <span data-ttu-id="32f06-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32f06-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32f06-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32f06-115">Delegated (work or school account)</span></span> | <span data-ttu-id="32f06-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32f06-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="32f06-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32f06-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32f06-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32f06-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="32f06-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="32f06-119">Application</span></span> | <span data-ttu-id="32f06-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32f06-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="32f06-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32f06-121">HTTP request</span></span>

<span data-ttu-id="32f06-122">Чтобы получить все дочерние папки в указанной папке, за исключением скрытых:</span><span class="sxs-lookup"><span data-stu-id="32f06-122">To get all the child folders under the specified folder, excluding those that are hidden:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="32f06-123">Чтобы включить _скрытые_ дочерние папки в отклик:</span><span class="sxs-lookup"><span data-stu-id="32f06-123">To include _hidden_ child folders in the response:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders?includeHiddenFolders=true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32f06-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="32f06-124">Optional query parameters</span></span>
<span data-ttu-id="32f06-125">Чтобы вернуть список всех объектов childFolder, включая скрытые (их свойство **isHidden** имеет значение true), в URL-адресе запроса укажите параметр запроса `includeHiddenFolders` как `true`, как показано в разделе [HTTP-запрос](#http-request).</span><span class="sxs-lookup"><span data-stu-id="32f06-125">To return a list of all childFolders including those that are hidden (their **isHidden** property is true), in the request URL, specify the `includeHiddenFolders` query parameter as `true`, as shown in the [HTTP request](#http-request) section.</span></span>

<span data-ttu-id="32f06-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="32f06-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="32f06-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32f06-127">Request headers</span></span>
| <span data-ttu-id="32f06-128">Имя</span><span class="sxs-lookup"><span data-stu-id="32f06-128">Name</span></span>       | <span data-ttu-id="32f06-129">Тип</span><span class="sxs-lookup"><span data-stu-id="32f06-129">Type</span></span> | <span data-ttu-id="32f06-130">Описание</span><span class="sxs-lookup"><span data-stu-id="32f06-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="32f06-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="32f06-131">Authorization</span></span>  | <span data-ttu-id="32f06-132">string</span><span class="sxs-lookup"><span data-stu-id="32f06-132">string</span></span>  | <span data-ttu-id="32f06-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32f06-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32f06-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32f06-135">Request body</span></span>
<span data-ttu-id="32f06-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32f06-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32f06-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="32f06-137">Response</span></span>

<span data-ttu-id="32f06-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32f06-138">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32f06-139">Пример</span><span class="sxs-lookup"><span data-stu-id="32f06-139">Example</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="32f06-140">Пример 1. Перечисление папок почты</span><span class="sxs-lookup"><span data-stu-id="32f06-140">Example 1: List mail folders</span></span>

<span data-ttu-id="32f06-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32f06-141">The following is an example of the request.</span></span>

##### <a name="request"></a><span data-ttu-id="32f06-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="32f06-142">Request</span></span>
<span data-ttu-id="32f06-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32f06-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="32f06-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="32f06-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
# <a name="c"></a>[<span data-ttu-id="32f06-145">C#</span><span class="sxs-lookup"><span data-stu-id="32f06-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32f06-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32f06-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32f06-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32f06-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32f06-148">Java</span><span class="sxs-lookup"><span data-stu-id="32f06-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="32f06-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="32f06-149">Response</span></span>
<span data-ttu-id="32f06-p106">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="32f06-p106">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "id": "id-value",
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "isHidden": false
    }
  ]
}
```
### <a name="example-2-include-hidden-child-folders-under-a-specified-mail-folder"></a><span data-ttu-id="32f06-152">Пример 2. Включение скрытых дочерних папок в указанную папку почты</span><span class="sxs-lookup"><span data-stu-id="32f06-152">Example 2: Include hidden child folders under a specified mail folder</span></span>

<span data-ttu-id="32f06-153">В следующем примере параметр запроса `includeHiddenFolders` используется для получения списка дочерних папок в указанной почтовой папке, включая скрытые почтовые папки.</span><span class="sxs-lookup"><span data-stu-id="32f06-153">The next example uses the `includeHiddenFolders` query parameter to get a list of child folders under a specified mail folder including hidden mail folders.</span></span> <span data-ttu-id="32f06-154">Отклик включает папку "Несрочные", параметру **isHidden** которой присвоено значение true.</span><span class="sxs-lookup"><span data-stu-id="32f06-154">The response includes the "Clutters" folder that has the **isHidden** set to true.</span></span>

##### <a name="request"></a><span data-ttu-id="32f06-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="32f06-155">Request</span></span>
<span data-ttu-id="32f06-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32f06-156">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="32f06-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="32f06-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_hiddenchildfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders?includeHiddenFolders=true
```
# <a name="c"></a>[<span data-ttu-id="32f06-158">C#</span><span class="sxs-lookup"><span data-stu-id="32f06-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-hiddenchildfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32f06-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32f06-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-hiddenchildfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32f06-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32f06-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-hiddenchildfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32f06-161">Java</span><span class="sxs-lookup"><span data-stu-id="32f06-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-hiddenchildfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="32f06-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="32f06-162">Response</span></span>
<span data-ttu-id="32f06-p108">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="32f06-p108">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "id": "AAMkAGVmMDEzA",
      "displayName": "Internal Screens",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 2,
      "isHidden": false
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Clutters",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "isHidden": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
