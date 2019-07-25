---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Узнайте, сколько сотрудников организации используют уникальные устройства. В отчете будет показано количество пользователей устройств с Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8fbd031f91fba63069cac3a16595d3f46bc8ea8b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892479"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="33113-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="33113-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="33113-105">Узнайте, сколько сотрудников организации используют уникальные устройства.</span><span class="sxs-lookup"><span data-stu-id="33113-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="33113-106">В отчете будет показано количество пользователей Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.</span><span class="sxs-lookup"><span data-stu-id="33113-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="33113-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="33113-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="33113-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33113-108">Permissions</span></span>

<span data-ttu-id="33113-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33113-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="33113-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33113-111">Permission type</span></span>                        | <span data-ttu-id="33113-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33113-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="33113-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33113-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="33113-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="33113-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="33113-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33113-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33113-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33113-116">Not supported.</span></span>                           |
| <span data-ttu-id="33113-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33113-117">Application</span></span>                            | <span data-ttu-id="33113-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="33113-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="33113-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33113-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="33113-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="33113-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="33113-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="33113-121">Function parameters</span></span>

<span data-ttu-id="33113-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="33113-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="33113-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="33113-123">Parameter</span></span> | <span data-ttu-id="33113-124">Тип</span><span class="sxs-lookup"><span data-stu-id="33113-124">Type</span></span>   | <span data-ttu-id="33113-125">Описание</span><span class="sxs-lookup"><span data-stu-id="33113-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="33113-126">period</span><span class="sxs-lookup"><span data-stu-id="33113-126">period</span></span>    | <span data-ttu-id="33113-127">string</span><span class="sxs-lookup"><span data-stu-id="33113-127">string</span></span> | <span data-ttu-id="33113-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="33113-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="33113-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="33113-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="33113-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="33113-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="33113-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33113-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="33113-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33113-132">Request headers</span></span>

| <span data-ttu-id="33113-133">Имя</span><span class="sxs-lookup"><span data-stu-id="33113-133">Name</span></span>          | <span data-ttu-id="33113-134">Описание</span><span class="sxs-lookup"><span data-stu-id="33113-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="33113-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33113-135">Authorization</span></span> | <span data-ttu-id="33113-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33113-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="33113-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="33113-138">If-None-Match</span></span> | <span data-ttu-id="33113-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="33113-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="33113-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="33113-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="33113-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="33113-141">Response</span></span>

<span data-ttu-id="33113-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="33113-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="33113-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="33113-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="33113-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="33113-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="33113-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="33113-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="33113-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="33113-146">Report Refresh Date</span></span>
- <span data-ttu-id="33113-147">"Windows";</span><span class="sxs-lookup"><span data-stu-id="33113-147">Windows</span></span>
- <span data-ttu-id="33113-148">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="33113-148">Windows Phone</span></span>
- <span data-ttu-id="33113-149">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="33113-149">Android Phone</span></span>
- <span data-ttu-id="33113-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="33113-150">iPhone</span></span>
- <span data-ttu-id="33113-151">iPad</span><span class="sxs-lookup"><span data-stu-id="33113-151">iPad</span></span>
- <span data-ttu-id="33113-152">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="33113-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="33113-153">Пример</span><span class="sxs-lookup"><span data-stu-id="33113-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="33113-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="33113-154">Request</span></span>

<span data-ttu-id="33113-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33113-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="33113-156">C#</span><span class="sxs-lookup"><span data-stu-id="33113-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33113-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="33113-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33113-158">Цель — C</span><span class="sxs-lookup"><span data-stu-id="33113-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="33113-159">Java</span><span class="sxs-lookup"><span data-stu-id="33113-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="33113-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="33113-160">Response</span></span>

<span data-ttu-id="33113-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="33113-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="33113-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="33113-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
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
