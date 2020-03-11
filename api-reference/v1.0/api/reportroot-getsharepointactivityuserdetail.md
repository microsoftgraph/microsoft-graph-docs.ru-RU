---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Получите сведения об активности пользователей в SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 31d2338cc06b04b8466b8746bc59c89e1ef78e7b
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591315"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="3e796-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="3e796-103">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="3e796-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e796-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e796-105">Получите сведения об активности пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3e796-105">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="3e796-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="3e796-106">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e796-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e796-107">Permissions</span></span>

<span data-ttu-id="3e796-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e796-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e796-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e796-110">Permission type</span></span>                        | <span data-ttu-id="3e796-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e796-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3e796-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e796-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e796-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e796-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3e796-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e796-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e796-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e796-115">Not supported.</span></span>                           |
| <span data-ttu-id="3e796-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e796-116">Application</span></span>                            | <span data-ttu-id="3e796-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e796-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="3e796-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3e796-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3e796-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="3e796-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3e796-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e796-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="3e796-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3e796-121">Function parameters</span></span>

<span data-ttu-id="3e796-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3e796-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="3e796-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="3e796-123">Parameter</span></span> | <span data-ttu-id="3e796-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3e796-124">Type</span></span>   | <span data-ttu-id="3e796-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3e796-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3e796-126">period</span><span class="sxs-lookup"><span data-stu-id="3e796-126">period</span></span>    | <span data-ttu-id="3e796-127">string</span><span class="sxs-lookup"><span data-stu-id="3e796-127">string</span></span> | <span data-ttu-id="3e796-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3e796-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3e796-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3e796-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3e796-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3e796-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="3e796-131">date</span><span class="sxs-lookup"><span data-stu-id="3e796-131">date</span></span>      | <span data-ttu-id="3e796-132">Date</span><span class="sxs-lookup"><span data-stu-id="3e796-132">Date</span></span>   | <span data-ttu-id="3e796-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="3e796-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="3e796-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="3e796-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="3e796-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="3e796-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="3e796-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="3e796-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e796-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e796-137">Request headers</span></span>

| <span data-ttu-id="3e796-138">Имя</span><span class="sxs-lookup"><span data-stu-id="3e796-138">Name</span></span>          | <span data-ttu-id="3e796-139">Описание</span><span class="sxs-lookup"><span data-stu-id="3e796-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3e796-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e796-140">Authorization</span></span> | <span data-ttu-id="3e796-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e796-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3e796-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3e796-143">If-None-Match</span></span> | <span data-ttu-id="3e796-144">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="3e796-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3e796-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3e796-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3e796-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e796-146">Response</span></span>

<span data-ttu-id="3e796-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3e796-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3e796-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3e796-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3e796-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3e796-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3e796-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3e796-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3e796-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3e796-151">Report Refresh Date</span></span>
- <span data-ttu-id="3e796-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="3e796-152">User Principal Name</span></span>
- <span data-ttu-id="3e796-153">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="3e796-153">Is Deleted</span></span>
- <span data-ttu-id="3e796-154">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="3e796-154">Deleted Date</span></span>
- <span data-ttu-id="3e796-155">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="3e796-155">Last Activity Date</span></span>
- <span data-ttu-id="3e796-156">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="3e796-156">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="3e796-157">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="3e796-157">Synced File Count</span></span>
- <span data-ttu-id="3e796-158">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="3e796-158">Shared Internally File Count</span></span>
- <span data-ttu-id="3e796-159">Shared Externally File Count (количество файлов, отправленных за пределы организации)</span><span class="sxs-lookup"><span data-stu-id="3e796-159">Shared Externally File Count</span></span>
- <span data-ttu-id="3e796-160">Visited Page Count (количество посещенных страниц)</span><span class="sxs-lookup"><span data-stu-id="3e796-160">Visited Page Count</span></span>
- <span data-ttu-id="3e796-161">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="3e796-161">Assigned Products</span></span>
- <span data-ttu-id="3e796-162">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="3e796-162">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3e796-163">Пример</span><span class="sxs-lookup"><span data-stu-id="3e796-163">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3e796-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e796-164">Request</span></span>

<span data-ttu-id="3e796-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e796-165">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="3e796-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e796-166">Response</span></span>

<span data-ttu-id="3e796-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3e796-167">The following is an example of the response.</span></span>

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

<span data-ttu-id="3e796-168">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3e796-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
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
