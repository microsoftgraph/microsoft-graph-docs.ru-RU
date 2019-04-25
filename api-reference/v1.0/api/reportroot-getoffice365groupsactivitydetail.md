---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Получите сведения об активности в группах Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5f4eb0428039a9e114d34313e5b7efb32d8e40a5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582236"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="b8904-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="b8904-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="b8904-104">Получите сведения об активности в группах Office 365.</span><span class="sxs-lookup"><span data-stu-id="b8904-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="b8904-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="b8904-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8904-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8904-106">Permissions</span></span>

<span data-ttu-id="b8904-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8904-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8904-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8904-109">Permission type</span></span>                        | <span data-ttu-id="b8904-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8904-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b8904-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8904-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8904-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8904-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b8904-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8904-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8904-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8904-114">Not supported.</span></span>                           |
| <span data-ttu-id="b8904-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8904-115">Application</span></span>                            | <span data-ttu-id="b8904-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8904-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b8904-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8904-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b8904-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b8904-118">Function parameters</span></span>

<span data-ttu-id="b8904-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="b8904-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b8904-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="b8904-120">Parameter</span></span> | <span data-ttu-id="b8904-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b8904-121">Type</span></span>   | <span data-ttu-id="b8904-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b8904-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b8904-123">period</span><span class="sxs-lookup"><span data-stu-id="b8904-123">period</span></span>    | <span data-ttu-id="b8904-124">string</span><span class="sxs-lookup"><span data-stu-id="b8904-124">string</span></span> | <span data-ttu-id="b8904-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="b8904-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b8904-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="b8904-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b8904-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="b8904-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b8904-128">date</span><span class="sxs-lookup"><span data-stu-id="b8904-128">date</span></span>      | <span data-ttu-id="b8904-129">Date</span><span class="sxs-lookup"><span data-stu-id="b8904-129">Date</span></span>   | <span data-ttu-id="b8904-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="b8904-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b8904-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="b8904-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b8904-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="b8904-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b8904-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="b8904-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8904-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8904-134">Request headers</span></span>

| <span data-ttu-id="b8904-135">Имя</span><span class="sxs-lookup"><span data-stu-id="b8904-135">Name</span></span>          | <span data-ttu-id="b8904-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b8904-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b8904-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8904-137">Authorization</span></span> | <span data-ttu-id="b8904-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8904-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b8904-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b8904-140">If-None-Match</span></span> | <span data-ttu-id="b8904-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="b8904-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b8904-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b8904-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b8904-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8904-143">Response</span></span>

<span data-ttu-id="b8904-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b8904-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b8904-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b8904-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b8904-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b8904-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b8904-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="b8904-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b8904-148">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="b8904-148">Report Refresh Date</span></span>
- <span data-ttu-id="b8904-149">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="b8904-149">Group Display Name</span></span>
- <span data-ttu-id="b8904-150">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="b8904-150">Is Deleted</span></span>
- <span data-ttu-id="b8904-151">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="b8904-151">Owner Principal Name</span></span>
- <span data-ttu-id="b8904-152">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="b8904-152">Last Activity Date</span></span>
- <span data-ttu-id="b8904-153">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="b8904-153">Group Type</span></span>
- <span data-ttu-id="b8904-154">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="b8904-154">Member Count</span></span>
- <span data-ttu-id="b8904-155">External Member Count (количество внешних участников)</span><span class="sxs-lookup"><span data-stu-id="b8904-155">External Member Count</span></span>
- <span data-ttu-id="b8904-156">Exchange Received Email Count (количество полученных сообщений Exchange)</span><span class="sxs-lookup"><span data-stu-id="b8904-156">Exchange Received Email Count</span></span>
- <span data-ttu-id="b8904-157">SharePoint Active File Count (количество активных файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="b8904-157">SharePoint Active File Count</span></span>
- <span data-ttu-id="b8904-158">Yammer Posted Message Count (количество опубликованных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="b8904-158">Yammer Posted Message Count</span></span>
- <span data-ttu-id="b8904-159">Yammer Read Message Count (количество прочитанных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="b8904-159">Yammer Read Message Count</span></span>
- <span data-ttu-id="b8904-160">Yammer Liked Message Count (количество понравившихся сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="b8904-160">Yammer Liked Message Count</span></span>
- <span data-ttu-id="b8904-161">Exchange Mailbox Total Item Count (общее количество элементов в почтовых ящиках Exchange)</span><span class="sxs-lookup"><span data-stu-id="b8904-161">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="b8904-162">Exchange Mailbox Storage Used (Byte) [занято почтовыми ящиками Exchange (байт)]</span><span class="sxs-lookup"><span data-stu-id="b8904-162">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="b8904-163">SharePoint Total File Count (общее количество файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="b8904-163">SharePoint Total File Count</span></span>
- <span data-ttu-id="b8904-164">SharePoint Site Storage Used (Byte) [занято сайтами SharePoint (байт)]</span><span class="sxs-lookup"><span data-stu-id="b8904-164">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="b8904-165">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="b8904-165">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b8904-166">Пример</span><span class="sxs-lookup"><span data-stu-id="b8904-166">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b8904-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8904-167">Request</span></span>

<span data-ttu-id="b8904-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8904-168">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b8904-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8904-169">Response</span></span>

<span data-ttu-id="b8904-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b8904-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="b8904-171">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b8904-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
```
