---
title: 'reportRoot: getYammerGroupsActivityCounts'
description: Узнайте, сколько сообщений Yammer было опубликовано, прочитано и оценено в группах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 84d438149e7bf39e823d6fefe0d691a1691dd067
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603808"
---
# <a name="reportroot-getyammergroupsactivitycounts"></a><span data-ttu-id="4032b-103">reportRoot: getYammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4032b-103">reportRoot: getYammerGroupsActivityCounts</span></span>

<span data-ttu-id="4032b-104">Узнайте, сколько сообщений Yammer было опубликовано, прочитано и оценено в группах.</span><span class="sxs-lookup"><span data-stu-id="4032b-104">Get the number of Yammer messages posted, read, and liked in groups.</span></span>

> <span data-ttu-id="4032b-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в группах Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="4032b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="4032b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4032b-106">Permissions</span></span>

<span data-ttu-id="4032b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4032b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4032b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4032b-109">Permission type</span></span>                        | <span data-ttu-id="4032b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4032b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4032b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4032b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4032b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4032b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4032b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4032b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4032b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4032b-114">Not supported.</span></span>                           |
| <span data-ttu-id="4032b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4032b-115">Application</span></span>                            | <span data-ttu-id="4032b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4032b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4032b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4032b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4032b-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4032b-118">Function parameters</span></span>

<span data-ttu-id="4032b-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4032b-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4032b-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="4032b-120">Parameter</span></span> | <span data-ttu-id="4032b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4032b-121">Type</span></span>   | <span data-ttu-id="4032b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4032b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4032b-123">period</span><span class="sxs-lookup"><span data-stu-id="4032b-123">period</span></span>    | <span data-ttu-id="4032b-124">string</span><span class="sxs-lookup"><span data-stu-id="4032b-124">string</span></span> | <span data-ttu-id="4032b-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4032b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4032b-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4032b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4032b-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4032b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4032b-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4032b-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4032b-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4032b-129">Request headers</span></span>

| <span data-ttu-id="4032b-130">Имя</span><span class="sxs-lookup"><span data-stu-id="4032b-130">Name</span></span>          | <span data-ttu-id="4032b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4032b-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4032b-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4032b-132">Authorization</span></span> | <span data-ttu-id="4032b-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4032b-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4032b-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4032b-135">If-None-Match</span></span> | <span data-ttu-id="4032b-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="4032b-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4032b-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4032b-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4032b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4032b-138">Response</span></span>

<span data-ttu-id="4032b-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4032b-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4032b-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4032b-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4032b-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4032b-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4032b-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4032b-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4032b-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4032b-143">Report Refresh Date</span></span>
- <span data-ttu-id="4032b-144">"Liked" (Понравилось);</span><span class="sxs-lookup"><span data-stu-id="4032b-144">Liked</span></span>
- <span data-ttu-id="4032b-145">"Posted" (Опубликовано);</span><span class="sxs-lookup"><span data-stu-id="4032b-145">Posted</span></span>
- <span data-ttu-id="4032b-146">"Read" (Чтение);</span><span class="sxs-lookup"><span data-stu-id="4032b-146">Read</span></span>
- <span data-ttu-id="4032b-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="4032b-147">Report Date</span></span>
- <span data-ttu-id="4032b-148">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="4032b-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4032b-149">Пример</span><span class="sxs-lookup"><span data-stu-id="4032b-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4032b-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="4032b-150">Request</span></span>

<span data-ttu-id="4032b-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4032b-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="4032b-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="4032b-152">Response</span></span>

<span data-ttu-id="4032b-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4032b-153">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4032b-154">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="4032b-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4032b-155">Языках</span><span class="sxs-lookup"><span data-stu-id="4032b-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitycounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4032b-156">Язык</span><span class="sxs-lookup"><span data-stu-id="4032b-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitycounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="4032b-157">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4032b-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getyammergroupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getyammergroupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
