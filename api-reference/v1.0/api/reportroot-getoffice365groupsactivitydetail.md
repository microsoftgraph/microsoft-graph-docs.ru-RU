---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Получите сведения об активности в группах Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a1803b9c92054126161329dc997e5270bcca6cf6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445214"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="dd839-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="dd839-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="dd839-104">Получите сведения об активности в группах Office 365.</span><span class="sxs-lookup"><span data-stu-id="dd839-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="dd839-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="dd839-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd839-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd839-106">Permissions</span></span>

<span data-ttu-id="dd839-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd839-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd839-109">Permission type</span></span>                        | <span data-ttu-id="dd839-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd839-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dd839-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd839-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd839-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd839-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dd839-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd839-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd839-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd839-114">Not supported.</span></span>                           |
| <span data-ttu-id="dd839-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd839-115">Application</span></span>                            | <span data-ttu-id="dd839-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd839-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dd839-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd839-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dd839-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd839-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="dd839-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="dd839-119">Function parameters</span></span>

<span data-ttu-id="dd839-120">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="dd839-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="dd839-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="dd839-121">Parameter</span></span> | <span data-ttu-id="dd839-122">Тип</span><span class="sxs-lookup"><span data-stu-id="dd839-122">Type</span></span>   | <span data-ttu-id="dd839-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dd839-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dd839-124">period</span><span class="sxs-lookup"><span data-stu-id="dd839-124">period</span></span>    | <span data-ttu-id="dd839-125">string</span><span class="sxs-lookup"><span data-stu-id="dd839-125">string</span></span> | <span data-ttu-id="dd839-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="dd839-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dd839-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="dd839-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dd839-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="dd839-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="dd839-129">date</span><span class="sxs-lookup"><span data-stu-id="dd839-129">date</span></span>      | <span data-ttu-id="dd839-130">Date</span><span class="sxs-lookup"><span data-stu-id="dd839-130">Date</span></span>   | <span data-ttu-id="dd839-131">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="dd839-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="dd839-132">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="dd839-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="dd839-133">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="dd839-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="dd839-134">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="dd839-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd839-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd839-135">Request headers</span></span>

| <span data-ttu-id="dd839-136">Имя</span><span class="sxs-lookup"><span data-stu-id="dd839-136">Name</span></span>          | <span data-ttu-id="dd839-137">Описание</span><span class="sxs-lookup"><span data-stu-id="dd839-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="dd839-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd839-138">Authorization</span></span> | <span data-ttu-id="dd839-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd839-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="dd839-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="dd839-141">If-None-Match</span></span> | <span data-ttu-id="dd839-142">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="dd839-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="dd839-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="dd839-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="dd839-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd839-144">Response</span></span>

<span data-ttu-id="dd839-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="dd839-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dd839-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="dd839-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dd839-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="dd839-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dd839-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="dd839-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dd839-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="dd839-149">Report Refresh Date</span></span>
- <span data-ttu-id="dd839-150">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="dd839-150">Group Display Name</span></span>
- <span data-ttu-id="dd839-151">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="dd839-151">Is Deleted</span></span>
- <span data-ttu-id="dd839-152">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="dd839-152">Owner Principal Name</span></span>
- <span data-ttu-id="dd839-153">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="dd839-153">Last Activity Date</span></span>
- <span data-ttu-id="dd839-154">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="dd839-154">Group Type</span></span>
- <span data-ttu-id="dd839-155">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="dd839-155">Member Count</span></span>
- <span data-ttu-id="dd839-156">External Member Count (количество внешних участников)</span><span class="sxs-lookup"><span data-stu-id="dd839-156">External Member Count</span></span>
- <span data-ttu-id="dd839-157">Exchange Received Email Count (количество полученных сообщений Exchange)</span><span class="sxs-lookup"><span data-stu-id="dd839-157">Exchange Received Email Count</span></span>
- <span data-ttu-id="dd839-158">SharePoint Active File Count (количество активных файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="dd839-158">SharePoint Active File Count</span></span>
- <span data-ttu-id="dd839-159">Yammer Posted Message Count (количество опубликованных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="dd839-159">Yammer Posted Message Count</span></span>
- <span data-ttu-id="dd839-160">Yammer Read Message Count (количество прочитанных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="dd839-160">Yammer Read Message Count</span></span>
- <span data-ttu-id="dd839-161">Yammer Liked Message Count (количество понравившихся сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="dd839-161">Yammer Liked Message Count</span></span>
- <span data-ttu-id="dd839-162">Exchange Mailbox Total Item Count (общее количество элементов в почтовых ящиках Exchange)</span><span class="sxs-lookup"><span data-stu-id="dd839-162">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="dd839-163">Exchange Mailbox Storage Used (Byte) [занято почтовыми ящиками Exchange (байт)]</span><span class="sxs-lookup"><span data-stu-id="dd839-163">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="dd839-164">SharePoint Total File Count (общее количество файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="dd839-164">SharePoint Total File Count</span></span>
- <span data-ttu-id="dd839-165">SharePoint Site Storage Used (Byte) [занято сайтами SharePoint (байт)]</span><span class="sxs-lookup"><span data-stu-id="dd839-165">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="dd839-166">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="dd839-166">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="dd839-167">Пример</span><span class="sxs-lookup"><span data-stu-id="dd839-167">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dd839-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd839-168">Request</span></span>

<span data-ttu-id="dd839-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd839-169">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dd839-170">C#</span><span class="sxs-lookup"><span data-stu-id="dd839-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd839-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="dd839-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dd839-172">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dd839-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dd839-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd839-173">Response</span></span>

<span data-ttu-id="dd839-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd839-174">The following is an example of the response.</span></span>

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

<span data-ttu-id="dd839-175">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="dd839-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
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
