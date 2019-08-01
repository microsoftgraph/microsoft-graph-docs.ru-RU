---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: Получение сведений об использовании сайтов SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 20e407dbc089f8ea62cd7b8c0ec63fbedb2d385a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021855"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="46c2b-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="46c2b-103">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="46c2b-104">Получение сведений об использовании сайтов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="46c2b-104">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="46c2b-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="46c2b-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="46c2b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46c2b-106">Permissions</span></span>

<span data-ttu-id="46c2b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46c2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46c2b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46c2b-109">Permission type</span></span>                        | <span data-ttu-id="46c2b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46c2b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="46c2b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46c2b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="46c2b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="46c2b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="46c2b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46c2b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46c2b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46c2b-114">Not supported.</span></span>                           |
| <span data-ttu-id="46c2b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46c2b-115">Application</span></span>                            | <span data-ttu-id="46c2b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="46c2b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="46c2b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46c2b-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="46c2b-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="46c2b-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="46c2b-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="46c2b-119">Function parameters</span></span>

<span data-ttu-id="46c2b-120">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="46c2b-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="46c2b-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="46c2b-121">Parameter</span></span> | <span data-ttu-id="46c2b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="46c2b-122">Type</span></span>   | <span data-ttu-id="46c2b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="46c2b-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="46c2b-124">period</span><span class="sxs-lookup"><span data-stu-id="46c2b-124">period</span></span>    | <span data-ttu-id="46c2b-125">string</span><span class="sxs-lookup"><span data-stu-id="46c2b-125">string</span></span> | <span data-ttu-id="46c2b-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="46c2b-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="46c2b-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="46c2b-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="46c2b-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="46c2b-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="46c2b-129">date</span><span class="sxs-lookup"><span data-stu-id="46c2b-129">date</span></span>      | <span data-ttu-id="46c2b-130">Date</span><span class="sxs-lookup"><span data-stu-id="46c2b-130">Date</span></span>   | <span data-ttu-id="46c2b-131">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="46c2b-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="46c2b-132">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="46c2b-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="46c2b-133">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="46c2b-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="46c2b-134">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="46c2b-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46c2b-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46c2b-135">Request headers</span></span>

| <span data-ttu-id="46c2b-136">Имя</span><span class="sxs-lookup"><span data-stu-id="46c2b-136">Name</span></span>          | <span data-ttu-id="46c2b-137">Описание</span><span class="sxs-lookup"><span data-stu-id="46c2b-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="46c2b-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46c2b-138">Authorization</span></span> | <span data-ttu-id="46c2b-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46c2b-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="46c2b-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="46c2b-141">If-None-Match</span></span> | <span data-ttu-id="46c2b-142">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="46c2b-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="46c2b-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="46c2b-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="46c2b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="46c2b-144">Response</span></span>

<span data-ttu-id="46c2b-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="46c2b-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="46c2b-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="46c2b-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="46c2b-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="46c2b-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="46c2b-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="46c2b-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="46c2b-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="46c2b-149">Report Refresh Date</span></span>
- <span data-ttu-id="46c2b-150">Идентификатор сайта</span><span class="sxs-lookup"><span data-stu-id="46c2b-150">Site Id</span></span>
- <span data-ttu-id="46c2b-151">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="46c2b-151">Site URL</span></span>
- <span data-ttu-id="46c2b-152">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="46c2b-152">Owner Display Name</span></span>
- <span data-ttu-id="46c2b-153">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="46c2b-153">Is Deleted</span></span>
- <span data-ttu-id="46c2b-154">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="46c2b-154">Last Activity Date</span></span>
- <span data-ttu-id="46c2b-155">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="46c2b-155">File Count</span></span>
- <span data-ttu-id="46c2b-156">"Active File Count" (Количество активных файлов);</span><span class="sxs-lookup"><span data-stu-id="46c2b-156">Active File Count</span></span>
- <span data-ttu-id="46c2b-157">"Page View Count" (Количество просмотров страницы);</span><span class="sxs-lookup"><span data-stu-id="46c2b-157">Page View Count</span></span>
- <span data-ttu-id="46c2b-158">"Visited Page Count" (Количество посещенных страниц);</span><span class="sxs-lookup"><span data-stu-id="46c2b-158">Visited Page Count</span></span>
- <span data-ttu-id="46c2b-159">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="46c2b-159">Storage Used (Byte)</span></span>
- <span data-ttu-id="46c2b-160">"Storage Allocated (Byte)" (Объем выделенного хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="46c2b-160">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="46c2b-161">"Root Web Template" (Шаблон корневого веб-сайта);</span><span class="sxs-lookup"><span data-stu-id="46c2b-161">Root Web Template</span></span>
- <span data-ttu-id="46c2b-162">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="46c2b-162">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="46c2b-163">Пример</span><span class="sxs-lookup"><span data-stu-id="46c2b-163">Example</span></span>

#### <a name="request"></a><span data-ttu-id="46c2b-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="46c2b-164">Request</span></span>

<span data-ttu-id="46c2b-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46c2b-165">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46c2b-166">C#</span><span class="sxs-lookup"><span data-stu-id="46c2b-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46c2b-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="46c2b-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46c2b-168">Цель — C</span><span class="sxs-lookup"><span data-stu-id="46c2b-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="46c2b-169">Java</span><span class="sxs-lookup"><span data-stu-id="46c2b-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="46c2b-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="46c2b-170">Response</span></span>

<span data-ttu-id="46c2b-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="46c2b-171">The following is an example of the response.</span></span>

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

<span data-ttu-id="46c2b-172">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="46c2b-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Report Period
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
