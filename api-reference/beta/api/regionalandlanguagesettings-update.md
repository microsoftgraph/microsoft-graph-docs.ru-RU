---
title: Обновление regionalAndLanguageSettings
description: Обновление региональных и языковых параметров пользователя.
author: jasonbro
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 82f33ae2b4165586ccb4a3d55873e1e6ff6c1765
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516621"
---
# <a name="update-regionalandlanguagesettings"></a><span data-ttu-id="0a89f-103">Обновление regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="0a89f-103">Update regionalAndLanguageSettings</span></span>

<span data-ttu-id="0a89f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a89f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a89f-105">Обновим некоторые или все свойства объекта [regionalAndLanguageSettings.](../resources/regionalAndLanguageSettings.md)</span><span class="sxs-lookup"><span data-stu-id="0a89f-105">Update some or all of the properties of a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a89f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a89f-106">Permissions</span></span>
<span data-ttu-id="0a89f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a89f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a89f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a89f-109">Permission Type</span></span>                   |<span data-ttu-id="0a89f-110">Разрешение (от наименее до самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="0a89f-110">Permission (from least to most privileged)</span></span>     |
|----------------------------------|---------------------------------------------- |
|<span data-ttu-id="0a89f-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a89f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0a89f-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a89f-112">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="0a89f-113">Делегированная (личная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a89f-113">Delegated (personal account)</span></span>      |<span data-ttu-id="0a89f-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a89f-114">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="0a89f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0a89f-115">Application</span></span>                       |<span data-ttu-id="0a89f-116">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a89f-116">User.ReadWrite, User.ReadWrite.All</span></span>             |

## <a name="http-request"></a><span data-ttu-id="0a89f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a89f-117">HTTP request</span></span>

<span data-ttu-id="0a89f-118">Обновление всех региональных и языковых параметров пользователя:</span><span class="sxs-lookup"><span data-stu-id="0a89f-118">To update all of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /settings/regionalAndLanguageSettings
```

<span data-ttu-id="0a89f-119">Обновление подмножество свойств региональных и языковых параметров пользователя:</span><span class="sxs-lookup"><span data-stu-id="0a89f-119">To update a subset of the properties of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /settings/regionalAndLanguageSettings
```

## <a name="request-headers"></a><span data-ttu-id="0a89f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a89f-120">Request headers</span></span>
| <span data-ttu-id="0a89f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a89f-121">Header</span></span>       | <span data-ttu-id="0a89f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0a89f-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="0a89f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a89f-123">Authorization</span></span>  | <span data-ttu-id="0a89f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a89f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0a89f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a89f-126">Content-Type</span></span>  | <span data-ttu-id="0a89f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a89f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a89f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a89f-129">Request body</span></span>
 <span data-ttu-id="0a89f-130">**PUT.** В теле запроса поставьте [объект regionalAndLanguageSettings.](../resources/regionalAndLanguageSettings.md)</span><span class="sxs-lookup"><span data-stu-id="0a89f-130">**PUT**: In the request body, supply a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>
 
 <span data-ttu-id="0a89f-131">**PATCH.** Только поставляем значения для соответствующих полей, которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="0a89f-131">**PATCH**: Only supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0a89f-132">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0a89f-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0a89f-133">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0a89f-133">For best performance you shouldn't include existing values that haven't changed.</span></span>
 
## <a name="response"></a><span data-ttu-id="0a89f-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a89f-134">Response</span></span>

<span data-ttu-id="0a89f-135">В случае успеха этот метод возвращает код ответа 200 и обновленный **объект regionalAndLanguageSettings.**</span><span class="sxs-lookup"><span data-stu-id="0a89f-135">If successful, this method returns a 200 response code and the updated **regionalAndLanguageSettings** object.</span></span>

## <a name="example"></a><span data-ttu-id="0a89f-136">Пример</span><span class="sxs-lookup"><span data-stu-id="0a89f-136">Example</span></span>

### <a name="example-1-update-the-entire-regionalandlanguagesettings-object-of-the-signed-in-user"></a><span data-ttu-id="0a89f-137">Пример 1. Обновление всего объекта regionalAndLanguageSettings для подписанного пользователя</span><span class="sxs-lookup"><span data-stu-id="0a89f-137">Example 1: Update the entire regionalAndLanguageSettings object of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="0a89f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a89f-138">Request</span></span>

<span data-ttu-id="0a89f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a89f-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a89f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a89f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_regionalAndLanguageSettings"
}-->
```http
PUT https://graph.microsoft.com/beta/me/settings/regionalandlanguagesettings
Content-type: application/json

{
    "defaultDisplayLanguage": {
        "locale": "en-US"
    },
    "authoringLanguages": [
        {
            "locale": "fr-FR"
        },
        {
            "locale": "de-DE"
        }
    ],
    "defaultTranslationLanguage": {
        "locale": "en-US"
    },
    "defaultSpeechInputLanguage": {
        "locale": "en-US"
    },
    "defaultRegionalFormat": {
        "locale": "en-GB"
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
        ]
     }
}
```
# <a name="c"></a>[<span data-ttu-id="0a89f-141">C#</span><span class="sxs-lookup"><span data-stu-id="0a89f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a89f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a89f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a89f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a89f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a89f-144">Java</span><span class="sxs-lookup"><span data-stu-id="0a89f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-regionalandlanguagesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="0a89f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a89f-145">Response</span></span>

<span data-ttu-id="0a89f-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a89f-146">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "name": "put_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-selected-properties-of-the-signed-in-user"></a><span data-ttu-id="0a89f-147">Пример 2. Обновление выбранных свойств подписанного пользователя</span><span class="sxs-lookup"><span data-stu-id="0a89f-147">Example 2: Update selected properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="0a89f-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a89f-148">Request</span></span>

<span data-ttu-id="0a89f-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a89f-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a89f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a89f-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_regionalAndLanguageSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/settings/regionalandlanguagesettings
Content-type: application/json

{
  "authoringLanguages": [
    {
     "locale": "en-US" },
    {
     "locale": "es-MX" }
  ],
  "defaultRegionalFormat": {
     "locale": "en-US"
   }
}
```
# <a name="c"></a>[<span data-ttu-id="0a89f-151">C#</span><span class="sxs-lookup"><span data-stu-id="0a89f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a89f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a89f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a89f-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a89f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a89f-154">Java</span><span class="sxs-lookup"><span data-stu-id="0a89f-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-regionalandlanguagesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="0a89f-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a89f-155">Response</span></span>

<span data-ttu-id="0a89f-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0a89f-156">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "name": "patch_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Update regionalAndLanguageSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


