---
title: 'reportRoot: getYammerGroupsActivityCounts'
description: Узнайте, сколько сообщений Yammer было опубликовано, прочитано и оценено в группах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 634140649d86ad0c75208b2985b11fba50f44ab7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881251"
---
# <a name="reportroot-getyammergroupsactivitycounts"></a><span data-ttu-id="c5dc5-103">reportRoot: getYammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="c5dc5-103">reportRoot: getYammerGroupsActivityCounts</span></span>

<span data-ttu-id="c5dc5-104">Узнайте, сколько сообщений Yammer было опубликовано, прочитано и оценено в группах.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-104">Get the number of Yammer messages posted, read, and liked in groups.</span></span>

> <span data-ttu-id="c5dc5-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в группах Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="c5dc5-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5dc5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5dc5-106">Permissions</span></span>

<span data-ttu-id="c5dc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5dc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5dc5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5dc5-109">Permission type</span></span>                        | <span data-ttu-id="c5dc5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5dc5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c5dc5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5dc5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5dc5-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5dc5-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c5dc5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5dc5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5dc5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-114">Not supported.</span></span>                           |
| <span data-ttu-id="c5dc5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5dc5-115">Application</span></span>                            | <span data-ttu-id="c5dc5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5dc5-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c5dc5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5dc5-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c5dc5-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5dc5-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c5dc5-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c5dc5-119">Function parameters</span></span>

<span data-ttu-id="c5dc5-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c5dc5-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="c5dc5-121">Parameter</span></span> | <span data-ttu-id="c5dc5-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c5dc5-122">Type</span></span>   | <span data-ttu-id="c5dc5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c5dc5-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c5dc5-124">period</span><span class="sxs-lookup"><span data-stu-id="c5dc5-124">period</span></span>    | <span data-ttu-id="c5dc5-125">string</span><span class="sxs-lookup"><span data-stu-id="c5dc5-125">string</span></span> | <span data-ttu-id="c5dc5-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c5dc5-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c5dc5-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c5dc5-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c5dc5-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5dc5-130">Request headers</span></span>

| <span data-ttu-id="c5dc5-131">Имя</span><span class="sxs-lookup"><span data-stu-id="c5dc5-131">Name</span></span>          | <span data-ttu-id="c5dc5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5dc5-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c5dc5-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5dc5-133">Authorization</span></span> | <span data-ttu-id="c5dc5-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c5dc5-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c5dc5-136">If-None-Match</span></span> | <span data-ttu-id="c5dc5-137">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c5dc5-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c5dc5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5dc5-139">Response</span></span>

<span data-ttu-id="c5dc5-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c5dc5-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c5dc5-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c5dc5-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c5dc5-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c5dc5-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c5dc5-144">Report Refresh Date</span></span>
- <span data-ttu-id="c5dc5-145">"Liked" (Понравилось);</span><span class="sxs-lookup"><span data-stu-id="c5dc5-145">Liked</span></span>
- <span data-ttu-id="c5dc5-146">"Posted" (Опубликовано);</span><span class="sxs-lookup"><span data-stu-id="c5dc5-146">Posted</span></span>
- <span data-ttu-id="c5dc5-147">"Read" (Чтение);</span><span class="sxs-lookup"><span data-stu-id="c5dc5-147">Read</span></span>
- <span data-ttu-id="c5dc5-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="c5dc5-148">Report Date</span></span>
- <span data-ttu-id="c5dc5-149">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="c5dc5-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c5dc5-150">Пример</span><span class="sxs-lookup"><span data-stu-id="c5dc5-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c5dc5-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5dc5-151">Request</span></span>

<span data-ttu-id="c5dc5-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c5dc5-153">C#</span><span class="sxs-lookup"><span data-stu-id="c5dc5-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5dc5-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="c5dc5-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c5dc5-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c5dc5-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c5dc5-156">Java</span><span class="sxs-lookup"><span data-stu-id="c5dc5-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammergroupsactivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c5dc5-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5dc5-157">Response</span></span>

<span data-ttu-id="c5dc5-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="c5dc5-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c5dc5-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
