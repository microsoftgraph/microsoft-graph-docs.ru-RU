---
title: Список childFolders
description: 'Получение коллекции папок в указанной папке. Вы можете использовать короткий путь `.../me/MailFolders` для получения верхнего уровня '
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3b8cb47681963233543a40449a1206c3206bb2f0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131609"
---
# <a name="list-childfolders"></a><span data-ttu-id="e42f2-104">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="e42f2-104">List childFolders</span></span>

<span data-ttu-id="e42f2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e42f2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e42f2-p102">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/mailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="e42f2-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="e42f2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e42f2-108">Permissions</span></span>
<span data-ttu-id="e42f2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e42f2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e42f2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e42f2-111">Permission type</span></span>      | <span data-ttu-id="e42f2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e42f2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e42f2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e42f2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e42f2-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e42f2-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e42f2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e42f2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e42f2-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e42f2-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e42f2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e42f2-117">Application</span></span> | <span data-ttu-id="e42f2-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e42f2-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e42f2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e42f2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e42f2-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e42f2-120">Optional query parameters</span></span>
<span data-ttu-id="e42f2-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e42f2-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e42f2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e42f2-122">Request headers</span></span>
| <span data-ttu-id="e42f2-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e42f2-123">Name</span></span>       | <span data-ttu-id="e42f2-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e42f2-124">Type</span></span> | <span data-ttu-id="e42f2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e42f2-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e42f2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e42f2-126">Authorization</span></span>  | <span data-ttu-id="e42f2-127">string</span><span class="sxs-lookup"><span data-stu-id="e42f2-127">string</span></span>  | <span data-ttu-id="e42f2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e42f2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e42f2-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e42f2-130">Request body</span></span>
<span data-ttu-id="e42f2-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e42f2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e42f2-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e42f2-132">Response</span></span>

<span data-ttu-id="e42f2-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e42f2-133">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e42f2-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e42f2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e42f2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e42f2-135">Request</span></span>
<span data-ttu-id="e42f2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e42f2-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e42f2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e42f2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
# <a name="c"></a>[<span data-ttu-id="e42f2-138">C#</span><span class="sxs-lookup"><span data-stu-id="e42f2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e42f2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e42f2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e42f2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e42f2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e42f2-141">Java</span><span class="sxs-lookup"><span data-stu-id="e42f2-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e42f2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e42f2-142">Response</span></span>
<span data-ttu-id="e42f2-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e42f2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
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
