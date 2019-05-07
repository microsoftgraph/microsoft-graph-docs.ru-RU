---
title: 'reportRoot: getSharePointSiteUsageFileCounts'
description: Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c8ca5fcda937fea0833ea53074081a93d19c4764
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33604678"
---
# <a name="reportroot-getsharepointsiteusagefilecounts"></a><span data-ttu-id="9b9ab-104">reportRoot: getSharePointSiteUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="9b9ab-104">reportRoot: getSharePointSiteUsageFileCounts</span></span>

<span data-ttu-id="9b9ab-105">Узнайте, сколько всего файлов на всех сайтах и сколько из них активны.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="9b9ab-106">Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="9b9ab-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="9b9ab-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b9ab-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b9ab-108">Permissions</span></span>

<span data-ttu-id="9b9ab-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b9ab-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b9ab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b9ab-111">Permission type</span></span>                        | <span data-ttu-id="9b9ab-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b9ab-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9b9ab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b9ab-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b9ab-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b9ab-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9b9ab-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b9ab-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b9ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-116">Not supported.</span></span>                           |
| <span data-ttu-id="9b9ab-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b9ab-117">Application</span></span>                            | <span data-ttu-id="9b9ab-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b9ab-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9b9ab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b9ab-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9b9ab-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="9b9ab-120">Function parameters</span></span>

<span data-ttu-id="9b9ab-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9b9ab-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="9b9ab-122">Parameter</span></span> | <span data-ttu-id="9b9ab-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9b9ab-123">Type</span></span>   | <span data-ttu-id="9b9ab-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9b9ab-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9b9ab-125">period</span><span class="sxs-lookup"><span data-stu-id="9b9ab-125">period</span></span>    | <span data-ttu-id="9b9ab-126">string</span><span class="sxs-lookup"><span data-stu-id="9b9ab-126">string</span></span> | <span data-ttu-id="9b9ab-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9b9ab-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9b9ab-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9b9ab-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9b9ab-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b9ab-131">Request headers</span></span>

| <span data-ttu-id="9b9ab-132">Имя</span><span class="sxs-lookup"><span data-stu-id="9b9ab-132">Name</span></span>          | <span data-ttu-id="9b9ab-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9b9ab-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="9b9ab-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b9ab-134">Authorization</span></span> | <span data-ttu-id="9b9ab-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="9b9ab-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9b9ab-137">If-None-Match</span></span> | <span data-ttu-id="9b9ab-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="9b9ab-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9b9ab-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b9ab-140">Response</span></span>

<span data-ttu-id="9b9ab-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9b9ab-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9b9ab-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9b9ab-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="9b9ab-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9b9ab-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="9b9ab-145">Report Refresh Date</span></span>
- <span data-ttu-id="9b9ab-146">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="9b9ab-146">Site Type</span></span>
- <span data-ttu-id="9b9ab-147">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="9b9ab-147">Total</span></span>
- <span data-ttu-id="9b9ab-148">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="9b9ab-148">Active</span></span>
- <span data-ttu-id="9b9ab-149">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="9b9ab-149">Report Date</span></span>
- <span data-ttu-id="9b9ab-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="9b9ab-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="9b9ab-151">Пример</span><span class="sxs-lookup"><span data-stu-id="9b9ab-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9b9ab-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b9ab-152">Request</span></span>

<span data-ttu-id="9b9ab-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagefilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="9b9ab-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b9ab-154">Response</span></span>

<span data-ttu-id="9b9ab-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-155">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9b9ab-156">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="9b9ab-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9b9ab-157">Языках</span><span class="sxs-lookup"><span data-stu-id="9b9ab-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagefilecounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b9ab-158">Язык</span><span class="sxs-lookup"><span data-stu-id="9b9ab-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagefilecounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="9b9ab-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="9b9ab-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getsharepointsiteusagefilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getsharepointsiteusagefilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
