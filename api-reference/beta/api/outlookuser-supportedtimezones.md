---
title: 'outlookUser: supportedTimeZones'
description: Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.
ms.openlocfilehash: c5886cc435b482a0acfcd99c65f356efe3a99d59
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075436"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="712f9-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="712f9-103">outlookUser: supportedTimeZones</span></span>

> <span data-ttu-id="712f9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="712f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="712f9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="712f9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="712f9-106">Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="712f9-106">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="712f9-107">Вы можете явно указать, что часовые пояса должны возвращаться в формате часовых поясов Windows или [Администрации адресного пространства Интернета](https://www.iana.org/time-zones) (IANA, другое название — часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="712f9-107">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="712f9-108">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="712f9-108">The Windows format is the default.</span></span>

<span data-ttu-id="712f9-109">Настраивая клиент Outlook, пользователь выбирает часовой пояс из этого списка.</span><span class="sxs-lookup"><span data-stu-id="712f9-109">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="712f9-110">После этого вы можете получить выбранный часовой пояс вместе с [ настройками почтового ящика пользователя](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="712f9-110">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="712f9-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="712f9-111">Permissions</span></span>
<span data-ttu-id="712f9-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="712f9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="712f9-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="712f9-114">Permission type</span></span>      | <span data-ttu-id="712f9-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="712f9-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="712f9-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="712f9-116">Delegated (work or school account)</span></span> | <span data-ttu-id="712f9-117">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="712f9-117">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="712f9-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="712f9-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="712f9-119">User.Read</span><span class="sxs-lookup"><span data-stu-id="712f9-119">User.Read</span></span>    |
|<span data-ttu-id="712f9-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="712f9-120">Application</span></span> | <span data-ttu-id="712f9-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="712f9-121">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="712f9-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="712f9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="712f9-123">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="712f9-123">Function parameters</span></span>
| <span data-ttu-id="712f9-124">Параметр функции</span><span class="sxs-lookup"><span data-stu-id="712f9-124">Function parameter</span></span>       | <span data-ttu-id="712f9-125">Тип</span><span class="sxs-lookup"><span data-stu-id="712f9-125">Type</span></span> | <span data-ttu-id="712f9-126">Описание</span><span class="sxs-lookup"><span data-stu-id="712f9-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="712f9-127">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="712f9-127">TimeZoneStandard</span></span>  | <span data-ttu-id="712f9-128">Строка</span><span class="sxs-lookup"><span data-stu-id="712f9-128">String</span></span>  | <span data-ttu-id="712f9-129">Формат часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="712f9-129">A time zone format.</span></span> <span data-ttu-id="712f9-130">Поддерживаемые значение: `Windows` и `Iana`.</span><span class="sxs-lookup"><span data-stu-id="712f9-130">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="712f9-131">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="712f9-131">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="712f9-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="712f9-132">Request headers</span></span>
| <span data-ttu-id="712f9-133">Имя</span><span class="sxs-lookup"><span data-stu-id="712f9-133">Name</span></span>       | <span data-ttu-id="712f9-134">Тип</span><span class="sxs-lookup"><span data-stu-id="712f9-134">Type</span></span> | <span data-ttu-id="712f9-135">Описание</span><span class="sxs-lookup"><span data-stu-id="712f9-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="712f9-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="712f9-136">Authorization</span></span>  | <span data-ttu-id="712f9-137">string</span><span class="sxs-lookup"><span data-stu-id="712f9-137">string</span></span>  | <span data-ttu-id="712f9-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="712f9-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="712f9-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="712f9-140">Request body</span></span>
<span data-ttu-id="712f9-141">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="712f9-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="712f9-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="712f9-142">Response</span></span>
<span data-ttu-id="712f9-143">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [timeZoneInformation](../resources/timezoneinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="712f9-143">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="712f9-144">Пример</span><span class="sxs-lookup"><span data-stu-id="712f9-144">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="712f9-145">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="712f9-145">Request 1</span></span>
<span data-ttu-id="712f9-146">В приведенном ниже примере не указывается параметр `timeZoneStandard` и считывается список поддерживаемых часовых поясов, представленных в формате часовых поясов Windows.</span><span class="sxs-lookup"><span data-stu-id="712f9-146">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="712f9-147">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="712f9-147">Response 1</span></span>
<span data-ttu-id="712f9-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="712f9-148">Here is an example of the response.</span></span> 
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

##### <a name="request-2"></a><span data-ttu-id="712f9-149">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="712f9-149">Request 2</span></span>
<span data-ttu-id="712f9-150">В приведенном ниже примере для параметра `TimeZoneStandard` задается значение `Iana` и считывается список поддерживаемых часовых поясов в формате IANA.</span><span class="sxs-lookup"><span data-stu-id="712f9-150">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="712f9-151">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="712f9-151">Response 2</span></span>
<span data-ttu-id="712f9-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="712f9-152">Here is an example of the response.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->