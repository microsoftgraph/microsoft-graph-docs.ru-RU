---
title: Список объектов mailFolder
description: 'Получение коллекции папок почты в корневой папке вошедшего пользователя. '
author: abheek-das
localization_priority: Priority
doc_type: apiPageType
ms.prod: outlook
ms.openlocfilehash: 707daff5e3043d10c038343967fa421875132788
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629527"
---
# <a name="list-mailfolders"></a><span data-ttu-id="70a0e-103">Список объектов mailFolder</span><span class="sxs-lookup"><span data-stu-id="70a0e-103">List mailFolders</span></span>

<span data-ttu-id="70a0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70a0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70a0e-105">Получение коллекции папок почты непосредственно в корневой папке вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="70a0e-105">Get the mail folder collection directly under the root folder of the signed-in user.</span></span> <span data-ttu-id="70a0e-106">Возвращаемая коллекция включает все [папки поиска почты](../resources/mailsearchfolder.md), расположенные непосредственно в корневой папке.</span><span class="sxs-lookup"><span data-stu-id="70a0e-106">The returned collection includes any [mail search folders](../resources/mailsearchfolder.md) directly under the root.</span></span>

<span data-ttu-id="70a0e-107">По умолчанию эта операция не возвращает скрытые папки.</span><span class="sxs-lookup"><span data-stu-id="70a0e-107">By default, this operation does not return hidden folders.</span></span> <span data-ttu-id="70a0e-108">Используйте параметр запроса _includeHiddenFolders_, чтобы включить их в отклик.</span><span class="sxs-lookup"><span data-stu-id="70a0e-108">Use a query parameter _includeHiddenFolders_ to include them in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="70a0e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70a0e-109">Permissions</span></span>
<span data-ttu-id="70a0e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70a0e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70a0e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70a0e-112">Permission type</span></span>      | <span data-ttu-id="70a0e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70a0e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70a0e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70a0e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="70a0e-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70a0e-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="70a0e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70a0e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70a0e-117">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70a0e-117">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="70a0e-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="70a0e-118">Application</span></span> | <span data-ttu-id="70a0e-119">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70a0e-119">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="70a0e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70a0e-120">HTTP request</span></span>

<span data-ttu-id="70a0e-121">Чтобы получить все папки почты в указанном почтовом ящике пользователя, за исключением скрытых:</span><span class="sxs-lookup"><span data-stu-id="70a0e-121">To get all the mail folders in the specified user's mailbox, excluding those that are hidden:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```

