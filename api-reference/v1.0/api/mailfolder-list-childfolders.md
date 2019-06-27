---
title: Список childFolders
description: 'Получение коллекции папок в указанной папке. Вы можете использовать короткий путь `.../me/MailFolders` для получения верхнего уровня '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: defe2ff5885ce36f21517aadaa72e38ce50353c8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266264"
---
# <a name="list-childfolders"></a><span data-ttu-id="53656-104">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="53656-104">List childFolders</span></span>

<span data-ttu-id="53656-p102">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/mailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="53656-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="53656-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53656-107">Permissions</span></span>
<span data-ttu-id="53656-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53656-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53656-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53656-110">Permission type</span></span>      | <span data-ttu-id="53656-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53656-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53656-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53656-112">Delegated (work or school account)</span></span> | <span data-ttu-id="53656-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53656-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="53656-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53656-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53656-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53656-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="53656-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53656-116">Application</span></span> | <span data-ttu-id="53656-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53656-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="53656-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53656-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="53656-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="53656-119">Optional query parameters</span></span>
<span data-ttu-id="53656-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="53656-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="53656-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53656-121">Request headers</span></span>
| <span data-ttu-id="53656-122">Имя</span><span class="sxs-lookup"><span data-stu-id="53656-122">Name</span></span>       | <span data-ttu-id="53656-123">Тип</span><span class="sxs-lookup"><span data-stu-id="53656-123">Type</span></span> | <span data-ttu-id="53656-124">Описание</span><span class="sxs-lookup"><span data-stu-id="53656-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="53656-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="53656-125">Authorization</span></span>  | <span data-ttu-id="53656-126">string</span><span class="sxs-lookup"><span data-stu-id="53656-126">string</span></span>  | <span data-ttu-id="53656-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53656-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53656-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53656-129">Request body</span></span>
<span data-ttu-id="53656-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53656-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53656-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="53656-131">Response</span></span>

<span data-ttu-id="53656-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53656-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53656-133">Пример</span><span class="sxs-lookup"><span data-stu-id="53656-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53656-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="53656-134">Request</span></span>
<span data-ttu-id="53656-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53656-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="53656-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="53656-136">Response</span></span>
<span data-ttu-id="53656-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53656-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="53656-140">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="53656-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="53656-141">C#</span><span class="sxs-lookup"><span data-stu-id="53656-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53656-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53656-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="53656-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53656-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_childfolders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
