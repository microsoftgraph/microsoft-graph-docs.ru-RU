---
title: 'outlookUser: supportedTimeZones'
description: Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 087a79b1765033a68d429339a507d4833a0809b1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274293"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="1029d-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="1029d-103">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="1029d-104">Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="1029d-104">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="1029d-105">Вы можете явно указать, что часовые пояса должны возвращаться в формате часовых поясов Windows или [Администрации адресного пространства Интернета](https://www.iana.org/time-zones) (IANA, другое название — часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="1029d-105">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="1029d-106">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1029d-106">The Windows format is the default.</span></span>

<span data-ttu-id="1029d-107">Настраивая клиент Outlook, пользователь выбирает часовой пояс из этого списка.</span><span class="sxs-lookup"><span data-stu-id="1029d-107">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="1029d-108">После этого вы можете получить выбранный часовой пояс вместе с [ настройками почтового ящика пользователя](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="1029d-108">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="1029d-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1029d-109">Permissions</span></span>
<span data-ttu-id="1029d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1029d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1029d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1029d-112">Permission type</span></span>      | <span data-ttu-id="1029d-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1029d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1029d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1029d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1029d-115">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="1029d-115">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="1029d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1029d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1029d-117">User.Read</span><span class="sxs-lookup"><span data-stu-id="1029d-117">User.Read</span></span>    |
|<span data-ttu-id="1029d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1029d-118">Application</span></span> | <span data-ttu-id="1029d-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1029d-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1029d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1029d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="1029d-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="1029d-121">Function parameters</span></span>
| <span data-ttu-id="1029d-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="1029d-122">Parameter</span></span>       | <span data-ttu-id="1029d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="1029d-123">Type</span></span> | <span data-ttu-id="1029d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1029d-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1029d-125">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="1029d-125">TimeZoneStandard</span></span>  | <span data-ttu-id="1029d-126">Тимезонестандард</span><span class="sxs-lookup"><span data-stu-id="1029d-126">timeZoneStandard</span></span>  | <span data-ttu-id="1029d-127">Формат часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="1029d-127">A time zone format.</span></span> <span data-ttu-id="1029d-128">Поддерживаемые значение: `Windows` и `Iana`.</span><span class="sxs-lookup"><span data-stu-id="1029d-128">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="1029d-129">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="1029d-129">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1029d-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1029d-130">Request headers</span></span>
| <span data-ttu-id="1029d-131">Имя</span><span class="sxs-lookup"><span data-stu-id="1029d-131">Name</span></span>       | <span data-ttu-id="1029d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="1029d-132">Type</span></span> | <span data-ttu-id="1029d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="1029d-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1029d-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="1029d-134">Authorization</span></span>  | <span data-ttu-id="1029d-135">string</span><span class="sxs-lookup"><span data-stu-id="1029d-135">string</span></span>  | <span data-ttu-id="1029d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1029d-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1029d-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1029d-138">Request body</span></span>
<span data-ttu-id="1029d-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1029d-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1029d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1029d-140">Response</span></span>
<span data-ttu-id="1029d-141">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [timeZoneInformation](../resources/timezoneinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1029d-141">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1029d-142">Пример</span><span class="sxs-lookup"><span data-stu-id="1029d-142">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="1029d-143">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="1029d-143">Request 1</span></span>
<span data-ttu-id="1029d-144">В приведенном ниже примере не указывается параметр `timeZoneStandard` и считывается список поддерживаемых часовых поясов, представленных в формате часовых поясов Windows.</span><span class="sxs-lookup"><span data-stu-id="1029d-144">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="1029d-145">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="1029d-145">Response 1</span></span>
<span data-ttu-id="1029d-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1029d-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_default",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Dateline Standard Time",
      "displayName":"(UTC-12:00) International Date Line West"
    },
    {
      "alias":"Samoa Standard Time",
      "displayName":"(UTC+13:00) Samoa"
    },
    {
       "alias":"UTC-11",
       "displayName":"(UTC-11:00) Coordinated Universal Time-11"
    },
    {
      "alias":"Aleutian Standard Time",
      "displayName":"(UTC-10:00) Aleutian Islands"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1029d-147">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="1029d-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1029d-148">C#</span><span class="sxs-lookup"><span data-stu-id="1029d-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1029d-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="1029d-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1029d-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1029d-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="1029d-151">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="1029d-151">Request 2</span></span>
<span data-ttu-id="1029d-152">В приведенном ниже примере для параметра `TimeZoneStandard` задается значение `Iana` и считывается список поддерживаемых часовых поясов в формате IANA.</span><span class="sxs-lookup"><span data-stu-id="1029d-152">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="1029d-153">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="1029d-153">Response 2</span></span>
<span data-ttu-id="1029d-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1029d-154">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_iana",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Etc/GMT+12",
      "displayName":"Etc/GMT+12"
    },
    {
      "alias":"US/Samoa",
      "displayName":"US/Samoa"
    },
    {
      "alias":"Etc/GMT+11",
      "displayName":"Etc/GMT+11"
    },
    {
      "alias":"US/Aleutian",
      "displayName":"US/Aleutian"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1029d-155">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="1029d-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1029d-156">C#</span><span class="sxs-lookup"><span data-stu-id="1029d-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1029d-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="1029d-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1029d-158">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1029d-158">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