<span data-ttu-id="70a0e-122">Чтобы включить _скрытые_ папки почты в отклик:</span><span class="sxs-lookup"><span data-stu-id="70a0e-122">To include _hidden_ mail folders in the response:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/?includeHiddenFolders=true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70a0e-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70a0e-123">Optional query parameters</span></span>
<span data-ttu-id="70a0e-124">Чтобы вернуть список всех объектов mailFolder, включая скрытые (их свойство **isHidden** имеет значение true), в URL-адресе запроса укажите параметр запроса `includeHiddenFolders` как `true`, как показано в разделе [HTTP-запрос](#http-request).</span><span class="sxs-lookup"><span data-stu-id="70a0e-124">To return a list of all mailFolders including those that are hidden (their **isHidden** property is true), in the request URL, specify the `includeHiddenFolders` query parameter as `true`, as shown in the [HTTP request](#http-request) section.</span></span>

<span data-ttu-id="70a0e-125">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="70a0e-125">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="70a0e-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70a0e-126">Request headers</span></span>
| <span data-ttu-id="70a0e-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70a0e-127">Header</span></span>       | <span data-ttu-id="70a0e-128">Значение</span><span class="sxs-lookup"><span data-stu-id="70a0e-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="70a0e-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70a0e-129">Authorization</span></span>  | <span data-ttu-id="70a0e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70a0e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="70a0e-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70a0e-132">Content-Type</span></span>   | <span data-ttu-id="70a0e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="70a0e-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70a0e-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70a0e-134">Request body</span></span>
<span data-ttu-id="70a0e-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70a0e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70a0e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="70a0e-136">Response</span></span>

<span data-ttu-id="70a0e-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70a0e-137">If successful, this method returns a `200 OK` response code and a collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="70a0e-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="70a0e-138">Examples</span></span>

### <a name="example-1-list-mail-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="70a0e-139">Пример 1. Перечисление папок почты из почтового ящика вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="70a0e-139">Example 1: List mail folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="70a0e-140">В этом примере в отклик включается объект **mailSearchFolder**.</span><span class="sxs-lookup"><span data-stu-id="70a0e-140">This example includes a **mailSearchFolder** object in the response.</span></span> <span data-ttu-id="70a0e-141">Папка поиска почты — это дочерняя папка в папке "Входящие" с отображаемым именем "Еженедельные дайджесты".</span><span class="sxs-lookup"><span data-stu-id="70a0e-141">The mail search folder is a child folder under the Inbox with the display name "Weekly digests".</span></span>

#### <a name="request"></a><span data-ttu-id="70a0e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="70a0e-142">Request</span></span>
<span data-ttu-id="70a0e-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70a0e-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70a0e-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="70a0e-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
# <a name="c"></a>[<span data-ttu-id="70a0e-145">C#</span><span class="sxs-lookup"><span data-stu-id="70a0e-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70a0e-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70a0e-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70a0e-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70a0e-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70a0e-148">Java</span><span class="sxs-lookup"><span data-stu-id="70a0e-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="70a0e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="70a0e-149">Response</span></span>
<span data-ttu-id="70a0e-150">Вот пример отклика, содержащего объект **mailSearchFolder**, который является дочерней папкой в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="70a0e-150">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="70a0e-151">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="70a0e-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="70a0e-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70a0e-152">All of the properties will be returned from an actual call.</span></span>

><span data-ttu-id="70a0e-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="70a0e-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders",
    "value": [
        {
            "id": "AQMkADYAAAIBXQAAAA==",
            "displayName": "Archive",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71,
            "isHidden": false
        },
        {
            "@odata.type": "#microsoft.graph.mailSearchFolder",
            "id": "AAMkADYRAAAZg1yTAAA=",
            "displayName": "Weekly digests",
            "parentFolderId": "AQMkADYAAAIBDAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 4,
            "totalItemCount": 5,
            "isHidden": false,
            "isSupported": true,
            "filterQuery": "contains(subject, 'weekly digest')"
        },
        {
            "id": "AQMkADYAAAIBGQAAAA==",
            "displayName": "Junk Email",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        }
    ]
}
```

### <a name="example-2-include-hidden-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="70a0e-154">Пример 2. Включение скрытых папок из почтового ящика вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="70a0e-154">Example 2: Include hidden folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="70a0e-155">В следующем примере параметр запроса `includeHiddenFolders` используется для получения списка папок почты, включая скрытые почтовые папки.</span><span class="sxs-lookup"><span data-stu-id="70a0e-155">The next example uses the `includeHiddenFolders` query parameter to get a list of mail folders including hidden mail folders.</span></span> <span data-ttu-id="70a0e-156">Отклик включает папку "Несрочные", параметру **isHidden** которой присвоено значение true.</span><span class="sxs-lookup"><span data-stu-id="70a0e-156">The response includes the "Clutters" folder that has the **isHidden** set to true.</span></span>

#### <a name="request"></a><span data-ttu-id="70a0e-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="70a0e-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_hiddenmailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/?includeHiddenFolders=true
```

#### <a name="response"></a><span data-ttu-id="70a0e-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="70a0e-158">Response</span></span>
<span data-ttu-id="70a0e-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="70a0e-159">Here is an example of the response.</span></span>

><span data-ttu-id="70a0e-160">**Примечание.** Объект отклика, показанный здесь, сокращен для удобочитаемости и не включает все стандартные папки из почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="70a0e-160">**Note:** The response object shown here is shortened for readability, and doesn't include all the default folders in a user mailbox.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders",
    "value": [
        {
            "id": "AAMkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWAAA=",
            "displayName": "Clutters",
            "parentFolderId": "AAMkADg3NTY5MDg4LWMzYmQtEIAAA=",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": true
        },
        {
            "id": "AAMkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWAAA=",
            "displayName": "Conversation History",
            "parentFolderId": "AAMkADg3NTY5MDg4LWMzYmQtEIAAA=",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
