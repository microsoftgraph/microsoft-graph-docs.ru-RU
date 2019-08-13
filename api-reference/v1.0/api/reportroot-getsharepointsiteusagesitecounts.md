---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 4391198c93d31e1da33d3e36433df4500947639d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357984"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="bd056-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="bd056-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="bd056-105">Узнайте, сколько всего файлов на всех сайтах и сколько из них активны.</span><span class="sxs-lookup"><span data-stu-id="bd056-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="bd056-106">Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="bd056-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="bd056-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="bd056-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd056-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd056-108">Permissions</span></span>

<span data-ttu-id="bd056-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd056-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd056-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd056-111">Permission type</span></span>                        | <span data-ttu-id="bd056-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd056-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bd056-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd056-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd056-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd056-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bd056-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd056-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd056-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd056-116">Not supported.</span></span>                           |
| <span data-ttu-id="bd056-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd056-117">Application</span></span>                            | <span data-ttu-id="bd056-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd056-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bd056-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd056-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bd056-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="bd056-120">Function parameters</span></span>

<span data-ttu-id="bd056-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="bd056-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bd056-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="bd056-122">Parameter</span></span> | <span data-ttu-id="bd056-123">Тип</span><span class="sxs-lookup"><span data-stu-id="bd056-123">Type</span></span>   | <span data-ttu-id="bd056-124">Описание</span><span class="sxs-lookup"><span data-stu-id="bd056-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bd056-125">period</span><span class="sxs-lookup"><span data-stu-id="bd056-125">period</span></span>    | <span data-ttu-id="bd056-126">string</span><span class="sxs-lookup"><span data-stu-id="bd056-126">string</span></span> | <span data-ttu-id="bd056-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="bd056-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bd056-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="bd056-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bd056-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="bd056-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bd056-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd056-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="bd056-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd056-131">Request headers</span></span>

| <span data-ttu-id="bd056-132">Имя</span><span class="sxs-lookup"><span data-stu-id="bd056-132">Name</span></span>          | <span data-ttu-id="bd056-133">Описание</span><span class="sxs-lookup"><span data-stu-id="bd056-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="bd056-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd056-134">Authorization</span></span> | <span data-ttu-id="bd056-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd056-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="bd056-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="bd056-137">If-None-Match</span></span> | <span data-ttu-id="bd056-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="bd056-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="bd056-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bd056-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="bd056-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd056-140">Response</span></span>

<span data-ttu-id="bd056-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="bd056-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bd056-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="bd056-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bd056-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bd056-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bd056-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="bd056-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bd056-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="bd056-145">Report Refresh Date</span></span>
- <span data-ttu-id="bd056-146">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="bd056-146">Site Type</span></span>
- <span data-ttu-id="bd056-147">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="bd056-147">Total</span></span>
- <span data-ttu-id="bd056-148">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="bd056-148">Active</span></span>
- <span data-ttu-id="bd056-149">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="bd056-149">Report Date</span></span>
- <span data-ttu-id="bd056-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="bd056-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="bd056-151">Пример</span><span class="sxs-lookup"><span data-stu-id="bd056-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bd056-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd056-152">Request</span></span>

<span data-ttu-id="bd056-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd056-153">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bd056-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd056-154">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bd056-155">C#</span><span class="sxs-lookup"><span data-stu-id="bd056-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagesitecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd056-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd056-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagesitecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bd056-157">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bd056-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagesitecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bd056-158">Java</span><span class="sxs-lookup"><span data-stu-id="bd056-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagesitecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bd056-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd056-159">Response</span></span>

<span data-ttu-id="bd056-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd056-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="bd056-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="bd056-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
