---
title: Список childFolders
description: 'Получение коллекции папок в указанной папке. Вы можете использовать короткий путь `.../me/MailFolders` для получения верхнего уровня '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: e8650156ae6d6beb6075f8265faae1ab06ac1a93
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454386"
---
# <a name="list-childfolders"></a><span data-ttu-id="f9569-104">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="f9569-104">List childFolders</span></span>

<span data-ttu-id="f9569-p102">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/mailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="f9569-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9569-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9569-107">Permissions</span></span>
<span data-ttu-id="f9569-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9569-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9569-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9569-110">Permission type</span></span>      | <span data-ttu-id="f9569-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9569-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9569-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9569-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9569-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9569-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f9569-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9569-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9569-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9569-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f9569-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9569-116">Application</span></span> | <span data-ttu-id="f9569-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9569-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9569-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9569-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9569-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f9569-119">Optional query parameters</span></span>
<span data-ttu-id="f9569-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f9569-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f9569-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9569-121">Request headers</span></span>
| <span data-ttu-id="f9569-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f9569-122">Name</span></span>       | <span data-ttu-id="f9569-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f9569-123">Type</span></span> | <span data-ttu-id="f9569-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f9569-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f9569-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9569-125">Authorization</span></span>  | <span data-ttu-id="f9569-126">string</span><span class="sxs-lookup"><span data-stu-id="f9569-126">string</span></span>  | <span data-ttu-id="f9569-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9569-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9569-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9569-129">Request body</span></span>
<span data-ttu-id="f9569-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9569-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9569-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9569-131">Response</span></span>

<span data-ttu-id="f9569-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9569-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9569-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f9569-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9569-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9569-134">Request</span></span>
<span data-ttu-id="f9569-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9569-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f9569-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9569-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9569-137">C#</span><span class="sxs-lookup"><span data-stu-id="f9569-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9569-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9569-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9569-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9569-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f9569-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9569-140">Response</span></span>
<span data-ttu-id="f9569-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9569-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
