---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 878f23339deacbc76e4cb9eed053a76db0ebaddd
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981202"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="cf9a6-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="cf9a6-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="cf9a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf9a6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cf9a6-105">Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-105">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf9a6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf9a6-106">Permissions</span></span>

<span data-ttu-id="cf9a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf9a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf9a6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf9a6-109">Permission type</span></span>                        | <span data-ttu-id="cf9a6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf9a6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cf9a6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf9a6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf9a6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf9a6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cf9a6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf9a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf9a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-114">Not supported.</span></span>                           |
| <span data-ttu-id="cf9a6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf9a6-115">Application</span></span>                            | <span data-ttu-id="cf9a6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf9a6-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="cf9a6-117">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="cf9a6-118">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="cf9a6-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="cf9a6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf9a6-119">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='{period_value}')
GET /reports/getTeamsDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="cf9a6-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="cf9a6-120">Function parameters</span></span>

<span data-ttu-id="cf9a6-121">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="cf9a6-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="cf9a6-122">Parameter</span></span> | <span data-ttu-id="cf9a6-123">Тип</span><span class="sxs-lookup"><span data-stu-id="cf9a6-123">Type</span></span>   | <span data-ttu-id="cf9a6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cf9a6-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cf9a6-125">period</span><span class="sxs-lookup"><span data-stu-id="cf9a6-125">period</span></span>    | <span data-ttu-id="cf9a6-126">string</span><span class="sxs-lookup"><span data-stu-id="cf9a6-126">string</span></span> | <span data-ttu-id="cf9a6-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cf9a6-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cf9a6-129">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-129">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="cf9a6-130">date</span><span class="sxs-lookup"><span data-stu-id="cf9a6-130">date</span></span>      | <span data-ttu-id="cf9a6-131">Date</span><span class="sxs-lookup"><span data-stu-id="cf9a6-131">Date</span></span>   | <span data-ttu-id="cf9a6-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="cf9a6-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="cf9a6-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="cf9a6-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf9a6-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf9a6-136">Request headers</span></span>

| <span data-ttu-id="cf9a6-137">Имя</span><span class="sxs-lookup"><span data-stu-id="cf9a6-137">Name</span></span>          | <span data-ttu-id="cf9a6-138">Описание</span><span class="sxs-lookup"><span data-stu-id="cf9a6-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cf9a6-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf9a6-139">Authorization</span></span> | <span data-ttu-id="cf9a6-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cf9a6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf9a6-142">Response</span></span>

<span data-ttu-id="cf9a6-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cf9a6-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cf9a6-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cf9a6-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="cf9a6-146">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="cf9a6-147">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="cf9a6-147">Report Refresh Date</span></span>
- <span data-ttu-id="cf9a6-148">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="cf9a6-148">User Principal Name</span></span>
- <span data-ttu-id="cf9a6-149">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="cf9a6-149">Last Activity Date</span></span>
- <span data-ttu-id="cf9a6-150">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="cf9a6-150">Is Deleted</span></span>
- <span data-ttu-id="cf9a6-151">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="cf9a6-151">Deleted Date</span></span>
- <span data-ttu-id="cf9a6-152">Used Web (использовал браузер);</span><span class="sxs-lookup"><span data-stu-id="cf9a6-152">Used Web</span></span>
- <span data-ttu-id="cf9a6-153">Used Windows Phone (использовал телефон с Windows);</span><span class="sxs-lookup"><span data-stu-id="cf9a6-153">Used Windows Phone</span></span>
- <span data-ttu-id="cf9a6-154">Used iOS (использовал iOS);</span><span class="sxs-lookup"><span data-stu-id="cf9a6-154">Used iOS</span></span>
- <span data-ttu-id="cf9a6-155">Used Mac (использовал Mac);</span><span class="sxs-lookup"><span data-stu-id="cf9a6-155">Used Mac</span></span>
- <span data-ttu-id="cf9a6-156">Used Android Phone (использовал телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="cf9a6-156">Used Android Phone</span></span>
- <span data-ttu-id="cf9a6-157">Used Windows (использовал Windows);</span><span class="sxs-lookup"><span data-stu-id="cf9a6-157">Used Windows</span></span>
- <span data-ttu-id="cf9a6-158">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="cf9a6-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="cf9a6-159">Пример</span><span class="sxs-lookup"><span data-stu-id="cf9a6-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cf9a6-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf9a6-160">Request</span></span>

<span data-ttu-id="cf9a6-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="cf9a6-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf9a6-162">Response</span></span>

<span data-ttu-id="cf9a6-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cf9a6-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="cf9a6-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

