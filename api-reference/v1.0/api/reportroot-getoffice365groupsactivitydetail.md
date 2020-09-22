---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Получение сведений о действиях в группах Microsoft 365, сгруппированных по группам.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b53f50c976170a921d076eb56f599e23db878432
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083213"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="5b751-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="5b751-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="5b751-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b751-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b751-105">Получение сведений о действиях в группах Microsoft 365, сгруппированных по группам.</span><span class="sxs-lookup"><span data-stu-id="5b751-105">Get details about Microsoft 365 groups activity by group.</span></span>

> <span data-ttu-id="5b751-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье microsoft 365 Reports — microsoft 365 Groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="5b751-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b751-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b751-107">Permissions</span></span>

<span data-ttu-id="5b751-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b751-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b751-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b751-110">Permission type</span></span>                        | <span data-ttu-id="5b751-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b751-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5b751-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b751-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b751-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b751-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5b751-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b751-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b751-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b751-115">Not supported.</span></span>                           |
| <span data-ttu-id="5b751-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b751-116">Application</span></span>                            | <span data-ttu-id="5b751-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b751-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="5b751-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5b751-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5b751-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5b751-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5b751-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b751-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5b751-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="5b751-121">Function parameters</span></span>

<span data-ttu-id="5b751-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="5b751-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="5b751-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="5b751-123">Parameter</span></span> | <span data-ttu-id="5b751-124">Тип</span><span class="sxs-lookup"><span data-stu-id="5b751-124">Type</span></span>   | <span data-ttu-id="5b751-125">Описание</span><span class="sxs-lookup"><span data-stu-id="5b751-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5b751-126">period</span><span class="sxs-lookup"><span data-stu-id="5b751-126">period</span></span>    | <span data-ttu-id="5b751-127">string</span><span class="sxs-lookup"><span data-stu-id="5b751-127">string</span></span> | <span data-ttu-id="5b751-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5b751-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5b751-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="5b751-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5b751-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="5b751-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5b751-131">date</span><span class="sxs-lookup"><span data-stu-id="5b751-131">date</span></span>      | <span data-ttu-id="5b751-132">Date</span><span class="sxs-lookup"><span data-stu-id="5b751-132">Date</span></span>   | <span data-ttu-id="5b751-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="5b751-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5b751-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="5b751-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5b751-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="5b751-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5b751-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="5b751-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b751-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b751-137">Request headers</span></span>

| <span data-ttu-id="5b751-138">Имя</span><span class="sxs-lookup"><span data-stu-id="5b751-138">Name</span></span>          | <span data-ttu-id="5b751-139">Описание</span><span class="sxs-lookup"><span data-stu-id="5b751-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5b751-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b751-140">Authorization</span></span> | <span data-ttu-id="5b751-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b751-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5b751-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5b751-143">If-None-Match</span></span> | <span data-ttu-id="5b751-144">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="5b751-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5b751-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5b751-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5b751-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b751-146">Response</span></span>

<span data-ttu-id="5b751-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="5b751-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5b751-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="5b751-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5b751-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5b751-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5b751-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="5b751-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5b751-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="5b751-151">Report Refresh Date</span></span>
- <span data-ttu-id="5b751-152">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="5b751-152">Group Display Name</span></span>
- <span data-ttu-id="5b751-153">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="5b751-153">Is Deleted</span></span>
- <span data-ttu-id="5b751-154">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="5b751-154">Owner Principal Name</span></span>
- <span data-ttu-id="5b751-155">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="5b751-155">Last Activity Date</span></span>
- <span data-ttu-id="5b751-156">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="5b751-156">Group Type</span></span>
- <span data-ttu-id="5b751-157">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="5b751-157">Member Count</span></span>
- <span data-ttu-id="5b751-158">External Member Count (количество внешних участников)</span><span class="sxs-lookup"><span data-stu-id="5b751-158">External Member Count</span></span>
- <span data-ttu-id="5b751-159">Exchange Received Email Count (количество полученных сообщений Exchange)</span><span class="sxs-lookup"><span data-stu-id="5b751-159">Exchange Received Email Count</span></span>
- <span data-ttu-id="5b751-160">SharePoint Active File Count (количество активных файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="5b751-160">SharePoint Active File Count</span></span>
- <span data-ttu-id="5b751-161">Yammer Posted Message Count (количество опубликованных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="5b751-161">Yammer Posted Message Count</span></span>
- <span data-ttu-id="5b751-162">Yammer Read Message Count (количество прочитанных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="5b751-162">Yammer Read Message Count</span></span>
- <span data-ttu-id="5b751-163">Yammer Liked Message Count (количество понравившихся сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="5b751-163">Yammer Liked Message Count</span></span>
- <span data-ttu-id="5b751-164">Exchange Mailbox Total Item Count (общее количество элементов в почтовых ящиках Exchange)</span><span class="sxs-lookup"><span data-stu-id="5b751-164">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="5b751-165">Exchange Mailbox Storage Used (Byte) [занято почтовыми ящиками Exchange (байт)]</span><span class="sxs-lookup"><span data-stu-id="5b751-165">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="5b751-166">SharePoint Total File Count (общее количество файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="5b751-166">SharePoint Total File Count</span></span>
- <span data-ttu-id="5b751-167">SharePoint Site Storage Used (Byte) [занято сайтами SharePoint (байт)]</span><span class="sxs-lookup"><span data-stu-id="5b751-167">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="5b751-168">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="5b751-168">Group Id</span></span>
- <span data-ttu-id="5b751-169">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="5b751-169">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5b751-170">Пример</span><span class="sxs-lookup"><span data-stu-id="5b751-170">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5b751-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b751-171">Request</span></span>

<span data-ttu-id="5b751-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b751-172">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="5b751-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b751-173">Response</span></span>

<span data-ttu-id="5b751-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b751-174">The following is an example of the response.</span></span>

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

<span data-ttu-id="5b751-175">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="5b751-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

