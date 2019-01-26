---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e0d55b24bc22c64adb7a17fe8fa3a56284301f00
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572894"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="08faf-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="08faf-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="08faf-105">Узнайте, сколько всего файлов на всех сайтах и сколько из них активны.</span><span class="sxs-lookup"><span data-stu-id="08faf-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="08faf-106">Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="08faf-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="08faf-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="08faf-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="08faf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08faf-108">Permissions</span></span>

<span data-ttu-id="08faf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08faf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08faf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08faf-111">Permission type</span></span>                        | <span data-ttu-id="08faf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08faf-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="08faf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08faf-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="08faf-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08faf-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="08faf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08faf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08faf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08faf-116">Not supported.</span></span>                           |
| <span data-ttu-id="08faf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08faf-117">Application</span></span>                            | <span data-ttu-id="08faf-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08faf-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="08faf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08faf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="08faf-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="08faf-120">Function parameters</span></span>

<span data-ttu-id="08faf-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="08faf-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="08faf-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="08faf-122">Parameter</span></span> | <span data-ttu-id="08faf-123">Тип</span><span class="sxs-lookup"><span data-stu-id="08faf-123">Type</span></span>   | <span data-ttu-id="08faf-124">Описание</span><span class="sxs-lookup"><span data-stu-id="08faf-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="08faf-125">period</span><span class="sxs-lookup"><span data-stu-id="08faf-125">period</span></span>    | <span data-ttu-id="08faf-126">строка</span><span class="sxs-lookup"><span data-stu-id="08faf-126">string</span></span> | <span data-ttu-id="08faf-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="08faf-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="08faf-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="08faf-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="08faf-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="08faf-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="08faf-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08faf-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="08faf-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08faf-131">Request headers</span></span>

| <span data-ttu-id="08faf-132">Имя</span><span class="sxs-lookup"><span data-stu-id="08faf-132">Name</span></span>          | <span data-ttu-id="08faf-133">Описание</span><span class="sxs-lookup"><span data-stu-id="08faf-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="08faf-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08faf-134">Authorization</span></span> | <span data-ttu-id="08faf-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08faf-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="08faf-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="08faf-137">If-None-Match</span></span> | <span data-ttu-id="08faf-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="08faf-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="08faf-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="08faf-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="08faf-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="08faf-140">Response</span></span>

<span data-ttu-id="08faf-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="08faf-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="08faf-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="08faf-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="08faf-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="08faf-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="08faf-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="08faf-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="08faf-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="08faf-145">Report Refresh Date</span></span>
- <span data-ttu-id="08faf-146">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="08faf-146">Site Type</span></span>
- <span data-ttu-id="08faf-147">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="08faf-147">Total</span></span>
- <span data-ttu-id="08faf-148">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="08faf-148">Active</span></span>
- <span data-ttu-id="08faf-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="08faf-149">Report Date</span></span>
- <span data-ttu-id="08faf-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="08faf-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="08faf-151">Пример</span><span class="sxs-lookup"><span data-stu-id="08faf-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="08faf-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="08faf-152">Request</span></span>

<span data-ttu-id="08faf-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08faf-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="08faf-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="08faf-154">Response</span></span>

<span data-ttu-id="08faf-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="08faf-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="08faf-156">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="08faf-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
