---
title: 'outlookUser: supportedLanguages'
description: Получение списка поддерживаемых языковых стандартов и языков, которые настроены на сервере почтовых ящиков пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c9a25b0f5f6972eba1b03be9b2f94f94dc74a552
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611731"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="5b501-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="5b501-103">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="5b501-104">Получение списка поддерживаемых языковых стандартов и языков, которые настроены на сервере почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="5b501-104">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="5b501-105">Настраивая клиент Outlook, пользователь выбирает язык из этого списка.</span><span class="sxs-lookup"><span data-stu-id="5b501-105">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="5b501-106">После этого вы можете получить выбранный язык вместе с [ настройками почтового ящика пользователя](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="5b501-106">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="5b501-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b501-107">Permissions</span></span>
<span data-ttu-id="5b501-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b501-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b501-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b501-110">Permission type</span></span>      | <span data-ttu-id="5b501-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b501-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b501-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b501-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5b501-113">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="5b501-113">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="5b501-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b501-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b501-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="5b501-115">User.Read</span></span>    |
|<span data-ttu-id="5b501-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b501-116">Application</span></span> | <span data-ttu-id="5b501-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b501-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b501-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b501-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="5b501-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b501-119">Request headers</span></span>
| <span data-ttu-id="5b501-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5b501-120">Name</span></span>       | <span data-ttu-id="5b501-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5b501-121">Type</span></span> | <span data-ttu-id="5b501-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5b501-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5b501-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b501-123">Authorization</span></span>  | <span data-ttu-id="5b501-124">string</span><span class="sxs-lookup"><span data-stu-id="5b501-124">string</span></span>  | <span data-ttu-id="5b501-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b501-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5b501-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b501-127">Request body</span></span>
<span data-ttu-id="5b501-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b501-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b501-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b501-129">Response</span></span>
<span data-ttu-id="5b501-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [localeInfo](../resources/localeinfo.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5b501-130">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b501-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5b501-131">Example</span></span>
<span data-ttu-id="5b501-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5b501-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5b501-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b501-133">Request</span></span>
<span data-ttu-id="5b501-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b501-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="5b501-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b501-135">Response</span></span>
<span data-ttu-id="5b501-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b501-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.localeInfo",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.localeInfo)",
  "value":[
    {
      "locale":"af-ZA",
      "displayName":"Afrikaans (Suid-Afrika)"
    },
    {
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    {
       "locale":"en-CA",
       "displayName":"English (Canada)"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5b501-137">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="5b501-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5b501-138">Языках</span><span class="sxs-lookup"><span data-stu-id="5b501-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedlanguages-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b501-139">Язык</span><span class="sxs-lookup"><span data-stu-id="5b501-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedlanguages-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/outlookuser-supportedlanguages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedlanguages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
