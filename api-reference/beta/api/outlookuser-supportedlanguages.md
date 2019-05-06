---
title: 'outlookUser: supportedLanguages'
description: Получение списка поддерживаемых языковых стандартов и языков, которые настроены на сервере почтовых ящиков пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: dcb136b9086ce2003eb72972224c61a261377c1f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33595974"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="89713-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="89713-103">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="89713-104">Получение списка поддерживаемых языковых стандартов и языков, которые настроены на сервере почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="89713-104">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="89713-105">Настраивая клиент Outlook, пользователь выбирает язык из этого списка.</span><span class="sxs-lookup"><span data-stu-id="89713-105">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="89713-106">После этого вы можете получить выбранный язык вместе с [ настройками почтового ящика пользователя](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="89713-106">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="89713-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89713-107">Permissions</span></span>
<span data-ttu-id="89713-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89713-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89713-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89713-110">Permission type</span></span>      | <span data-ttu-id="89713-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89713-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89713-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89713-112">Delegated (work or school account)</span></span> | <span data-ttu-id="89713-113">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="89713-113">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="89713-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89713-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89713-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="89713-115">User.Read</span></span>    |
|<span data-ttu-id="89713-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89713-116">Application</span></span> | <span data-ttu-id="89713-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="89713-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89713-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89713-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="89713-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89713-119">Request headers</span></span>
| <span data-ttu-id="89713-120">Имя</span><span class="sxs-lookup"><span data-stu-id="89713-120">Name</span></span>       | <span data-ttu-id="89713-121">Тип</span><span class="sxs-lookup"><span data-stu-id="89713-121">Type</span></span> | <span data-ttu-id="89713-122">Описание</span><span class="sxs-lookup"><span data-stu-id="89713-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="89713-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89713-123">Authorization</span></span>  | <span data-ttu-id="89713-124">string</span><span class="sxs-lookup"><span data-stu-id="89713-124">string</span></span>  | <span data-ttu-id="89713-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89713-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="89713-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89713-127">Request body</span></span>
<span data-ttu-id="89713-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89713-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89713-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="89713-129">Response</span></span>
<span data-ttu-id="89713-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [localeInfo](../resources/localeinfo.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="89713-130">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89713-131">Пример</span><span class="sxs-lookup"><span data-stu-id="89713-131">Example</span></span>
<span data-ttu-id="89713-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="89713-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="89713-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="89713-133">Request</span></span>
<span data-ttu-id="89713-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89713-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="89713-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="89713-135">Response</span></span>
<span data-ttu-id="89713-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="89713-136">Here is an example of the response.</span></span> 
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="89713-137">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="89713-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="89713-138">Языках</span><span class="sxs-lookup"><span data-stu-id="89713-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedlanguages-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89713-139">Язык</span><span class="sxs-lookup"><span data-stu-id="89713-139">Javascript</span></span>](#tab/javascript)
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
