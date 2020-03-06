---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: Получение сведений об использовании сайтов SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b027671861b77aa2c3b69e8d7c9aa180899691d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510223"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="dfffa-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="dfffa-103">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="dfffa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfffa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dfffa-105">Получение сведений об использовании сайтов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="dfffa-105">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="dfffa-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="dfffa-106">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="dfffa-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfffa-107">Permissions</span></span>

<span data-ttu-id="dfffa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfffa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfffa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfffa-110">Permission type</span></span>                        | <span data-ttu-id="dfffa-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfffa-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dfffa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfffa-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfffa-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfffa-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dfffa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfffa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfffa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfffa-115">Not supported.</span></span>                           |
| <span data-ttu-id="dfffa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfffa-116">Application</span></span>                            | <span data-ttu-id="dfffa-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfffa-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="dfffa-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dfffa-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="dfffa-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="dfffa-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="dfffa-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfffa-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="dfffa-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="dfffa-121">Function parameters</span></span>

<span data-ttu-id="dfffa-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="dfffa-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="dfffa-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="dfffa-123">Parameter</span></span> | <span data-ttu-id="dfffa-124">Тип</span><span class="sxs-lookup"><span data-stu-id="dfffa-124">Type</span></span>   | <span data-ttu-id="dfffa-125">Описание</span><span class="sxs-lookup"><span data-stu-id="dfffa-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dfffa-126">period</span><span class="sxs-lookup"><span data-stu-id="dfffa-126">period</span></span>    | <span data-ttu-id="dfffa-127">string</span><span class="sxs-lookup"><span data-stu-id="dfffa-127">string</span></span> | <span data-ttu-id="dfffa-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="dfffa-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dfffa-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="dfffa-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dfffa-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="dfffa-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="dfffa-131">date</span><span class="sxs-lookup"><span data-stu-id="dfffa-131">date</span></span>      | <span data-ttu-id="dfffa-132">Date</span><span class="sxs-lookup"><span data-stu-id="dfffa-132">Date</span></span>   | <span data-ttu-id="dfffa-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="dfffa-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="dfffa-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="dfffa-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="dfffa-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="dfffa-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="dfffa-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="dfffa-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfffa-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfffa-137">Request headers</span></span>

| <span data-ttu-id="dfffa-138">Имя</span><span class="sxs-lookup"><span data-stu-id="dfffa-138">Name</span></span>          | <span data-ttu-id="dfffa-139">Описание</span><span class="sxs-lookup"><span data-stu-id="dfffa-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="dfffa-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfffa-140">Authorization</span></span> | <span data-ttu-id="dfffa-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfffa-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="dfffa-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="dfffa-143">If-None-Match</span></span> | <span data-ttu-id="dfffa-144">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="dfffa-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="dfffa-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="dfffa-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="dfffa-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfffa-146">Response</span></span>

<span data-ttu-id="dfffa-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="dfffa-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dfffa-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="dfffa-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dfffa-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="dfffa-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dfffa-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="dfffa-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dfffa-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="dfffa-151">Report Refresh Date</span></span>
- <span data-ttu-id="dfffa-152">Идентификатор сайта</span><span class="sxs-lookup"><span data-stu-id="dfffa-152">Site Id</span></span>
- <span data-ttu-id="dfffa-153">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="dfffa-153">Site URL</span></span>
- <span data-ttu-id="dfffa-154">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="dfffa-154">Owner Display Name</span></span>
- <span data-ttu-id="dfffa-155">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="dfffa-155">Is Deleted</span></span>
- <span data-ttu-id="dfffa-156">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="dfffa-156">Last Activity Date</span></span>
- <span data-ttu-id="dfffa-157">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="dfffa-157">File Count</span></span>
- <span data-ttu-id="dfffa-158">"Active File Count" (Количество активных файлов);</span><span class="sxs-lookup"><span data-stu-id="dfffa-158">Active File Count</span></span>
- <span data-ttu-id="dfffa-159">"Page View Count" (Количество просмотров страницы);</span><span class="sxs-lookup"><span data-stu-id="dfffa-159">Page View Count</span></span>
- <span data-ttu-id="dfffa-160">"Visited Page Count" (Количество посещенных страниц);</span><span class="sxs-lookup"><span data-stu-id="dfffa-160">Visited Page Count</span></span>
- <span data-ttu-id="dfffa-161">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="dfffa-161">Storage Used (Byte)</span></span>
- <span data-ttu-id="dfffa-162">"Storage Allocated (Byte)" (Объем выделенного хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="dfffa-162">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="dfffa-163">"Root Web Template" (Шаблон корневого веб-сайта);</span><span class="sxs-lookup"><span data-stu-id="dfffa-163">Root Web Template</span></span>
- <span data-ttu-id="dfffa-164">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="dfffa-164">Owner Principal Name</span></span>
- <span data-ttu-id="dfffa-165">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="dfffa-165">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="dfffa-166">Пример</span><span class="sxs-lookup"><span data-stu-id="dfffa-166">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dfffa-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfffa-167">Request</span></span>

<span data-ttu-id="dfffa-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfffa-168">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dfffa-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfffa-169">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageDetail(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="dfffa-170">C#</span><span class="sxs-lookup"><span data-stu-id="dfffa-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfffa-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfffa-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfffa-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfffa-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfffa-173">Java</span><span class="sxs-lookup"><span data-stu-id="dfffa-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dfffa-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfffa-174">Response</span></span>

<span data-ttu-id="dfffa-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfffa-175">The following is an example of the response.</span></span>

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

<span data-ttu-id="dfffa-176">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="dfffa-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Owner Principal Name,Report Period
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
