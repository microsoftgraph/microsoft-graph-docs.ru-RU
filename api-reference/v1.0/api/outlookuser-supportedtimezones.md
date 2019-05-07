---
title: 'outlookUser: supportedTimeZones'
description: Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b77c50e65f4709925a2a2b979ba5828503050352
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611647"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="55e12-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="55e12-103">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="55e12-104">Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="55e12-104">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="55e12-105">Вы можете явно указать, что часовые пояса должны возвращаться в формате часовых поясов Windows или [Администрации адресного пространства Интернета](https://www.iana.org/time-zones) (IANA, другое название — часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="55e12-105">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="55e12-106">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="55e12-106">The Windows format is the default.</span></span>

<span data-ttu-id="55e12-107">Настраивая клиент Outlook, пользователь выбирает часовой пояс из этого списка.</span><span class="sxs-lookup"><span data-stu-id="55e12-107">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="55e12-108">После этого вы можете получить выбранный часовой пояс вместе с [ настройками почтового ящика пользователя](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="55e12-108">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="55e12-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55e12-109">Permissions</span></span>
<span data-ttu-id="55e12-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55e12-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55e12-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55e12-112">Permission type</span></span>      | <span data-ttu-id="55e12-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55e12-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55e12-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55e12-114">Delegated (work or school account)</span></span> | <span data-ttu-id="55e12-115">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="55e12-115">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="55e12-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55e12-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55e12-117">User.Read</span><span class="sxs-lookup"><span data-stu-id="55e12-117">User.Read</span></span>    |
|<span data-ttu-id="55e12-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55e12-118">Application</span></span> | <span data-ttu-id="55e12-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="55e12-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55e12-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55e12-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="55e12-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="55e12-121">Function parameters</span></span>
| <span data-ttu-id="55e12-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="55e12-122">Parameter</span></span>       | <span data-ttu-id="55e12-123">Тип</span><span class="sxs-lookup"><span data-stu-id="55e12-123">Type</span></span> | <span data-ttu-id="55e12-124">Описание</span><span class="sxs-lookup"><span data-stu-id="55e12-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="55e12-125">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="55e12-125">TimeZoneStandard</span></span>  | <span data-ttu-id="55e12-126">Тимезонестандард</span><span class="sxs-lookup"><span data-stu-id="55e12-126">timeZoneStandard</span></span>  | <span data-ttu-id="55e12-127">Формат часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="55e12-127">A time zone format.</span></span> <span data-ttu-id="55e12-128">Поддерживаемые значение: `Windows` и `Iana`.</span><span class="sxs-lookup"><span data-stu-id="55e12-128">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="55e12-129">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="55e12-129">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="55e12-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55e12-130">Request headers</span></span>
| <span data-ttu-id="55e12-131">Имя</span><span class="sxs-lookup"><span data-stu-id="55e12-131">Name</span></span>       | <span data-ttu-id="55e12-132">Тип</span><span class="sxs-lookup"><span data-stu-id="55e12-132">Type</span></span> | <span data-ttu-id="55e12-133">Описание</span><span class="sxs-lookup"><span data-stu-id="55e12-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="55e12-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="55e12-134">Authorization</span></span>  | <span data-ttu-id="55e12-135">string</span><span class="sxs-lookup"><span data-stu-id="55e12-135">string</span></span>  | <span data-ttu-id="55e12-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55e12-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55e12-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55e12-138">Request body</span></span>
<span data-ttu-id="55e12-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55e12-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55e12-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="55e12-140">Response</span></span>
<span data-ttu-id="55e12-141">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [timeZoneInformation](../resources/timezoneinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="55e12-141">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55e12-142">Пример</span><span class="sxs-lookup"><span data-stu-id="55e12-142">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="55e12-143">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="55e12-143">Request 1</span></span>
<span data-ttu-id="55e12-144">В приведенном ниже примере не указывается параметр `timeZoneStandard` и считывается список поддерживаемых часовых поясов, представленных в формате часовых поясов Windows.</span><span class="sxs-lookup"><span data-stu-id="55e12-144">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="55e12-145">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="55e12-145">Response 1</span></span>
<span data-ttu-id="55e12-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55e12-146">Here is an example of the response.</span></span> 
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="55e12-147">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="55e12-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="55e12-148">Языках</span><span class="sxs-lookup"><span data-stu-id="55e12-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55e12-149">Язык</span><span class="sxs-lookup"><span data-stu-id="55e12-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="55e12-150">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="55e12-150">Request 2</span></span>
<span data-ttu-id="55e12-151">В приведенном ниже примере для параметра `TimeZoneStandard` задается значение `Iana` и считывается список поддерживаемых часовых поясов в формате IANA.</span><span class="sxs-lookup"><span data-stu-id="55e12-151">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="55e12-152">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="55e12-152">Response 2</span></span>
<span data-ttu-id="55e12-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="55e12-153">Here is an example of the response.</span></span> 

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="55e12-154">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="55e12-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="55e12-155">Языках</span><span class="sxs-lookup"><span data-stu-id="55e12-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55e12-156">Язык</span><span class="sxs-lookup"><span data-stu-id="55e12-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
