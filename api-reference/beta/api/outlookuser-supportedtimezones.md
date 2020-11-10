---
title: 'outlookUser: supportedTimeZones'
description: Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 81c605b678bb4de28d924bf64cab998d7f0f465e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964459"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="6caec-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="6caec-103">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="6caec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6caec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6caec-105">Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="6caec-105">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="6caec-106">Вы можете явно указать, что часовые пояса должны возвращаться в формате часовых поясов Windows или [Администрации адресного пространства Интернета](https://www.iana.org/time-zones) (IANA, другое название — часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="6caec-106">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="6caec-107">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6caec-107">The Windows format is the default.</span></span>

<span data-ttu-id="6caec-108">Настраивая клиент Outlook, пользователь выбирает часовой пояс из этого списка.</span><span class="sxs-lookup"><span data-stu-id="6caec-108">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="6caec-109">После этого вы можете получить выбранный часовой пояс вместе с [ настройками почтового ящика пользователя](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="6caec-109">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="6caec-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6caec-110">Permissions</span></span>
<span data-ttu-id="6caec-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6caec-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6caec-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6caec-113">Permission type</span></span>      | <span data-ttu-id="6caec-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6caec-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6caec-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6caec-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6caec-116">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="6caec-116">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="6caec-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6caec-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6caec-118">User.Read</span><span class="sxs-lookup"><span data-stu-id="6caec-118">User.Read</span></span>    |
|<span data-ttu-id="6caec-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6caec-119">Application</span></span> | <span data-ttu-id="6caec-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6caec-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6caec-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6caec-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="6caec-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6caec-122">Function parameters</span></span>
| <span data-ttu-id="6caec-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="6caec-123">Parameter</span></span>      | <span data-ttu-id="6caec-124">Тип</span><span class="sxs-lookup"><span data-stu-id="6caec-124">Type</span></span>    | <span data-ttu-id="6caec-125">Описание</span><span class="sxs-lookup"><span data-stu-id="6caec-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6caec-126">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="6caec-126">TimeZoneStandard</span></span>  | <span data-ttu-id="6caec-127">Строка</span><span class="sxs-lookup"><span data-stu-id="6caec-127">String</span></span>  | <span data-ttu-id="6caec-128">Формат часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="6caec-128">A time zone format.</span></span> <span data-ttu-id="6caec-129">Поддерживаемые значение: `Windows` и `Iana`.</span><span class="sxs-lookup"><span data-stu-id="6caec-129">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="6caec-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6caec-130">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6caec-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6caec-131">Request headers</span></span>
| <span data-ttu-id="6caec-132">Имя</span><span class="sxs-lookup"><span data-stu-id="6caec-132">Name</span></span>       | <span data-ttu-id="6caec-133">Тип</span><span class="sxs-lookup"><span data-stu-id="6caec-133">Type</span></span> | <span data-ttu-id="6caec-134">Описание</span><span class="sxs-lookup"><span data-stu-id="6caec-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6caec-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="6caec-135">Authorization</span></span>  | <span data-ttu-id="6caec-136">string</span><span class="sxs-lookup"><span data-stu-id="6caec-136">string</span></span>  | <span data-ttu-id="6caec-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6caec-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6caec-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6caec-139">Request body</span></span>
<span data-ttu-id="6caec-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6caec-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6caec-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6caec-141">Response</span></span>
<span data-ttu-id="6caec-142">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [timeZoneInformation](../resources/timezoneinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6caec-142">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6caec-143">Пример</span><span class="sxs-lookup"><span data-stu-id="6caec-143">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="6caec-144">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="6caec-144">Request 1</span></span>
<span data-ttu-id="6caec-145">В приведенном ниже примере не указывается параметр `timeZoneStandard` и считывается список поддерживаемых часовых поясов, представленных в формате часовых поясов Windows.</span><span class="sxs-lookup"><span data-stu-id="6caec-145">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 

# <a name="http"></a>[<span data-ttu-id="6caec-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="6caec-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones
```
# <a name="c"></a>[<span data-ttu-id="6caec-147">C#</span><span class="sxs-lookup"><span data-stu-id="6caec-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6caec-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6caec-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6caec-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6caec-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6caec-150">Java</span><span class="sxs-lookup"><span data-stu-id="6caec-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="6caec-151">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="6caec-151">Response 1</span></span>
<span data-ttu-id="6caec-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6caec-152">Here is an example of the response.</span></span> 
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

##### <a name="request-2"></a><span data-ttu-id="6caec-153">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="6caec-153">Request 2</span></span>
<span data-ttu-id="6caec-154">В приведенном ниже примере для параметра `TimeZoneStandard` задается значение `Iana` и считывается список поддерживаемых часовых поясов в формате IANA.</span><span class="sxs-lookup"><span data-stu-id="6caec-154">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 


# <a name="http"></a>[<span data-ttu-id="6caec-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="6caec-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```
# <a name="c"></a>[<span data-ttu-id="6caec-156">C#</span><span class="sxs-lookup"><span data-stu-id="6caec-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-iana-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6caec-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6caec-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-iana-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6caec-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6caec-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-iana-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6caec-159">Java</span><span class="sxs-lookup"><span data-stu-id="6caec-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-iana-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="6caec-160">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="6caec-160">Response 2</span></span>
<span data-ttu-id="6caec-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6caec-161">Here is an example of the response.</span></span> 

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


