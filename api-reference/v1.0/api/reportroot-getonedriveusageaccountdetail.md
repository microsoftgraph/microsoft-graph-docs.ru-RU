---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Получите сведения об использовании OneDrive с разбивкой по учетным записям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b1fb1c43b5f9c5ecc1a1f62106e781e0b3dca2e1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371639"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="576e3-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="576e3-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

<span data-ttu-id="576e3-104">Получите сведения об использовании OneDrive с разбивкой по учетным записям.</span><span class="sxs-lookup"><span data-stu-id="576e3-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="576e3-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="576e3-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="576e3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="576e3-106">Permissions</span></span>

<span data-ttu-id="576e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="576e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="576e3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="576e3-109">Permission type</span></span>                        | <span data-ttu-id="576e3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="576e3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="576e3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="576e3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="576e3-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="576e3-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="576e3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="576e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="576e3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="576e3-114">Not supported.</span></span>                           |
| <span data-ttu-id="576e3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="576e3-115">Application</span></span>                            | <span data-ttu-id="576e3-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="576e3-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="576e3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="576e3-117">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="576e3-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="576e3-118">Function parameters</span></span>

<span data-ttu-id="576e3-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="576e3-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="576e3-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="576e3-120">Parameter</span></span> | <span data-ttu-id="576e3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="576e3-121">Type</span></span>   | <span data-ttu-id="576e3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="576e3-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="576e3-123">period</span><span class="sxs-lookup"><span data-stu-id="576e3-123">period</span></span>    | <span data-ttu-id="576e3-124">string</span><span class="sxs-lookup"><span data-stu-id="576e3-124">string</span></span> | <span data-ttu-id="576e3-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="576e3-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="576e3-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="576e3-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="576e3-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="576e3-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="576e3-128">date</span><span class="sxs-lookup"><span data-stu-id="576e3-128">date</span></span>      | <span data-ttu-id="576e3-129">Date</span><span class="sxs-lookup"><span data-stu-id="576e3-129">Date</span></span>   | <span data-ttu-id="576e3-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="576e3-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="576e3-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="576e3-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="576e3-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="576e3-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="576e3-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="576e3-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="576e3-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="576e3-134">Request headers</span></span>

| <span data-ttu-id="576e3-135">Имя</span><span class="sxs-lookup"><span data-stu-id="576e3-135">Name</span></span>          | <span data-ttu-id="576e3-136">Описание</span><span class="sxs-lookup"><span data-stu-id="576e3-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="576e3-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="576e3-137">Authorization</span></span> | <span data-ttu-id="576e3-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="576e3-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="576e3-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="576e3-140">If-None-Match</span></span> | <span data-ttu-id="576e3-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="576e3-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="576e3-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="576e3-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="576e3-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="576e3-143">Response</span></span>

<span data-ttu-id="576e3-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="576e3-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="576e3-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="576e3-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="576e3-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="576e3-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="576e3-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="576e3-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="576e3-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="576e3-148">Report Refresh Date</span></span>
- <span data-ttu-id="576e3-149">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="576e3-149">Site URL</span></span>
- <span data-ttu-id="576e3-150">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="576e3-150">Owner Display Name</span></span>
- <span data-ttu-id="576e3-151">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="576e3-151">Is Deleted</span></span>
- <span data-ttu-id="576e3-152">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="576e3-152">Last Activity Date</span></span>
- <span data-ttu-id="576e3-153">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="576e3-153">File Count</span></span>
- <span data-ttu-id="576e3-154">Active File Count (количество активных файлов)</span><span class="sxs-lookup"><span data-stu-id="576e3-154">Active File Count</span></span>
- <span data-ttu-id="576e3-155">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="576e3-155">Storage Used (Byte)</span></span>
- <span data-ttu-id="576e3-156">Storage Allocated (Byte) [выделено (байт)]</span><span class="sxs-lookup"><span data-stu-id="576e3-156">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="576e3-157">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="576e3-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="576e3-158">Пример</span><span class="sxs-lookup"><span data-stu-id="576e3-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="576e3-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="576e3-159">Request</span></span>

<span data-ttu-id="576e3-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="576e3-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="576e3-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="576e3-161">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="576e3-162">C#</span><span class="sxs-lookup"><span data-stu-id="576e3-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="576e3-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="576e3-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="576e3-164">Цель — C</span><span class="sxs-lookup"><span data-stu-id="576e3-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="576e3-165">Java</span><span class="sxs-lookup"><span data-stu-id="576e3-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="576e3-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="576e3-166">Response</span></span>

<span data-ttu-id="576e3-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="576e3-167">The following is an example of the response.</span></span>

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

<span data-ttu-id="576e3-168">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="576e3-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Report Period
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
