---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Получите сведения о действиях в OneDrive с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e152bf466ce1065e6b323523a6aa5771720a2eaf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35452503"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="d00db-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="d00db-103">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="d00db-104">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="d00db-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="d00db-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="d00db-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="d00db-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d00db-106">Permissions</span></span>

<span data-ttu-id="d00db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d00db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d00db-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d00db-109">Permission type</span></span>                        | <span data-ttu-id="d00db-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d00db-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d00db-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d00db-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d00db-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d00db-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d00db-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d00db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d00db-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d00db-114">Not supported.</span></span>                           |
| <span data-ttu-id="d00db-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d00db-115">Application</span></span>                            | <span data-ttu-id="d00db-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d00db-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d00db-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d00db-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d00db-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="d00db-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="d00db-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="d00db-119">Function parameters</span></span>

<span data-ttu-id="d00db-120">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="d00db-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d00db-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="d00db-121">Parameter</span></span> | <span data-ttu-id="d00db-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d00db-122">Type</span></span>   | <span data-ttu-id="d00db-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d00db-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d00db-124">period</span><span class="sxs-lookup"><span data-stu-id="d00db-124">period</span></span>    | <span data-ttu-id="d00db-125">string</span><span class="sxs-lookup"><span data-stu-id="d00db-125">string</span></span> | <span data-ttu-id="d00db-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="d00db-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d00db-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="d00db-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d00db-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="d00db-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d00db-129">date</span><span class="sxs-lookup"><span data-stu-id="d00db-129">date</span></span>      | <span data-ttu-id="d00db-130">Date</span><span class="sxs-lookup"><span data-stu-id="d00db-130">Date</span></span>   | <span data-ttu-id="d00db-131">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="d00db-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d00db-132">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="d00db-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d00db-133">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="d00db-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d00db-134">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="d00db-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d00db-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d00db-135">Request headers</span></span>

| <span data-ttu-id="d00db-136">Имя</span><span class="sxs-lookup"><span data-stu-id="d00db-136">Name</span></span>          | <span data-ttu-id="d00db-137">Описание</span><span class="sxs-lookup"><span data-stu-id="d00db-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d00db-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d00db-138">Authorization</span></span> | <span data-ttu-id="d00db-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d00db-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d00db-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d00db-141">If-None-Match</span></span> | <span data-ttu-id="d00db-142">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="d00db-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d00db-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d00db-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d00db-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d00db-144">Response</span></span>

<span data-ttu-id="d00db-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="d00db-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d00db-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="d00db-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d00db-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d00db-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d00db-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="d00db-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d00db-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="d00db-149">Report Refresh Date</span></span>
- <span data-ttu-id="d00db-150">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="d00db-150">User Principal Name</span></span>
- <span data-ttu-id="d00db-151">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="d00db-151">Is Deleted</span></span>
- <span data-ttu-id="d00db-152">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="d00db-152">Deleted Date</span></span>
- <span data-ttu-id="d00db-153">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="d00db-153">Last Activity Date</span></span>
- <span data-ttu-id="d00db-154">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="d00db-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="d00db-155">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="d00db-155">Synced File Count</span></span>
- <span data-ttu-id="d00db-156">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="d00db-156">Shared Internally File Count</span></span>
- <span data-ttu-id="d00db-157">"Shared Externally File Count" (Количество файлов, к которым предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="d00db-157">Shared Externally File Count</span></span>
- <span data-ttu-id="d00db-158">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="d00db-158">Assigned Products</span></span>
- <span data-ttu-id="d00db-159">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="d00db-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d00db-160">Пример</span><span class="sxs-lookup"><span data-stu-id="d00db-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d00db-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="d00db-161">Request</span></span>

<span data-ttu-id="d00db-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d00db-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d00db-163">C#</span><span class="sxs-lookup"><span data-stu-id="d00db-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d00db-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="d00db-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d00db-165">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d00db-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d00db-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="d00db-166">Response</span></span>

<span data-ttu-id="d00db-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d00db-167">The following is an example of the response.</span></span>

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

<span data-ttu-id="d00db-168">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="d00db-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
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
