---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Получите сведения об активности пользователей в SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 49eb57db04a8d9bcf243ac1ec28cfb7ce2ec5541
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897941"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="5f2d7-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="5f2d7-103">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="5f2d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f2d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f2d7-105">Получите сведения о действиях в SharePoint с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-105">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="5f2d7-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-SharePoint Activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="5f2d7-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="5f2d7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f2d7-107">Permissions</span></span>

<span data-ttu-id="5f2d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f2d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f2d7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f2d7-110">Permission type</span></span>                        | <span data-ttu-id="5f2d7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f2d7-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5f2d7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f2d7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f2d7-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f2d7-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5f2d7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f2d7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f2d7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-115">Not supported.</span></span>                           |
| <span data-ttu-id="5f2d7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f2d7-116">Application</span></span>                            | <span data-ttu-id="5f2d7-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f2d7-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="5f2d7-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5f2d7-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5f2d7-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5f2d7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f2d7-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5f2d7-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="5f2d7-121">Function parameters</span></span>

<span data-ttu-id="5f2d7-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="5f2d7-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="5f2d7-123">Parameter</span></span> | <span data-ttu-id="5f2d7-124">Тип</span><span class="sxs-lookup"><span data-stu-id="5f2d7-124">Type</span></span>   | <span data-ttu-id="5f2d7-125">Описание</span><span class="sxs-lookup"><span data-stu-id="5f2d7-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5f2d7-126">period</span><span class="sxs-lookup"><span data-stu-id="5f2d7-126">period</span></span>    | <span data-ttu-id="5f2d7-127">string</span><span class="sxs-lookup"><span data-stu-id="5f2d7-127">string</span></span> | <span data-ttu-id="5f2d7-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5f2d7-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5f2d7-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5f2d7-131">date</span><span class="sxs-lookup"><span data-stu-id="5f2d7-131">date</span></span>      | <span data-ttu-id="5f2d7-132">Date</span><span class="sxs-lookup"><span data-stu-id="5f2d7-132">Date</span></span>   | <span data-ttu-id="5f2d7-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5f2d7-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5f2d7-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5f2d7-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f2d7-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f2d7-137">Request headers</span></span>

| <span data-ttu-id="5f2d7-138">Имя</span><span class="sxs-lookup"><span data-stu-id="5f2d7-138">Name</span></span>          | <span data-ttu-id="5f2d7-139">Описание</span><span class="sxs-lookup"><span data-stu-id="5f2d7-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5f2d7-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f2d7-140">Authorization</span></span> | <span data-ttu-id="5f2d7-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5f2d7-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5f2d7-143">If-None-Match</span></span> | <span data-ttu-id="5f2d7-144">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5f2d7-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5f2d7-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f2d7-146">Response</span></span>

<span data-ttu-id="5f2d7-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5f2d7-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5f2d7-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5f2d7-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="5f2d7-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5f2d7-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="5f2d7-151">Report Refresh Date</span></span>
- <span data-ttu-id="5f2d7-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="5f2d7-152">User Principal Name</span></span>
- <span data-ttu-id="5f2d7-153">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="5f2d7-153">Is Deleted</span></span>
- <span data-ttu-id="5f2d7-154">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="5f2d7-154">Deleted Date</span></span>
- <span data-ttu-id="5f2d7-155">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="5f2d7-155">Last Activity Date</span></span>
- <span data-ttu-id="5f2d7-156">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="5f2d7-156">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="5f2d7-157">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="5f2d7-157">Synced File Count</span></span>
- <span data-ttu-id="5f2d7-158">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="5f2d7-158">Shared Internally File Count</span></span>
- <span data-ttu-id="5f2d7-159">Shared Externally File Count (количество файлов, отправленных за пределы организации)</span><span class="sxs-lookup"><span data-stu-id="5f2d7-159">Shared Externally File Count</span></span>
- <span data-ttu-id="5f2d7-160">Visited Page Count (количество посещенных страниц)</span><span class="sxs-lookup"><span data-stu-id="5f2d7-160">Visited Page Count</span></span>
- <span data-ttu-id="5f2d7-161">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="5f2d7-161">Assigned Products</span></span>
- <span data-ttu-id="5f2d7-162">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="5f2d7-162">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5f2d7-163">Пример</span><span class="sxs-lookup"><span data-stu-id="5f2d7-163">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5f2d7-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f2d7-164">Request</span></span>

<span data-ttu-id="5f2d7-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-165">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="5f2d7-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f2d7-166">Response</span></span>

<span data-ttu-id="5f2d7-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-167">The following is an example of the response.</span></span>

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

<span data-ttu-id="5f2d7-168">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="5f2d7-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
