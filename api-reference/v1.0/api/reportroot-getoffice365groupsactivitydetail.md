---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Получите сведения об активности в группах Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: ac35137942b37c1c1c2faa1b20b341796a8668e6
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591294"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="202b3-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="202b3-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="202b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="202b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="202b3-105">Получите сведения об активности в группах Office 365.</span><span class="sxs-lookup"><span data-stu-id="202b3-105">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="202b3-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="202b3-106">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="202b3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="202b3-107">Permissions</span></span>

<span data-ttu-id="202b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="202b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="202b3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="202b3-110">Permission type</span></span>                        | <span data-ttu-id="202b3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="202b3-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="202b3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="202b3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="202b3-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="202b3-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="202b3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="202b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="202b3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202b3-115">Not supported.</span></span>                           |
| <span data-ttu-id="202b3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="202b3-116">Application</span></span>                            | <span data-ttu-id="202b3-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="202b3-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="202b3-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="202b3-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="202b3-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="202b3-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="202b3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="202b3-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="202b3-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="202b3-121">Function parameters</span></span>

<span data-ttu-id="202b3-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="202b3-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="202b3-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="202b3-123">Parameter</span></span> | <span data-ttu-id="202b3-124">Тип</span><span class="sxs-lookup"><span data-stu-id="202b3-124">Type</span></span>   | <span data-ttu-id="202b3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="202b3-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="202b3-126">period</span><span class="sxs-lookup"><span data-stu-id="202b3-126">period</span></span>    | <span data-ttu-id="202b3-127">string</span><span class="sxs-lookup"><span data-stu-id="202b3-127">string</span></span> | <span data-ttu-id="202b3-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="202b3-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="202b3-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="202b3-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="202b3-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="202b3-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="202b3-131">date</span><span class="sxs-lookup"><span data-stu-id="202b3-131">date</span></span>      | <span data-ttu-id="202b3-132">Date</span><span class="sxs-lookup"><span data-stu-id="202b3-132">Date</span></span>   | <span data-ttu-id="202b3-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="202b3-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="202b3-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="202b3-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="202b3-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="202b3-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="202b3-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="202b3-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="202b3-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="202b3-137">Request headers</span></span>

| <span data-ttu-id="202b3-138">Имя</span><span class="sxs-lookup"><span data-stu-id="202b3-138">Name</span></span>          | <span data-ttu-id="202b3-139">Описание</span><span class="sxs-lookup"><span data-stu-id="202b3-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="202b3-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="202b3-140">Authorization</span></span> | <span data-ttu-id="202b3-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="202b3-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="202b3-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="202b3-143">If-None-Match</span></span> | <span data-ttu-id="202b3-144">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="202b3-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="202b3-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="202b3-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="202b3-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="202b3-146">Response</span></span>

<span data-ttu-id="202b3-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="202b3-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="202b3-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="202b3-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="202b3-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="202b3-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="202b3-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="202b3-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="202b3-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="202b3-151">Report Refresh Date</span></span>
- <span data-ttu-id="202b3-152">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="202b3-152">Group Display Name</span></span>
- <span data-ttu-id="202b3-153">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="202b3-153">Is Deleted</span></span>
- <span data-ttu-id="202b3-154">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="202b3-154">Owner Principal Name</span></span>
- <span data-ttu-id="202b3-155">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="202b3-155">Last Activity Date</span></span>
- <span data-ttu-id="202b3-156">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="202b3-156">Group Type</span></span>
- <span data-ttu-id="202b3-157">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="202b3-157">Member Count</span></span>
- <span data-ttu-id="202b3-158">External Member Count (количество внешних участников)</span><span class="sxs-lookup"><span data-stu-id="202b3-158">External Member Count</span></span>
- <span data-ttu-id="202b3-159">Exchange Received Email Count (количество полученных сообщений Exchange)</span><span class="sxs-lookup"><span data-stu-id="202b3-159">Exchange Received Email Count</span></span>
- <span data-ttu-id="202b3-160">SharePoint Active File Count (количество активных файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="202b3-160">SharePoint Active File Count</span></span>
- <span data-ttu-id="202b3-161">Yammer Posted Message Count (количество опубликованных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="202b3-161">Yammer Posted Message Count</span></span>
- <span data-ttu-id="202b3-162">Yammer Read Message Count (количество прочитанных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="202b3-162">Yammer Read Message Count</span></span>
- <span data-ttu-id="202b3-163">Yammer Liked Message Count (количество понравившихся сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="202b3-163">Yammer Liked Message Count</span></span>
- <span data-ttu-id="202b3-164">Exchange Mailbox Total Item Count (общее количество элементов в почтовых ящиках Exchange)</span><span class="sxs-lookup"><span data-stu-id="202b3-164">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="202b3-165">Exchange Mailbox Storage Used (Byte) [занято почтовыми ящиками Exchange (байт)]</span><span class="sxs-lookup"><span data-stu-id="202b3-165">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="202b3-166">SharePoint Total File Count (общее количество файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="202b3-166">SharePoint Total File Count</span></span>
- <span data-ttu-id="202b3-167">SharePoint Site Storage Used (Byte) [занято сайтами SharePoint (байт)]</span><span class="sxs-lookup"><span data-stu-id="202b3-167">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="202b3-168">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="202b3-168">Group Id</span></span>
- <span data-ttu-id="202b3-169">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="202b3-169">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="202b3-170">Пример</span><span class="sxs-lookup"><span data-stu-id="202b3-170">Example</span></span>

#### <a name="request"></a><span data-ttu-id="202b3-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="202b3-171">Request</span></span>

<span data-ttu-id="202b3-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="202b3-172">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="202b3-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="202b3-173">Response</span></span>

<span data-ttu-id="202b3-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="202b3-174">The following is an example of the response.</span></span>

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

<span data-ttu-id="202b3-175">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="202b3-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
