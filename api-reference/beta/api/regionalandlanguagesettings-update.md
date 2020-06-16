---
title: Обновление Регионаландлангуажесеттингс
description: Обновление региональных и языковых параметров пользователя
author: jasonbro
localization_priority: Normal
ms.prod: settings
doc_type: apiPageType
ms.openlocfilehash: c84023c281dcda00db756a80f5d14668d213e727
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744245"
---
# <a name="update-regionalandlanguagesettings"></a><span data-ttu-id="af857-103">Обновление Регионаландлангуажесеттингс</span><span class="sxs-lookup"><span data-stu-id="af857-103">Update regionalAndLanguageSettings</span></span>

<span data-ttu-id="af857-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af857-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af857-105">Обновление некоторых или всех свойств объекта [регионаландлангуажесеттингс](../resources/regionalAndLanguageSettings.md) .</span><span class="sxs-lookup"><span data-stu-id="af857-105">Update some or all of the properties of a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="af857-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af857-106">Permissions</span></span>
<span data-ttu-id="af857-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af857-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af857-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af857-109">Permission Type</span></span>                   |<span data-ttu-id="af857-110">Разрешение (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="af857-110">Permission (from least to most privileged)</span></span>     |
|----------------------------------|---------------------------------------------- |
|<span data-ttu-id="af857-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af857-111">Delegated (work or school account)</span></span>|<span data-ttu-id="af857-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="af857-112">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="af857-113">Делегированная учетная запись (личная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af857-113">Delegated (personal account)</span></span>      |<span data-ttu-id="af857-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="af857-114">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="af857-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af857-115">Application</span></span>                       |<span data-ttu-id="af857-116">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="af857-116">User.ReadWrite, User.ReadWrite.All</span></span>             |

## <a name="http-request"></a><span data-ttu-id="af857-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af857-117">HTTP request</span></span>

<span data-ttu-id="af857-118">Чтобы обновить региональные и языковые параметры пользователя, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="af857-118">To update all of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /settings/regionalAndLanguageSettings
```

<span data-ttu-id="af857-119">Обновление подмножества свойств региональных и языковых параметров пользователя:</span><span class="sxs-lookup"><span data-stu-id="af857-119">To update a subset of the properties of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /settings/regionalAndLanguageSettings
```

## <a name="request-headers"></a><span data-ttu-id="af857-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af857-120">Request headers</span></span>
| <span data-ttu-id="af857-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af857-121">Header</span></span>       | <span data-ttu-id="af857-122">Значение</span><span class="sxs-lookup"><span data-stu-id="af857-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="af857-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af857-123">Authorization</span></span>  | <span data-ttu-id="af857-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af857-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="af857-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af857-126">Content-Type</span></span>  | <span data-ttu-id="af857-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af857-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="af857-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af857-129">Request body</span></span>
 <span data-ttu-id="af857-130">**Put**: в теле запроса добавьте объект [регионаландлангуажесеттингс](../resources/regionalAndLanguageSettings.md) .</span><span class="sxs-lookup"><span data-stu-id="af857-130">**PUT**: In the request body, supply a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>
 
 <span data-ttu-id="af857-131">**Patch**: указывайте только значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="af857-131">**PATCH**: Only supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="af857-132">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="af857-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="af857-133">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="af857-133">For best performance you shouldn't include existing values that haven't changed.</span></span>
 
## <a name="response"></a><span data-ttu-id="af857-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="af857-134">Response</span></span>

<span data-ttu-id="af857-135">В случае успешного выполнения этот метод возвращает код ответа 200 и обновленный объект Регионаландлангуажесеттингс</span><span class="sxs-lookup"><span data-stu-id="af857-135">If successful, this method returns a 200 response code and the updated regionalAndLanguageSettings object</span></span>

## <a name="example"></a><span data-ttu-id="af857-136">Пример</span><span class="sxs-lookup"><span data-stu-id="af857-136">Example</span></span>

### <a name="example-1-update-the-entire-regionalandlanguagesettings-object-of-the-signed-in-user"></a><span data-ttu-id="af857-137">Пример 1: обновление всего объекта Регионаландлангуажесеттингс пользователя, выполнившего вход в систему</span><span class="sxs-lookup"><span data-stu-id="af857-137">Example 1: Update the entire regionalAndLanguageSettings object of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="af857-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="af857-138">Request</span></span>

<span data-ttu-id="af857-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af857-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="af857-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="af857-140">HTTP</span></span>](#tab/http)
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

---

#### <a name="response"></a><span data-ttu-id="af857-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="af857-141">Response</span></span>

<span data-ttu-id="af857-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af857-142">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "name": "put_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-selected-properties-of-the-signed-in-user"></a><span data-ttu-id="af857-143">Пример 2: Обновление выбранных свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="af857-143">Example 2: Update selected properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="af857-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="af857-144">Request</span></span>

<span data-ttu-id="af857-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af857-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="af857-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="af857-146">HTTP</span></span>](#tab/http)
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

---

#### <a name="response"></a><span data-ttu-id="af857-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="af857-147">Response</span></span>

<span data-ttu-id="af857-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="af857-148">The following is an example of the response.</span></span>
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
