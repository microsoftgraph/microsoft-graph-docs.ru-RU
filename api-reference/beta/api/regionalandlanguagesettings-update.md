---
title: Обновление Регионаландлангуажесеттингс
description: Обновление региональных и языковых параметров пользователя
author: jasonbro
localization_priority: Normal
ms.prod: settings
doc_type: apiPageType
ms.openlocfilehash: 2af80fb6261d04e2aa35a6fe3ea20ce30c63842f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971981"
---
# <a name="update-regionalandlanguagesettings"></a><span data-ttu-id="9c37e-103">Обновление Регионаландлангуажесеттингс</span><span class="sxs-lookup"><span data-stu-id="9c37e-103">Update regionalAndLanguageSettings</span></span>

<span data-ttu-id="9c37e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c37e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c37e-105">Обновление некоторых или всех свойств объекта [регионаландлангуажесеттингс](../resources/regionalAndLanguageSettings.md) .</span><span class="sxs-lookup"><span data-stu-id="9c37e-105">Update some or all of the properties of a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c37e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c37e-106">Permissions</span></span>
<span data-ttu-id="9c37e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c37e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c37e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c37e-109">Permission Type</span></span>                   |<span data-ttu-id="9c37e-110">Разрешение (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="9c37e-110">Permission (from least to most privileged)</span></span>     |
|----------------------------------|---------------------------------------------- |
|<span data-ttu-id="9c37e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c37e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9c37e-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9c37e-112">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="9c37e-113">Делегированная учетная запись (личная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c37e-113">Delegated (personal account)</span></span>      |<span data-ttu-id="9c37e-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9c37e-114">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="9c37e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c37e-115">Application</span></span>                       |<span data-ttu-id="9c37e-116">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9c37e-116">User.ReadWrite, User.ReadWrite.All</span></span>             |

## <a name="http-request"></a><span data-ttu-id="9c37e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c37e-117">HTTP request</span></span>

<span data-ttu-id="9c37e-118">Чтобы обновить региональные и языковые параметры пользователя, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="9c37e-118">To update all of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /settings/regionalAndLanguageSettings
```

<span data-ttu-id="9c37e-119">Обновление подмножества свойств региональных и языковых параметров пользователя:</span><span class="sxs-lookup"><span data-stu-id="9c37e-119">To update a subset of the properties of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /settings/regionalAndLanguageSettings
```

## <a name="request-headers"></a><span data-ttu-id="9c37e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c37e-120">Request headers</span></span>
| <span data-ttu-id="9c37e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c37e-121">Header</span></span>       | <span data-ttu-id="9c37e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9c37e-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="9c37e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c37e-123">Authorization</span></span>  | <span data-ttu-id="9c37e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c37e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9c37e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c37e-126">Content-Type</span></span>  | <span data-ttu-id="9c37e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c37e-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c37e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c37e-129">Request body</span></span>
 <span data-ttu-id="9c37e-130">**Put**: в теле запроса добавьте объект [регионаландлангуажесеттингс](../resources/regionalAndLanguageSettings.md) .</span><span class="sxs-lookup"><span data-stu-id="9c37e-130">**PUT**: In the request body, supply a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>
 
 <span data-ttu-id="9c37e-131">**Patch**: указывайте только значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="9c37e-131">**PATCH**: Only supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9c37e-132">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="9c37e-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9c37e-133">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9c37e-133">For best performance you shouldn't include existing values that haven't changed.</span></span>
 
## <a name="response"></a><span data-ttu-id="9c37e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c37e-134">Response</span></span>

<span data-ttu-id="9c37e-135">В случае успешного выполнения этот метод возвращает код ответа 200 и обновленный объект Регионаландлангуажесеттингс</span><span class="sxs-lookup"><span data-stu-id="9c37e-135">If successful, this method returns a 200 response code and the updated regionalAndLanguageSettings object</span></span>

## <a name="example"></a><span data-ttu-id="9c37e-136">Пример</span><span class="sxs-lookup"><span data-stu-id="9c37e-136">Example</span></span>

### <a name="example-1-update-the-entire-regionalandlanguagesettings-object-of-the-signed-in-user"></a><span data-ttu-id="9c37e-137">Пример 1: обновление всего объекта Регионаландлангуажесеттингс пользователя, выполнившего вход в систему</span><span class="sxs-lookup"><span data-stu-id="9c37e-137">Example 1: Update the entire regionalAndLanguageSettings object of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="9c37e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c37e-138">Request</span></span>

<span data-ttu-id="9c37e-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c37e-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c37e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c37e-140">HTTP</span></span>](#tab/http)
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
    }
}
```
# <a name="c"></a>[<span data-ttu-id="9c37e-141">C#</span><span class="sxs-lookup"><span data-stu-id="9c37e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c37e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c37e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c37e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c37e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="9c37e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c37e-144">Response</span></span>

<span data-ttu-id="9c37e-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9c37e-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "name": "put_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-selected-properties-of-the-signed-in-user"></a><span data-ttu-id="9c37e-146">Пример 2: Обновление выбранных свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="9c37e-146">Example 2: Update selected properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="9c37e-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c37e-147">Request</span></span>

<span data-ttu-id="9c37e-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c37e-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c37e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c37e-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9c37e-150">C#</span><span class="sxs-lookup"><span data-stu-id="9c37e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c37e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c37e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c37e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c37e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="9c37e-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c37e-153">Response</span></span>

<span data-ttu-id="9c37e-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9c37e-154">The following is an example of the response.</span></span>
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


