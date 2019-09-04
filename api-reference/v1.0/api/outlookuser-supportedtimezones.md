---
title: 'outlookUser: supportedTimeZones'
description: Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3d408e1dcdaec6e28ce37b23b5421f86337064bc
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728596"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="3799c-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="3799c-103">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="3799c-104">Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="3799c-104">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="3799c-105">Вы можете явно указать, что часовые пояса должны возвращаться в формате часовых поясов Windows или [Администрации адресного пространства Интернета](https://www.iana.org/time-zones) (IANA, другое название — часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="3799c-105">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="3799c-106">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3799c-106">The Windows format is the default.</span></span>

<span data-ttu-id="3799c-107">Настраивая клиент Outlook, пользователь выбирает часовой пояс из этого списка.</span><span class="sxs-lookup"><span data-stu-id="3799c-107">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="3799c-108">После этого вы можете получить выбранный часовой пояс вместе с [ настройками почтового ящика пользователя](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="3799c-108">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="3799c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3799c-109">Permissions</span></span>
<span data-ttu-id="3799c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3799c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3799c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3799c-112">Permission type</span></span>      | <span data-ttu-id="3799c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3799c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3799c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3799c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3799c-115">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="3799c-115">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="3799c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3799c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3799c-117">User.Read</span><span class="sxs-lookup"><span data-stu-id="3799c-117">User.Read</span></span>    |
|<span data-ttu-id="3799c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3799c-118">Application</span></span> | <span data-ttu-id="3799c-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3799c-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3799c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3799c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="3799c-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3799c-121">Function parameters</span></span>
| <span data-ttu-id="3799c-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="3799c-122">Parameter</span></span>       | <span data-ttu-id="3799c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3799c-123">Type</span></span> | <span data-ttu-id="3799c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3799c-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3799c-125">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="3799c-125">TimeZoneStandard</span></span>  | <span data-ttu-id="3799c-126">тимезонестандард</span><span class="sxs-lookup"><span data-stu-id="3799c-126">timeZoneStandard</span></span>  | <span data-ttu-id="3799c-127">Формат часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="3799c-127">A time zone format.</span></span> <span data-ttu-id="3799c-128">Поддерживаемые значение: `Windows` и `Iana`.</span><span class="sxs-lookup"><span data-stu-id="3799c-128">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="3799c-129">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="3799c-129">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3799c-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3799c-130">Request headers</span></span>
| <span data-ttu-id="3799c-131">Имя</span><span class="sxs-lookup"><span data-stu-id="3799c-131">Name</span></span>       | <span data-ttu-id="3799c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3799c-132">Type</span></span> | <span data-ttu-id="3799c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3799c-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3799c-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="3799c-134">Authorization</span></span>  | <span data-ttu-id="3799c-135">string</span><span class="sxs-lookup"><span data-stu-id="3799c-135">string</span></span>  | <span data-ttu-id="3799c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3799c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3799c-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3799c-138">Request body</span></span>
<span data-ttu-id="3799c-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3799c-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3799c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3799c-140">Response</span></span>
<span data-ttu-id="3799c-141">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [timeZoneInformation](../resources/timezoneinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3799c-141">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3799c-142">Пример</span><span class="sxs-lookup"><span data-stu-id="3799c-142">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="3799c-143">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="3799c-143">Request 1</span></span>
<span data-ttu-id="3799c-144">В приведенном ниже примере не указывается параметр `timeZoneStandard` и считывается список поддерживаемых часовых поясов, представленных в формате часовых поясов Windows.</span><span class="sxs-lookup"><span data-stu-id="3799c-144">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="3799c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="3799c-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3799c-146">C#</span><span class="sxs-lookup"><span data-stu-id="3799c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3799c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3799c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3799c-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3799c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3799c-149">Java</span><span class="sxs-lookup"><span data-stu-id="3799c-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="3799c-150">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="3799c-150">Response 1</span></span>
<span data-ttu-id="3799c-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3799c-151">Here is an example of the response.</span></span> 
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

##### <a name="request-2"></a><span data-ttu-id="3799c-152">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="3799c-152">Request 2</span></span>
<span data-ttu-id="3799c-153">В приведенном ниже примере для параметра `TimeZoneStandard` задается значение `Iana` и считывается список поддерживаемых часовых поясов в формате IANA.</span><span class="sxs-lookup"><span data-stu-id="3799c-153">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="3799c-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="3799c-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3799c-155">C#</span><span class="sxs-lookup"><span data-stu-id="3799c-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-iana-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3799c-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3799c-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-iana-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3799c-157">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3799c-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-iana-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3799c-158">Java</span><span class="sxs-lookup"><span data-stu-id="3799c-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-iana-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="3799c-159">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="3799c-159">Response 2</span></span>
<span data-ttu-id="3799c-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3799c-160">Here is an example of the response.</span></span> 

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
