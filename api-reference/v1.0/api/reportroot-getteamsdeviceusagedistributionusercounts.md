---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 79f0e776426179b63fbe75fd0cfac465927f642f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277191"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="ce0ce-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="ce0ce-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="ce0ce-104">Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce0ce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce0ce-105">Permissions</span></span>

<span data-ttu-id="ce0ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce0ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce0ce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce0ce-108">Permission type</span></span>                        | <span data-ttu-id="ce0ce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce0ce-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ce0ce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce0ce-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce0ce-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce0ce-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ce0ce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce0ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce0ce-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-113">Not supported.</span></span>                           |
| <span data-ttu-id="ce0ce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce0ce-114">Application</span></span>                            | <span data-ttu-id="ce0ce-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce0ce-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ce0ce-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce0ce-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ce0ce-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ce0ce-117">Function parameters</span></span>

<span data-ttu-id="ce0ce-118">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ce0ce-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="ce0ce-119">Parameter</span></span> | <span data-ttu-id="ce0ce-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ce0ce-120">Type</span></span>   | <span data-ttu-id="ce0ce-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ce0ce-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ce0ce-122">period</span><span class="sxs-lookup"><span data-stu-id="ce0ce-122">period</span></span>    | <span data-ttu-id="ce0ce-123">string</span><span class="sxs-lookup"><span data-stu-id="ce0ce-123">string</span></span> | <span data-ttu-id="ce0ce-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ce0ce-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ce0ce-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ce0ce-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ce0ce-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce0ce-128">Request headers</span></span>

| <span data-ttu-id="ce0ce-129">Имя</span><span class="sxs-lookup"><span data-stu-id="ce0ce-129">Name</span></span>          | <span data-ttu-id="ce0ce-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ce0ce-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ce0ce-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce0ce-131">Authorization</span></span> | <span data-ttu-id="ce0ce-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ce0ce-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce0ce-134">Response</span></span>

<span data-ttu-id="ce0ce-135">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-135">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ce0ce-136">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-136">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ce0ce-137">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-137">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ce0ce-138">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ce0ce-138">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="ce0ce-139">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ce0ce-139">Report Refresh Date</span></span>
- <span data-ttu-id="ce0ce-140">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="ce0ce-140">Web</span></span>
- <span data-ttu-id="ce0ce-141">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="ce0ce-141">Windows Phone</span></span>
- <span data-ttu-id="ce0ce-142">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="ce0ce-142">Android Phone</span></span>
- <span data-ttu-id="ce0ce-143">"iOS";</span><span class="sxs-lookup"><span data-stu-id="ce0ce-143">iOS</span></span>
- <span data-ttu-id="ce0ce-144">"Mac";</span><span class="sxs-lookup"><span data-stu-id="ce0ce-144">Mac</span></span>
- <span data-ttu-id="ce0ce-145">"Windows";</span><span class="sxs-lookup"><span data-stu-id="ce0ce-145">Windows</span></span>
- <span data-ttu-id="ce0ce-146">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="ce0ce-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ce0ce-147">Пример</span><span class="sxs-lookup"><span data-stu-id="ce0ce-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ce0ce-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce0ce-148">Request</span></span>

<span data-ttu-id="ce0ce-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ce0ce-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce0ce-150">Response</span></span>

<span data-ttu-id="ce0ce-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-151">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ce0ce-152">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ce0ce-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ce0ce-153">C#</span><span class="sxs-lookup"><span data-stu-id="ce0ce-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce0ce-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce0ce-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ce0ce-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ce0ce-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="ce0ce-156">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ce0ce-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
