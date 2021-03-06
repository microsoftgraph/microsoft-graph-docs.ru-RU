---
title: Получить ресурс regionalAndLanguageSettings
description: Извлечение свойств региональных свойств пользователяAndLanguageSettings
author: jasonbro
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 6bd4f758a2e7b0113ba6da5eb04b1823171986b8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516635"
---
# <a name="get-regionalandlanguagesettings"></a><span data-ttu-id="4bc6d-103">Get regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="4bc6d-103">Get regionalAndLanguageSettings</span></span>

<span data-ttu-id="4bc6d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bc6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bc6d-105">Получите свойства объекта [regionalAndLanguageSettings.](../resources/regionalAndLanguageSettings.md)</span><span class="sxs-lookup"><span data-stu-id="4bc6d-105">Get the properties of a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bc6d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4bc6d-106">Permissions</span></span>
<span data-ttu-id="4bc6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bc6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bc6d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bc6d-109">Permission Type</span></span>                   |<span data-ttu-id="4bc6d-110">Разрешение (от наименее до самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="4bc6d-110">Permission (from least to most privileged)</span></span>     |
|----------------------------------|---------------------------------------------- |
|<span data-ttu-id="4bc6d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bc6d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4bc6d-112">User.Read, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bc6d-112">User.Read, User.Read.All</span></span>                        |
|<span data-ttu-id="4bc6d-113">Делегированная (личная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bc6d-113">Delegated (personal account)</span></span>      |<span data-ttu-id="4bc6d-114">User.Read, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bc6d-114">User.Read, User.Read.All</span></span>              |
|<span data-ttu-id="4bc6d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4bc6d-115">Application</span></span>                       |<span data-ttu-id="4bc6d-116">User.Read, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bc6d-116">User.Read, User.Read.All</span></span>              |

## <a name="http-request"></a><span data-ttu-id="4bc6d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bc6d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /settings/regionalAndLanguageSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4bc6d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4bc6d-118">Optional query parameters</span></span>
<span data-ttu-id="4bc6d-119">Вы можете использовать `$select` для получения определенных региональных свойствAndLanguageSettings, включая те, которые не возвращаются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4bc6d-119">You can use `$select` to get specific regionalAndLanguageSettings properties, including those that are not returned by default.</span></span>

<span data-ttu-id="4bc6d-120">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4bc6d-120">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4bc6d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bc6d-121">Request headers</span></span>
| <span data-ttu-id="4bc6d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4bc6d-122">Header</span></span>       | <span data-ttu-id="4bc6d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4bc6d-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="4bc6d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4bc6d-124">Authorization</span></span>  | <span data-ttu-id="4bc6d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bc6d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bc6d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bc6d-127">Request body</span></span>
<span data-ttu-id="4bc6d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4bc6d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bc6d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bc6d-129">Response</span></span>

<span data-ttu-id="4bc6d-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4bc6d-130">If successful, this method returns a `200 OK` response code and [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bc6d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4bc6d-131">Example</span></span>

<span data-ttu-id="4bc6d-132">В следующем примере получаются свойства пользователя, вписаного в него.</span><span class="sxs-lookup"><span data-stu-id="4bc6d-132">The following example gets the properties of the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="4bc6d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bc6d-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4bc6d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bc6d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_regionalAndLanguageSettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/settings/regionalAndLanguageSettings
```
# <a name="c"></a>[<span data-ttu-id="4bc6d-135">C#</span><span class="sxs-lookup"><span data-stu-id="4bc6d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4bc6d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bc6d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4bc6d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4bc6d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4bc6d-138">Java</span><span class="sxs-lookup"><span data-stu-id="4bc6d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-regionalandlanguagesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4bc6d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bc6d-139">Response</span></span>

><span data-ttu-id="4bc6d-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4bc6d-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "name": "get_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "defaultDisplayLanguage": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "authoringLanguages": [
        {
            "locale": "fr-FR",
            "displayName": "French (France)"
        },
        {
            "locale": "de-DE",
            "displayName": "German (Germany)"
        },
    ],
    "defaultTranslationLanguage": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "defaultSpeechInputLanguage": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "defaultRegionalFormat": {
        "locale": "en-GB",
        "displayName": "English (United Kingdom)"
    },
    "regionalFormatOverrides": {
        "calendar": "Gregorian Calendar",
        "firstDayOfWeek": "Sunday",
        "shortDateFormat": "yyyy-MM-dd",
        "longDateFormat": "dddd, MMMM d, yyyy",
        "shortTimeFormat": "HH:mm",
        "longTimeFormat": "h:mm:ss tt",
        "timeZone": "Pacific Standard Time"
    },
    "translationPreferences": {
        "translationBehavior": "Yes",
        "languageOverrides": [
            {
                "languageTag": "fr",
                "translationBehavior": "Yes" 
            }
        ],
        "untranslatedLanguages": ["de"]
     }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get regionalAndLanguageSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


