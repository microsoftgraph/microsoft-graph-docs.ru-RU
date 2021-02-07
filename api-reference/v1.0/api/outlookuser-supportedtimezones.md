---
title: 'outlookUser: supportedTimeZones'
description: Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 53bdd461051f2a137c0a9b04b82a0d9acc254065
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128304"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="10bf5-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="10bf5-103">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="10bf5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10bf5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10bf5-105">Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="10bf5-105">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="10bf5-106">Вы можете явно указать, что часовые пояса должны возвращаться в формате часовых поясов Windows или [Администрации адресного пространства Интернета](https://www.iana.org/time-zones) (IANA, другое название — часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="10bf5-106">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="10bf5-107">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="10bf5-107">The Windows format is the default.</span></span>

<span data-ttu-id="10bf5-108">Настраивая клиент Outlook, пользователь выбирает часовой пояс из этого списка.</span><span class="sxs-lookup"><span data-stu-id="10bf5-108">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="10bf5-109">После этого вы можете получить выбранный часовой пояс вместе с [ настройками почтового ящика пользователя](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="10bf5-109">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="10bf5-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10bf5-110">Permissions</span></span>
<span data-ttu-id="10bf5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10bf5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10bf5-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10bf5-113">Permission type</span></span>      | <span data-ttu-id="10bf5-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10bf5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10bf5-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10bf5-115">Delegated (work or school account)</span></span> | <span data-ttu-id="10bf5-116">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="10bf5-116">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="10bf5-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10bf5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10bf5-118">User.Read</span><span class="sxs-lookup"><span data-stu-id="10bf5-118">User.Read</span></span>    |
|<span data-ttu-id="10bf5-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10bf5-119">Application</span></span> | <span data-ttu-id="10bf5-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="10bf5-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10bf5-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10bf5-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="10bf5-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="10bf5-122">Function parameters</span></span>
| <span data-ttu-id="10bf5-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="10bf5-123">Parameter</span></span>       | <span data-ttu-id="10bf5-124">Тип</span><span class="sxs-lookup"><span data-stu-id="10bf5-124">Type</span></span> | <span data-ttu-id="10bf5-125">Описание</span><span class="sxs-lookup"><span data-stu-id="10bf5-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="10bf5-126">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="10bf5-126">TimeZoneStandard</span></span>  | <span data-ttu-id="10bf5-127">timeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="10bf5-127">timeZoneStandard</span></span>  | <span data-ttu-id="10bf5-128">Формат часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="10bf5-128">A time zone format.</span></span> <span data-ttu-id="10bf5-129">Поддерживаемые значение: `Windows` и `Iana`.</span><span class="sxs-lookup"><span data-stu-id="10bf5-129">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="10bf5-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="10bf5-130">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="10bf5-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10bf5-131">Request headers</span></span>
| <span data-ttu-id="10bf5-132">Имя</span><span class="sxs-lookup"><span data-stu-id="10bf5-132">Name</span></span>       | <span data-ttu-id="10bf5-133">Тип</span><span class="sxs-lookup"><span data-stu-id="10bf5-133">Type</span></span> | <span data-ttu-id="10bf5-134">Описание</span><span class="sxs-lookup"><span data-stu-id="10bf5-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="10bf5-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="10bf5-135">Authorization</span></span>  | <span data-ttu-id="10bf5-136">string</span><span class="sxs-lookup"><span data-stu-id="10bf5-136">string</span></span>  | <span data-ttu-id="10bf5-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10bf5-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10bf5-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10bf5-139">Request body</span></span>
<span data-ttu-id="10bf5-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10bf5-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10bf5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="10bf5-141">Response</span></span>
<span data-ttu-id="10bf5-142">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [timeZoneInformation](../resources/timezoneinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="10bf5-142">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10bf5-143">Пример</span><span class="sxs-lookup"><span data-stu-id="10bf5-143">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="10bf5-144">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="10bf5-144">Request 1</span></span>
<span data-ttu-id="10bf5-145">В приведенном ниже примере не указывается параметр `timeZoneStandard` и считывается список поддерживаемых часовых поясов, представленных в формате часовых поясов Windows.</span><span class="sxs-lookup"><span data-stu-id="10bf5-145">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 

# <a name="http"></a>[<span data-ttu-id="10bf5-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="10bf5-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones
```
# <a name="c"></a>[<span data-ttu-id="10bf5-147">C#</span><span class="sxs-lookup"><span data-stu-id="10bf5-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10bf5-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10bf5-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10bf5-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10bf5-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10bf5-150">Java</span><span class="sxs-lookup"><span data-stu-id="10bf5-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="10bf5-151">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="10bf5-151">Response 1</span></span>
<span data-ttu-id="10bf5-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="10bf5-152">Here is an example of the response.</span></span> 
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

##### <a name="request-2"></a><span data-ttu-id="10bf5-153">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="10bf5-153">Request 2</span></span>
<span data-ttu-id="10bf5-154">В приведенном ниже примере для параметра `TimeZoneStandard` задается значение `Iana` и считывается список поддерживаемых часовых поясов в формате IANA.</span><span class="sxs-lookup"><span data-stu-id="10bf5-154">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 


# <a name="http"></a>[<span data-ttu-id="10bf5-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="10bf5-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```
# <a name="c"></a>[<span data-ttu-id="10bf5-156">C#</span><span class="sxs-lookup"><span data-stu-id="10bf5-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-iana-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10bf5-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10bf5-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-iana-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10bf5-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10bf5-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-iana-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10bf5-159">Java</span><span class="sxs-lookup"><span data-stu-id="10bf5-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-iana-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="10bf5-160">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="10bf5-160">Response 2</span></span>
<span data-ttu-id="10bf5-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10bf5-161">Here is an example of the response.</span></span> 

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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

