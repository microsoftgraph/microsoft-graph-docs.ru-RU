---
title: 'reportRoot: getYammerGroupsActivityGroupCounts'
description: Узнайте, сколько всего существовало групп и в скольких из них выполнялись действия с беседами.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c36ffa232b1697779aabf16041ff65c3fe25aef6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347690"
---
# <a name="reportroot-getyammergroupsactivitygroupcounts"></a><span data-ttu-id="ffe82-103">reportRoot: getYammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="ffe82-103">reportRoot: getYammerGroupsActivityGroupCounts</span></span>

<span data-ttu-id="ffe82-104">Узнайте, сколько всего существовало групп и в скольких из них выполнялись действия с беседами.</span><span class="sxs-lookup"><span data-stu-id="ffe82-104">Get the total number of groups that existed and how many included group conversation activity.</span></span>

> <span data-ttu-id="ffe82-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в группах Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="ffe82-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="ffe82-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ffe82-106">Permissions</span></span>

<span data-ttu-id="ffe82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffe82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ffe82-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffe82-109">Permission type</span></span>                        | <span data-ttu-id="ffe82-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffe82-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ffe82-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffe82-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ffe82-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffe82-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ffe82-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffe82-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffe82-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffe82-114">Not supported.</span></span>                           |
| <span data-ttu-id="ffe82-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffe82-115">Application</span></span>                            | <span data-ttu-id="ffe82-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffe82-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ffe82-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffe82-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ffe82-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ffe82-118">Function parameters</span></span>

<span data-ttu-id="ffe82-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ffe82-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ffe82-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="ffe82-120">Parameter</span></span> | <span data-ttu-id="ffe82-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ffe82-121">Type</span></span>   | <span data-ttu-id="ffe82-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ffe82-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ffe82-123">period</span><span class="sxs-lookup"><span data-stu-id="ffe82-123">period</span></span>    | <span data-ttu-id="ffe82-124">string</span><span class="sxs-lookup"><span data-stu-id="ffe82-124">string</span></span> | <span data-ttu-id="ffe82-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ffe82-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ffe82-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ffe82-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ffe82-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ffe82-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ffe82-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffe82-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ffe82-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffe82-129">Request headers</span></span>

| <span data-ttu-id="ffe82-130">Имя</span><span class="sxs-lookup"><span data-stu-id="ffe82-130">Name</span></span>          | <span data-ttu-id="ffe82-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ffe82-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ffe82-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffe82-132">Authorization</span></span> | <span data-ttu-id="ffe82-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffe82-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ffe82-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ffe82-135">If-None-Match</span></span> | <span data-ttu-id="ffe82-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="ffe82-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ffe82-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ffe82-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ffe82-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffe82-138">Response</span></span>

<span data-ttu-id="ffe82-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ffe82-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ffe82-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ffe82-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ffe82-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ffe82-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ffe82-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ffe82-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ffe82-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ffe82-143">Report Refresh Date</span></span>
- <span data-ttu-id="ffe82-144">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="ffe82-144">Total</span></span>
- <span data-ttu-id="ffe82-145">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="ffe82-145">Active</span></span>
- <span data-ttu-id="ffe82-146">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="ffe82-146">Report Date</span></span>
- <span data-ttu-id="ffe82-147">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="ffe82-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ffe82-148">Пример</span><span class="sxs-lookup"><span data-stu-id="ffe82-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ffe82-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffe82-149">Request</span></span>

<span data-ttu-id="ffe82-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffe82-150">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ffe82-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffe82-151">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivitygroupcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityGroupCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ffe82-152">C#</span><span class="sxs-lookup"><span data-stu-id="ffe82-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitygroupcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ffe82-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffe82-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitygroupcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ffe82-154">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ffe82-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitygroupcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ffe82-155">Java</span><span class="sxs-lookup"><span data-stu-id="ffe82-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammergroupsactivitygroupcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ffe82-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffe82-156">Response</span></span>

<span data-ttu-id="ffe82-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ffe82-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="ffe82-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ffe82-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
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
