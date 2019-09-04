---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Получите сведения об активности в группах Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: db7fee658e16f8331a8a3910f3a8ea014d35c407
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729695"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="35e4f-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="35e4f-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="35e4f-104">Получите сведения об активности в группах Office 365.</span><span class="sxs-lookup"><span data-stu-id="35e4f-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="35e4f-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="35e4f-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="35e4f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35e4f-106">Permissions</span></span>

<span data-ttu-id="35e4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35e4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35e4f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35e4f-109">Permission type</span></span>                        | <span data-ttu-id="35e4f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35e4f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="35e4f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35e4f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="35e4f-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="35e4f-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="35e4f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35e4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35e4f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35e4f-114">Not supported.</span></span>                           |
| <span data-ttu-id="35e4f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35e4f-115">Application</span></span>                            | <span data-ttu-id="35e4f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="35e4f-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="35e4f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35e4f-117">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="35e4f-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="35e4f-118">Function parameters</span></span>

<span data-ttu-id="35e4f-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="35e4f-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="35e4f-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="35e4f-120">Parameter</span></span> | <span data-ttu-id="35e4f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="35e4f-121">Type</span></span>   | <span data-ttu-id="35e4f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="35e4f-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="35e4f-123">period</span><span class="sxs-lookup"><span data-stu-id="35e4f-123">period</span></span>    | <span data-ttu-id="35e4f-124">string</span><span class="sxs-lookup"><span data-stu-id="35e4f-124">string</span></span> | <span data-ttu-id="35e4f-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="35e4f-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="35e4f-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="35e4f-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="35e4f-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="35e4f-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="35e4f-128">date</span><span class="sxs-lookup"><span data-stu-id="35e4f-128">date</span></span>      | <span data-ttu-id="35e4f-129">Date</span><span class="sxs-lookup"><span data-stu-id="35e4f-129">Date</span></span>   | <span data-ttu-id="35e4f-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="35e4f-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="35e4f-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="35e4f-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="35e4f-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="35e4f-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="35e4f-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="35e4f-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35e4f-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35e4f-134">Request headers</span></span>

| <span data-ttu-id="35e4f-135">Имя</span><span class="sxs-lookup"><span data-stu-id="35e4f-135">Name</span></span>          | <span data-ttu-id="35e4f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="35e4f-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="35e4f-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35e4f-137">Authorization</span></span> | <span data-ttu-id="35e4f-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35e4f-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="35e4f-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="35e4f-140">If-None-Match</span></span> | <span data-ttu-id="35e4f-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="35e4f-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="35e4f-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="35e4f-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="35e4f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="35e4f-143">Response</span></span>

<span data-ttu-id="35e4f-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="35e4f-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="35e4f-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="35e4f-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="35e4f-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="35e4f-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="35e4f-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="35e4f-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="35e4f-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="35e4f-148">Report Refresh Date</span></span>
- <span data-ttu-id="35e4f-149">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="35e4f-149">Group Display Name</span></span>
- <span data-ttu-id="35e4f-150">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="35e4f-150">Is Deleted</span></span>
- <span data-ttu-id="35e4f-151">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="35e4f-151">Owner Principal Name</span></span>
- <span data-ttu-id="35e4f-152">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="35e4f-152">Last Activity Date</span></span>
- <span data-ttu-id="35e4f-153">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="35e4f-153">Group Type</span></span>
- <span data-ttu-id="35e4f-154">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="35e4f-154">Member Count</span></span>
- <span data-ttu-id="35e4f-155">External Member Count (количество внешних участников)</span><span class="sxs-lookup"><span data-stu-id="35e4f-155">External Member Count</span></span>
- <span data-ttu-id="35e4f-156">Exchange Received Email Count (количество полученных сообщений Exchange)</span><span class="sxs-lookup"><span data-stu-id="35e4f-156">Exchange Received Email Count</span></span>
- <span data-ttu-id="35e4f-157">SharePoint Active File Count (количество активных файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="35e4f-157">SharePoint Active File Count</span></span>
- <span data-ttu-id="35e4f-158">Yammer Posted Message Count (количество опубликованных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="35e4f-158">Yammer Posted Message Count</span></span>
- <span data-ttu-id="35e4f-159">Yammer Read Message Count (количество прочитанных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="35e4f-159">Yammer Read Message Count</span></span>
- <span data-ttu-id="35e4f-160">Yammer Liked Message Count (количество понравившихся сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="35e4f-160">Yammer Liked Message Count</span></span>
- <span data-ttu-id="35e4f-161">Exchange Mailbox Total Item Count (общее количество элементов в почтовых ящиках Exchange)</span><span class="sxs-lookup"><span data-stu-id="35e4f-161">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="35e4f-162">Exchange Mailbox Storage Used (Byte) [занято почтовыми ящиками Exchange (байт)]</span><span class="sxs-lookup"><span data-stu-id="35e4f-162">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="35e4f-163">SharePoint Total File Count (общее количество файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="35e4f-163">SharePoint Total File Count</span></span>
- <span data-ttu-id="35e4f-164">SharePoint Site Storage Used (Byte) [занято сайтами SharePoint (байт)]</span><span class="sxs-lookup"><span data-stu-id="35e4f-164">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="35e4f-165">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="35e4f-165">Group Id</span></span>
- <span data-ttu-id="35e4f-166">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="35e4f-166">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="35e4f-167">Пример</span><span class="sxs-lookup"><span data-stu-id="35e4f-167">Example</span></span>

#### <a name="request"></a><span data-ttu-id="35e4f-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="35e4f-168">Request</span></span>

<span data-ttu-id="35e4f-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35e4f-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="35e4f-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="35e4f-170">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="35e4f-171">C#</span><span class="sxs-lookup"><span data-stu-id="35e4f-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35e4f-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35e4f-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="35e4f-173">Цель — C</span><span class="sxs-lookup"><span data-stu-id="35e4f-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="35e4f-174">Java</span><span class="sxs-lookup"><span data-stu-id="35e4f-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365groupsactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="35e4f-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="35e4f-175">Response</span></span>

<span data-ttu-id="35e4f-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="35e4f-176">The following is an example of the response.</span></span>

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

<span data-ttu-id="35e4f-177">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="35e4f-177">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Group Id,Report Period
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
