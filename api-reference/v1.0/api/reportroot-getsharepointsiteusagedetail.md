---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: Получение сведений об использовании сайтов SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 2ac63d1c94ae0ffe67143cb04a8e66566dfc4509
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33604760"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="71b41-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="71b41-103">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="71b41-104">Получение сведений об использовании сайтов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="71b41-104">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="71b41-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="71b41-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="71b41-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71b41-106">Permissions</span></span>

<span data-ttu-id="71b41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71b41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71b41-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71b41-109">Permission type</span></span>                        | <span data-ttu-id="71b41-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71b41-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="71b41-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71b41-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="71b41-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="71b41-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="71b41-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71b41-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71b41-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71b41-114">Not supported.</span></span>                           |
| <span data-ttu-id="71b41-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71b41-115">Application</span></span>                            | <span data-ttu-id="71b41-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="71b41-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="71b41-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71b41-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="71b41-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="71b41-118">Function parameters</span></span>

<span data-ttu-id="71b41-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="71b41-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="71b41-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="71b41-120">Parameter</span></span> | <span data-ttu-id="71b41-121">Тип</span><span class="sxs-lookup"><span data-stu-id="71b41-121">Type</span></span>   | <span data-ttu-id="71b41-122">Описание</span><span class="sxs-lookup"><span data-stu-id="71b41-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="71b41-123">period</span><span class="sxs-lookup"><span data-stu-id="71b41-123">period</span></span>    | <span data-ttu-id="71b41-124">string</span><span class="sxs-lookup"><span data-stu-id="71b41-124">string</span></span> | <span data-ttu-id="71b41-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="71b41-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="71b41-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="71b41-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="71b41-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="71b41-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="71b41-128">date</span><span class="sxs-lookup"><span data-stu-id="71b41-128">date</span></span>      | <span data-ttu-id="71b41-129">Date</span><span class="sxs-lookup"><span data-stu-id="71b41-129">Date</span></span>   | <span data-ttu-id="71b41-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="71b41-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="71b41-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="71b41-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="71b41-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="71b41-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="71b41-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="71b41-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71b41-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71b41-134">Request headers</span></span>

| <span data-ttu-id="71b41-135">Имя</span><span class="sxs-lookup"><span data-stu-id="71b41-135">Name</span></span>          | <span data-ttu-id="71b41-136">Описание</span><span class="sxs-lookup"><span data-stu-id="71b41-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="71b41-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71b41-137">Authorization</span></span> | <span data-ttu-id="71b41-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71b41-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="71b41-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="71b41-140">If-None-Match</span></span> | <span data-ttu-id="71b41-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="71b41-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="71b41-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="71b41-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="71b41-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="71b41-143">Response</span></span>

<span data-ttu-id="71b41-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="71b41-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="71b41-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="71b41-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="71b41-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="71b41-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="71b41-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="71b41-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="71b41-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="71b41-148">Report Refresh Date</span></span>
- <span data-ttu-id="71b41-149">Идентификатор сайта</span><span class="sxs-lookup"><span data-stu-id="71b41-149">Site Id</span></span>
- <span data-ttu-id="71b41-150">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="71b41-150">Site URL</span></span>
- <span data-ttu-id="71b41-151">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="71b41-151">Owner Display Name</span></span>
- <span data-ttu-id="71b41-152">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="71b41-152">Is Deleted</span></span>
- <span data-ttu-id="71b41-153">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="71b41-153">Last Activity Date</span></span>
- <span data-ttu-id="71b41-154">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="71b41-154">File Count</span></span>
- <span data-ttu-id="71b41-155">"Active File Count" (Количество активных файлов);</span><span class="sxs-lookup"><span data-stu-id="71b41-155">Active File Count</span></span>
- <span data-ttu-id="71b41-156">"Page View Count" (Количество просмотров страницы);</span><span class="sxs-lookup"><span data-stu-id="71b41-156">Page View Count</span></span>
- <span data-ttu-id="71b41-157">"Visited Page Count" (Количество посещенных страниц);</span><span class="sxs-lookup"><span data-stu-id="71b41-157">Visited Page Count</span></span>
- <span data-ttu-id="71b41-158">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="71b41-158">Storage Used (Byte)</span></span>
- <span data-ttu-id="71b41-159">"Storage Allocated (Byte)" (Объем выделенного хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="71b41-159">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="71b41-160">"Root Web Template" (Шаблон корневого веб-сайта);</span><span class="sxs-lookup"><span data-stu-id="71b41-160">Root Web Template</span></span>
- <span data-ttu-id="71b41-161">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="71b41-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="71b41-162">Пример</span><span class="sxs-lookup"><span data-stu-id="71b41-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="71b41-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="71b41-163">Request</span></span>

<span data-ttu-id="71b41-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71b41-164">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="71b41-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="71b41-165">Response</span></span>

<span data-ttu-id="71b41-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71b41-166">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="71b41-167">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="71b41-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="71b41-168">Языках</span><span class="sxs-lookup"><span data-stu-id="71b41-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusageuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71b41-169">Язык</span><span class="sxs-lookup"><span data-stu-id="71b41-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusageuserdetail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="71b41-170">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="71b41-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getsharepointsiteusagedetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getsharepointsiteusagedetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
