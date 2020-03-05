---
title: 'outlookUser: supportedTimeZones'
description: Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 94b6f49ce30e454d1d4c523e402c93166f59c4cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456035"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="bbf46-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="bbf46-103">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="bbf46-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bbf46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbf46-105">Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="bbf46-105">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="bbf46-106">Вы можете явно указать, что часовые пояса должны возвращаться в формате часовых поясов Windows или [Администрации адресного пространства Интернета](https://www.iana.org/time-zones) (IANA, другое название — часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="bbf46-106">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="bbf46-107">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bbf46-107">The Windows format is the default.</span></span>

<span data-ttu-id="bbf46-108">Настраивая клиент Outlook, пользователь выбирает часовой пояс из этого списка.</span><span class="sxs-lookup"><span data-stu-id="bbf46-108">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="bbf46-109">После этого вы можете получить выбранный часовой пояс вместе с [ настройками почтового ящика пользователя](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="bbf46-109">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="bbf46-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbf46-110">Permissions</span></span>
<span data-ttu-id="bbf46-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbf46-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbf46-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbf46-113">Permission type</span></span>      | <span data-ttu-id="bbf46-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbf46-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbf46-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbf46-115">Delegated (work or school account)</span></span> | <span data-ttu-id="bbf46-116">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="bbf46-116">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="bbf46-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbf46-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbf46-118">User.Read</span><span class="sxs-lookup"><span data-stu-id="bbf46-118">User.Read</span></span>    |
|<span data-ttu-id="bbf46-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbf46-119">Application</span></span> | <span data-ttu-id="bbf46-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf46-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbf46-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbf46-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="bbf46-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="bbf46-122">Function parameters</span></span>
| <span data-ttu-id="bbf46-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="bbf46-123">Parameter</span></span>      | <span data-ttu-id="bbf46-124">Тип</span><span class="sxs-lookup"><span data-stu-id="bbf46-124">Type</span></span>    | <span data-ttu-id="bbf46-125">Описание</span><span class="sxs-lookup"><span data-stu-id="bbf46-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bbf46-126">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="bbf46-126">TimeZoneStandard</span></span>  | <span data-ttu-id="bbf46-127">Строка</span><span class="sxs-lookup"><span data-stu-id="bbf46-127">String</span></span>  | <span data-ttu-id="bbf46-128">Формат часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="bbf46-128">A time zone format.</span></span> <span data-ttu-id="bbf46-129">Поддерживаемые значение: `Windows` и `Iana`.</span><span class="sxs-lookup"><span data-stu-id="bbf46-129">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="bbf46-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bbf46-130">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="bbf46-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbf46-131">Request headers</span></span>
| <span data-ttu-id="bbf46-132">Имя</span><span class="sxs-lookup"><span data-stu-id="bbf46-132">Name</span></span>       | <span data-ttu-id="bbf46-133">Тип</span><span class="sxs-lookup"><span data-stu-id="bbf46-133">Type</span></span> | <span data-ttu-id="bbf46-134">Описание</span><span class="sxs-lookup"><span data-stu-id="bbf46-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bbf46-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbf46-135">Authorization</span></span>  | <span data-ttu-id="bbf46-136">string</span><span class="sxs-lookup"><span data-stu-id="bbf46-136">string</span></span>  | <span data-ttu-id="bbf46-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbf46-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbf46-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bbf46-139">Request body</span></span>
<span data-ttu-id="bbf46-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bbf46-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbf46-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbf46-141">Response</span></span>
<span data-ttu-id="bbf46-142">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [timeZoneInformation](../resources/timezoneinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bbf46-142">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbf46-143">Пример</span><span class="sxs-lookup"><span data-stu-id="bbf46-143">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="bbf46-144">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="bbf46-144">Request 1</span></span>
<span data-ttu-id="bbf46-145">В приведенном ниже примере не указывается параметр `timeZoneStandard` и считывается список поддерживаемых часовых поясов, представленных в формате часовых поясов Windows.</span><span class="sxs-lookup"><span data-stu-id="bbf46-145">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 

# <a name="http"></a>[<span data-ttu-id="bbf46-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf46-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones
```
# <a name="c"></a>[<span data-ttu-id="bbf46-147">C#</span><span class="sxs-lookup"><span data-stu-id="bbf46-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbf46-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbf46-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbf46-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbf46-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="bbf46-150">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="bbf46-150">Response 1</span></span>
<span data-ttu-id="bbf46-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bbf46-151">Here is an example of the response.</span></span> 
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
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

##### <a name="request-2"></a><span data-ttu-id="bbf46-152">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="bbf46-152">Request 2</span></span>
<span data-ttu-id="bbf46-153">В приведенном ниже примере для параметра `TimeZoneStandard` задается значение `Iana` и считывается список поддерживаемых часовых поясов в формате IANA.</span><span class="sxs-lookup"><span data-stu-id="bbf46-153">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 


# <a name="http"></a>[<span data-ttu-id="bbf46-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf46-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```
# <a name="c"></a>[<span data-ttu-id="bbf46-155">C#</span><span class="sxs-lookup"><span data-stu-id="bbf46-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-iana-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbf46-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbf46-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-iana-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbf46-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbf46-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-iana-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="bbf46-158">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="bbf46-158">Response 2</span></span>
<span data-ttu-id="bbf46-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bbf46-159">Here is an example of the response.</span></span> 

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
