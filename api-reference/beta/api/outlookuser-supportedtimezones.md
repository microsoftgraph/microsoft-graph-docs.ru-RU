---
title: 'outlookUser: supportedTimeZones'
description: Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9a6e536c5eec85057a6c0788e282164a3bf24ee2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128675"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="14fd7-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="14fd7-103">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="14fd7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14fd7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14fd7-105">Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="14fd7-105">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="14fd7-106">Вы можете явно указать, что часовые пояса должны возвращаться в формате часовых поясов Windows или [Администрации адресного пространства Интернета](https://www.iana.org/time-zones) (IANA, другое название — часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="14fd7-106">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="14fd7-107">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="14fd7-107">The Windows format is the default.</span></span>

<span data-ttu-id="14fd7-108">Настраивая клиент Outlook, пользователь выбирает часовой пояс из этого списка.</span><span class="sxs-lookup"><span data-stu-id="14fd7-108">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="14fd7-109">После этого вы можете получить выбранный часовой пояс вместе с [ настройками почтового ящика пользователя](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="14fd7-109">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="14fd7-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14fd7-110">Permissions</span></span>
<span data-ttu-id="14fd7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14fd7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14fd7-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14fd7-113">Permission type</span></span>      | <span data-ttu-id="14fd7-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14fd7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14fd7-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14fd7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="14fd7-116">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="14fd7-116">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="14fd7-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14fd7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14fd7-118">User.Read</span><span class="sxs-lookup"><span data-stu-id="14fd7-118">User.Read</span></span>    |
|<span data-ttu-id="14fd7-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14fd7-119">Application</span></span> | <span data-ttu-id="14fd7-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="14fd7-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14fd7-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14fd7-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="14fd7-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="14fd7-122">Function parameters</span></span>
| <span data-ttu-id="14fd7-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="14fd7-123">Parameter</span></span>      | <span data-ttu-id="14fd7-124">Тип</span><span class="sxs-lookup"><span data-stu-id="14fd7-124">Type</span></span>    | <span data-ttu-id="14fd7-125">Описание</span><span class="sxs-lookup"><span data-stu-id="14fd7-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="14fd7-126">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="14fd7-126">TimeZoneStandard</span></span>  | <span data-ttu-id="14fd7-127">Строка</span><span class="sxs-lookup"><span data-stu-id="14fd7-127">String</span></span>  | <span data-ttu-id="14fd7-128">Формат часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="14fd7-128">A time zone format.</span></span> <span data-ttu-id="14fd7-129">Поддерживаемые значение: `Windows` и `Iana`.</span><span class="sxs-lookup"><span data-stu-id="14fd7-129">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="14fd7-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="14fd7-130">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="14fd7-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14fd7-131">Request headers</span></span>
| <span data-ttu-id="14fd7-132">Имя</span><span class="sxs-lookup"><span data-stu-id="14fd7-132">Name</span></span>       | <span data-ttu-id="14fd7-133">Тип</span><span class="sxs-lookup"><span data-stu-id="14fd7-133">Type</span></span> | <span data-ttu-id="14fd7-134">Описание</span><span class="sxs-lookup"><span data-stu-id="14fd7-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="14fd7-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="14fd7-135">Authorization</span></span>  | <span data-ttu-id="14fd7-136">string</span><span class="sxs-lookup"><span data-stu-id="14fd7-136">string</span></span>  | <span data-ttu-id="14fd7-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14fd7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14fd7-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14fd7-139">Request body</span></span>
<span data-ttu-id="14fd7-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14fd7-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14fd7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="14fd7-141">Response</span></span>
<span data-ttu-id="14fd7-142">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [timeZoneInformation](../resources/timezoneinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="14fd7-142">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14fd7-143">Пример</span><span class="sxs-lookup"><span data-stu-id="14fd7-143">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="14fd7-144">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="14fd7-144">Request 1</span></span>
<span data-ttu-id="14fd7-145">В приведенном ниже примере не указывается параметр `timeZoneStandard` и считывается список поддерживаемых часовых поясов, представленных в формате часовых поясов Windows.</span><span class="sxs-lookup"><span data-stu-id="14fd7-145">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 

# <a name="http"></a>[<span data-ttu-id="14fd7-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="14fd7-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones
```
# <a name="c"></a>[<span data-ttu-id="14fd7-147">C#</span><span class="sxs-lookup"><span data-stu-id="14fd7-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14fd7-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14fd7-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14fd7-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14fd7-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14fd7-150">Java</span><span class="sxs-lookup"><span data-stu-id="14fd7-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="14fd7-151">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="14fd7-151">Response 1</span></span>
<span data-ttu-id="14fd7-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="14fd7-152">Here is an example of the response.</span></span> 
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

##### <a name="request-2"></a><span data-ttu-id="14fd7-153">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="14fd7-153">Request 2</span></span>
<span data-ttu-id="14fd7-154">В приведенном ниже примере для параметра `TimeZoneStandard` задается значение `Iana` и считывается список поддерживаемых часовых поясов в формате IANA.</span><span class="sxs-lookup"><span data-stu-id="14fd7-154">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 


# <a name="http"></a>[<span data-ttu-id="14fd7-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="14fd7-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```
# <a name="c"></a>[<span data-ttu-id="14fd7-156">C#</span><span class="sxs-lookup"><span data-stu-id="14fd7-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-iana-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14fd7-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14fd7-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-iana-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14fd7-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14fd7-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-iana-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14fd7-159">Java</span><span class="sxs-lookup"><span data-stu-id="14fd7-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-iana-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="14fd7-160">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="14fd7-160">Response 2</span></span>
<span data-ttu-id="14fd7-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="14fd7-161">Here is an example of the response.</span></span> 

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


