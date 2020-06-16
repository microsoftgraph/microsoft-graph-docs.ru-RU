---
title: Получение ресурса Регионаландлангуажесеттингс
description: Получение свойств объекта Регионаландлангуажесеттингс пользователя
author: jasonbro
localization_priority: Normal
ms.prod: settings
doc_type: apiPageType
ms.openlocfilehash: 493af1c75e20552e9fb420402365894a04717e17
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744242"
---
# <a name="get-regionalandlanguagesettings"></a><span data-ttu-id="586a0-103">Получение Регионаландлангуажесеттингс</span><span class="sxs-lookup"><span data-stu-id="586a0-103">Get regionalAndLanguageSettings</span></span>

<span data-ttu-id="586a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="586a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="586a0-105">Получение свойств объекта [регионаландлангуажесеттингс](../resources/regionalAndLanguageSettings.md) .</span><span class="sxs-lookup"><span data-stu-id="586a0-105">Get the properties of a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="586a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="586a0-106">Permissions</span></span>
<span data-ttu-id="586a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="586a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="586a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="586a0-109">Permission Type</span></span>                   |<span data-ttu-id="586a0-110">Разрешение (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="586a0-110">Permission (from least to most privileged)</span></span>     |
|----------------------------------|---------------------------------------------- |
|<span data-ttu-id="586a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="586a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="586a0-112">User. Read, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="586a0-112">User.Read, User.Read.All</span></span>                        |
|<span data-ttu-id="586a0-113">Делегированная учетная запись (личная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="586a0-113">Delegated (personal account)</span></span>      |<span data-ttu-id="586a0-114">User. Read, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="586a0-114">User.Read, User.Read.All</span></span>              |
|<span data-ttu-id="586a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="586a0-115">Application</span></span>                       |<span data-ttu-id="586a0-116">User. Read, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="586a0-116">User.Read, User.Read.All</span></span>              |

## <a name="http-request"></a><span data-ttu-id="586a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="586a0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /settings/regionalAndLanguageSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="586a0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="586a0-118">Optional query parameters</span></span>
<span data-ttu-id="586a0-119">Вы можете использовать `$select` для получения определенных свойств регионаландлангуажесеттингс, включая те, которые не возвращаются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="586a0-119">You can use `$select` to get specific regionalAndLanguageSettings properties, including those that are not returned by default.</span></span>

<span data-ttu-id="586a0-120">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="586a0-120">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="586a0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="586a0-121">Request headers</span></span>
| <span data-ttu-id="586a0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="586a0-122">Header</span></span>       | <span data-ttu-id="586a0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="586a0-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="586a0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="586a0-124">Authorization</span></span>  | <span data-ttu-id="586a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="586a0-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="586a0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="586a0-127">Content-Type</span></span>   | <span data-ttu-id="586a0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="586a0-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="586a0-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="586a0-129">Request body</span></span>
<span data-ttu-id="586a0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="586a0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="586a0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="586a0-131">Response</span></span>

<span data-ttu-id="586a0-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [регионаландлангуажесеттингс](../resources/regionalandlanguagesettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="586a0-132">If successful, this method returns a `200 OK` response code and [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="586a0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="586a0-133">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="586a0-134">Пример 1. Получение свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="586a0-134">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="586a0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="586a0-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="586a0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="586a0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_regionalAndLanguageSettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/settings/regionalAndLanguageSettings
```

##### <a name="response"></a><span data-ttu-id="586a0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="586a0-137">Response</span></span>
<span data-ttu-id="586a0-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="586a0-138">Here is an example of the response.</span></span> <span data-ttu-id="586a0-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="586a0-139">Note: The response object shown here may be truncated for brevity.</span></span> 

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
