---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Получите сведения об активности пользователей в SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7fec31dd0ceab917f85714cf452617a5bba4b32d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572250"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="08482-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="08482-103">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="08482-104">Получите сведения об активности пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="08482-104">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="08482-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="08482-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="08482-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08482-106">Permissions</span></span>

<span data-ttu-id="08482-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08482-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08482-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08482-109">Permission type</span></span>                        | <span data-ttu-id="08482-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08482-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="08482-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08482-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="08482-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08482-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="08482-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08482-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08482-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08482-114">Not supported.</span></span>                           |
| <span data-ttu-id="08482-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08482-115">Application</span></span>                            | <span data-ttu-id="08482-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08482-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="08482-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08482-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="08482-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="08482-118">Function parameters</span></span>

<span data-ttu-id="08482-119">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="08482-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="08482-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="08482-120">Parameter</span></span> | <span data-ttu-id="08482-121">Тип</span><span class="sxs-lookup"><span data-stu-id="08482-121">Type</span></span>   | <span data-ttu-id="08482-122">Описание</span><span class="sxs-lookup"><span data-stu-id="08482-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="08482-123">period</span><span class="sxs-lookup"><span data-stu-id="08482-123">period</span></span>    | <span data-ttu-id="08482-124">строка</span><span class="sxs-lookup"><span data-stu-id="08482-124">string</span></span> | <span data-ttu-id="08482-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="08482-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="08482-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="08482-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="08482-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="08482-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="08482-128">date</span><span class="sxs-lookup"><span data-stu-id="08482-128">date</span></span>      | <span data-ttu-id="08482-129">Date</span><span class="sxs-lookup"><span data-stu-id="08482-129">Date</span></span>   | <span data-ttu-id="08482-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="08482-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="08482-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="08482-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="08482-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="08482-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="08482-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="08482-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08482-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08482-134">Request headers</span></span>

| <span data-ttu-id="08482-135">Имя</span><span class="sxs-lookup"><span data-stu-id="08482-135">Name</span></span>          | <span data-ttu-id="08482-136">Описание</span><span class="sxs-lookup"><span data-stu-id="08482-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="08482-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08482-137">Authorization</span></span> | <span data-ttu-id="08482-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08482-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="08482-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="08482-140">If-None-Match</span></span> | <span data-ttu-id="08482-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="08482-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="08482-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="08482-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="08482-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="08482-143">Response</span></span>

<span data-ttu-id="08482-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="08482-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="08482-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="08482-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="08482-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="08482-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="08482-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="08482-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="08482-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="08482-148">Report Refresh Date</span></span>
- <span data-ttu-id="08482-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="08482-149">User Principal Name</span></span>
- <span data-ttu-id="08482-150">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="08482-150">Is Deleted</span></span>
- <span data-ttu-id="08482-151">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="08482-151">Deleted Date</span></span>
- <span data-ttu-id="08482-152">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="08482-152">Last Activity Date</span></span>
- <span data-ttu-id="08482-153">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="08482-153">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="08482-154">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="08482-154">Synced File Count</span></span>
- <span data-ttu-id="08482-155">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="08482-155">Shared Internally File Count</span></span>
- <span data-ttu-id="08482-156">Shared Externally File Count (количество файлов, отправленных за пределы организации)</span><span class="sxs-lookup"><span data-stu-id="08482-156">Shared Externally File Count</span></span>
- <span data-ttu-id="08482-157">Visited Page Count (количество посещенных страниц)</span><span class="sxs-lookup"><span data-stu-id="08482-157">Visited Page Count</span></span>
- <span data-ttu-id="08482-158">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="08482-158">Assigned Products</span></span>
- <span data-ttu-id="08482-159">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="08482-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="08482-160">Пример</span><span class="sxs-lookup"><span data-stu-id="08482-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="08482-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="08482-161">Request</span></span>

<span data-ttu-id="08482-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08482-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="08482-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="08482-163">Response</span></span>

<span data-ttu-id="08482-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="08482-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="08482-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="08482-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
```
