---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: Получите сведения о количестве пользователей в день с разбивкой по типам устройств.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: ff2a159bbb5570728f935ad04f889edcb0cbc041
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021595"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="f7d31-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="f7d31-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="f7d31-104">Получите сведения о количестве пользователей в день с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="f7d31-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="f7d31-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="f7d31-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7d31-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7d31-106">Permissions</span></span>

<span data-ttu-id="f7d31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7d31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7d31-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7d31-109">Permission type</span></span>                        | <span data-ttu-id="f7d31-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7d31-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f7d31-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7d31-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7d31-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7d31-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f7d31-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7d31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7d31-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7d31-114">Not supported.</span></span>                           |
| <span data-ttu-id="f7d31-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7d31-115">Application</span></span>                            | <span data-ttu-id="f7d31-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7d31-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f7d31-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7d31-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f7d31-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7d31-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f7d31-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="f7d31-119">Function parameters</span></span>

<span data-ttu-id="f7d31-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="f7d31-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f7d31-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="f7d31-121">Parameter</span></span> | <span data-ttu-id="f7d31-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f7d31-122">Type</span></span>   | <span data-ttu-id="f7d31-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f7d31-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f7d31-124">period</span><span class="sxs-lookup"><span data-stu-id="f7d31-124">period</span></span>    | <span data-ttu-id="f7d31-125">string</span><span class="sxs-lookup"><span data-stu-id="f7d31-125">string</span></span> | <span data-ttu-id="f7d31-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f7d31-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f7d31-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="f7d31-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f7d31-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="f7d31-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f7d31-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7d31-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f7d31-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7d31-130">Request headers</span></span>

| <span data-ttu-id="f7d31-131">Имя</span><span class="sxs-lookup"><span data-stu-id="f7d31-131">Name</span></span>          | <span data-ttu-id="f7d31-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7d31-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f7d31-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7d31-133">Authorization</span></span> | <span data-ttu-id="f7d31-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7d31-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f7d31-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f7d31-136">If-None-Match</span></span> | <span data-ttu-id="f7d31-137">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="f7d31-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f7d31-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f7d31-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f7d31-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7d31-139">Response</span></span>

<span data-ttu-id="f7d31-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="f7d31-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f7d31-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="f7d31-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f7d31-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f7d31-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f7d31-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="f7d31-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f7d31-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="f7d31-144">Report Refresh Date</span></span>
- <span data-ttu-id="f7d31-145">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="f7d31-145">Web</span></span>
- <span data-ttu-id="f7d31-146">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="f7d31-146">Windows Phone</span></span>
- <span data-ttu-id="f7d31-147">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="f7d31-147">Android Phone</span></span>
- <span data-ttu-id="f7d31-148">iPhone</span><span class="sxs-lookup"><span data-stu-id="f7d31-148">iPhone</span></span>
- <span data-ttu-id="f7d31-149">iPad</span><span class="sxs-lookup"><span data-stu-id="f7d31-149">iPad</span></span>
- <span data-ttu-id="f7d31-150">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="f7d31-150">Other</span></span>
- <span data-ttu-id="f7d31-151">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="f7d31-151">Report Date</span></span>
- <span data-ttu-id="f7d31-152">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="f7d31-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f7d31-153">Пример</span><span class="sxs-lookup"><span data-stu-id="f7d31-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f7d31-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7d31-154">Request</span></span>

<span data-ttu-id="f7d31-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7d31-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7d31-156">C#</span><span class="sxs-lookup"><span data-stu-id="f7d31-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7d31-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="f7d31-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7d31-158">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f7d31-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f7d31-159">Java</span><span class="sxs-lookup"><span data-stu-id="f7d31-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammerdeviceusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f7d31-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7d31-160">Response</span></span>

<span data-ttu-id="f7d31-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7d31-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="f7d31-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="f7d31-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
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
