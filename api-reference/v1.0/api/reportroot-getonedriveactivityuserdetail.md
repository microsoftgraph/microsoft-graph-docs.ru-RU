---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Получите сведения о действиях в OneDrive с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e0a94e160b6583b4e073f7ca1bceb9137694cf6e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268609"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="e238b-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="e238b-103">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="e238b-104">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="e238b-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="e238b-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="e238b-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="e238b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e238b-106">Permissions</span></span>

<span data-ttu-id="e238b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e238b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e238b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e238b-109">Permission type</span></span>                        | <span data-ttu-id="e238b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e238b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e238b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e238b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e238b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e238b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e238b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e238b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e238b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e238b-114">Not supported.</span></span>                           |
| <span data-ttu-id="e238b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e238b-115">Application</span></span>                            | <span data-ttu-id="e238b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e238b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e238b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e238b-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e238b-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="e238b-118">Function parameters</span></span>

<span data-ttu-id="e238b-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="e238b-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e238b-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="e238b-120">Parameter</span></span> | <span data-ttu-id="e238b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e238b-121">Type</span></span>   | <span data-ttu-id="e238b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e238b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e238b-123">period</span><span class="sxs-lookup"><span data-stu-id="e238b-123">period</span></span>    | <span data-ttu-id="e238b-124">string</span><span class="sxs-lookup"><span data-stu-id="e238b-124">string</span></span> | <span data-ttu-id="e238b-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="e238b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e238b-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="e238b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e238b-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="e238b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e238b-128">date</span><span class="sxs-lookup"><span data-stu-id="e238b-128">date</span></span>      | <span data-ttu-id="e238b-129">Date</span><span class="sxs-lookup"><span data-stu-id="e238b-129">Date</span></span>   | <span data-ttu-id="e238b-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="e238b-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e238b-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="e238b-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e238b-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="e238b-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e238b-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="e238b-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e238b-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e238b-134">Request headers</span></span>

| <span data-ttu-id="e238b-135">Имя</span><span class="sxs-lookup"><span data-stu-id="e238b-135">Name</span></span>          | <span data-ttu-id="e238b-136">Описание</span><span class="sxs-lookup"><span data-stu-id="e238b-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e238b-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e238b-137">Authorization</span></span> | <span data-ttu-id="e238b-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e238b-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e238b-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e238b-140">If-None-Match</span></span> | <span data-ttu-id="e238b-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="e238b-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e238b-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e238b-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e238b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e238b-143">Response</span></span>

<span data-ttu-id="e238b-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="e238b-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e238b-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="e238b-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e238b-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e238b-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e238b-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="e238b-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e238b-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="e238b-148">Report Refresh Date</span></span>
- <span data-ttu-id="e238b-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="e238b-149">User Principal Name</span></span>
- <span data-ttu-id="e238b-150">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="e238b-150">Is Deleted</span></span>
- <span data-ttu-id="e238b-151">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="e238b-151">Deleted Date</span></span>
- <span data-ttu-id="e238b-152">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="e238b-152">Last Activity Date</span></span>
- <span data-ttu-id="e238b-153">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="e238b-153">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="e238b-154">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="e238b-154">Synced File Count</span></span>
- <span data-ttu-id="e238b-155">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="e238b-155">Shared Internally File Count</span></span>
- <span data-ttu-id="e238b-156">"Shared Externally File Count" (Количество файлов, к которым предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="e238b-156">Shared Externally File Count</span></span>
- <span data-ttu-id="e238b-157">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="e238b-157">Assigned Products</span></span>
- <span data-ttu-id="e238b-158">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="e238b-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e238b-159">Пример</span><span class="sxs-lookup"><span data-stu-id="e238b-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e238b-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="e238b-160">Request</span></span>

<span data-ttu-id="e238b-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e238b-161">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="e238b-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="e238b-162">Response</span></span>

<span data-ttu-id="e238b-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e238b-163">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e238b-164">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e238b-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e238b-165">C#</span><span class="sxs-lookup"><span data-stu-id="e238b-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e238b-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="e238b-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e238b-167">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e238b-167">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="e238b-168">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="e238b-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getonedriveactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getonedriveactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getonedriveactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
