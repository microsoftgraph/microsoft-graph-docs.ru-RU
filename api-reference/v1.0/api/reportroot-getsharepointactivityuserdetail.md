---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Получите сведения об активности пользователей в SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9e68b0575965870ec971cff59dba4467e4ef8f95
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021818"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="fa5cf-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="fa5cf-103">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="fa5cf-104">Получите сведения об активности пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-104">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="fa5cf-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="fa5cf-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa5cf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa5cf-106">Permissions</span></span>

<span data-ttu-id="fa5cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa5cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa5cf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa5cf-109">Permission type</span></span>                        | <span data-ttu-id="fa5cf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa5cf-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fa5cf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa5cf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa5cf-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa5cf-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fa5cf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa5cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa5cf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-114">Not supported.</span></span>                           |
| <span data-ttu-id="fa5cf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa5cf-115">Application</span></span>                            | <span data-ttu-id="fa5cf-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa5cf-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fa5cf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa5cf-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fa5cf-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa5cf-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="fa5cf-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="fa5cf-119">Function parameters</span></span>

<span data-ttu-id="fa5cf-120">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="fa5cf-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="fa5cf-121">Parameter</span></span> | <span data-ttu-id="fa5cf-122">Тип</span><span class="sxs-lookup"><span data-stu-id="fa5cf-122">Type</span></span>   | <span data-ttu-id="fa5cf-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fa5cf-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fa5cf-124">period</span><span class="sxs-lookup"><span data-stu-id="fa5cf-124">period</span></span>    | <span data-ttu-id="fa5cf-125">string</span><span class="sxs-lookup"><span data-stu-id="fa5cf-125">string</span></span> | <span data-ttu-id="fa5cf-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fa5cf-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fa5cf-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="fa5cf-129">date</span><span class="sxs-lookup"><span data-stu-id="fa5cf-129">date</span></span>      | <span data-ttu-id="fa5cf-130">Date</span><span class="sxs-lookup"><span data-stu-id="fa5cf-130">Date</span></span>   | <span data-ttu-id="fa5cf-131">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="fa5cf-132">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="fa5cf-133">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="fa5cf-134">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa5cf-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa5cf-135">Request headers</span></span>

| <span data-ttu-id="fa5cf-136">Имя</span><span class="sxs-lookup"><span data-stu-id="fa5cf-136">Name</span></span>          | <span data-ttu-id="fa5cf-137">Описание</span><span class="sxs-lookup"><span data-stu-id="fa5cf-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="fa5cf-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa5cf-138">Authorization</span></span> | <span data-ttu-id="fa5cf-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="fa5cf-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="fa5cf-141">If-None-Match</span></span> | <span data-ttu-id="fa5cf-142">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="fa5cf-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fa5cf-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa5cf-144">Response</span></span>

<span data-ttu-id="fa5cf-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fa5cf-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fa5cf-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fa5cf-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="fa5cf-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fa5cf-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="fa5cf-149">Report Refresh Date</span></span>
- <span data-ttu-id="fa5cf-150">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="fa5cf-150">User Principal Name</span></span>
- <span data-ttu-id="fa5cf-151">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="fa5cf-151">Is Deleted</span></span>
- <span data-ttu-id="fa5cf-152">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="fa5cf-152">Deleted Date</span></span>
- <span data-ttu-id="fa5cf-153">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="fa5cf-153">Last Activity Date</span></span>
- <span data-ttu-id="fa5cf-154">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="fa5cf-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="fa5cf-155">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="fa5cf-155">Synced File Count</span></span>
- <span data-ttu-id="fa5cf-156">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="fa5cf-156">Shared Internally File Count</span></span>
- <span data-ttu-id="fa5cf-157">Shared Externally File Count (количество файлов, отправленных за пределы организации)</span><span class="sxs-lookup"><span data-stu-id="fa5cf-157">Shared Externally File Count</span></span>
- <span data-ttu-id="fa5cf-158">Visited Page Count (количество посещенных страниц)</span><span class="sxs-lookup"><span data-stu-id="fa5cf-158">Visited Page Count</span></span>
- <span data-ttu-id="fa5cf-159">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="fa5cf-159">Assigned Products</span></span>
- <span data-ttu-id="fa5cf-160">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="fa5cf-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fa5cf-161">Пример</span><span class="sxs-lookup"><span data-stu-id="fa5cf-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fa5cf-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa5cf-162">Request</span></span>

<span data-ttu-id="fa5cf-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-163">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa5cf-164">C#</span><span class="sxs-lookup"><span data-stu-id="fa5cf-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa5cf-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="fa5cf-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa5cf-166">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fa5cf-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fa5cf-167">Java</span><span class="sxs-lookup"><span data-stu-id="fa5cf-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fa5cf-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa5cf-168">Response</span></span>

<span data-ttu-id="fa5cf-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-169">The following is an example of the response.</span></span>

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

<span data-ttu-id="fa5cf-170">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="fa5cf-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
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
