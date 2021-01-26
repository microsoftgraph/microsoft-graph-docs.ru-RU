---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Получите сведения об использовании OneDrive с разбивкой по учетным записям.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 5ed5a3bb06a80d7af6505e6042e566da2f511dd6
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981223"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="70983-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="70983-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

<span data-ttu-id="70983-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70983-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70983-105">Получите сведения об использовании OneDrive с разбивкой по учетным записям.</span><span class="sxs-lookup"><span data-stu-id="70983-105">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="70983-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 об использовании OneDrive для бизнеса.](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)</span><span class="sxs-lookup"><span data-stu-id="70983-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="70983-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70983-107">Permissions</span></span>

<span data-ttu-id="70983-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70983-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70983-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70983-110">Permission type</span></span>                        | <span data-ttu-id="70983-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70983-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="70983-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70983-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="70983-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="70983-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="70983-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70983-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70983-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70983-115">Not supported.</span></span>                           |
| <span data-ttu-id="70983-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70983-116">Application</span></span>                            | <span data-ttu-id="70983-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="70983-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="70983-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="70983-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="70983-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="70983-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="70983-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70983-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="70983-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="70983-121">Function parameters</span></span>

<span data-ttu-id="70983-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="70983-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="70983-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="70983-123">Parameter</span></span> | <span data-ttu-id="70983-124">Тип</span><span class="sxs-lookup"><span data-stu-id="70983-124">Type</span></span>   | <span data-ttu-id="70983-125">Описание</span><span class="sxs-lookup"><span data-stu-id="70983-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="70983-126">period</span><span class="sxs-lookup"><span data-stu-id="70983-126">period</span></span>    | <span data-ttu-id="70983-127">string</span><span class="sxs-lookup"><span data-stu-id="70983-127">string</span></span> | <span data-ttu-id="70983-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="70983-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="70983-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="70983-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="70983-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="70983-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="70983-131">date</span><span class="sxs-lookup"><span data-stu-id="70983-131">date</span></span>      | <span data-ttu-id="70983-132">Date</span><span class="sxs-lookup"><span data-stu-id="70983-132">Date</span></span>   | <span data-ttu-id="70983-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="70983-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="70983-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="70983-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="70983-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="70983-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="70983-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="70983-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70983-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70983-137">Request headers</span></span>

| <span data-ttu-id="70983-138">Имя</span><span class="sxs-lookup"><span data-stu-id="70983-138">Name</span></span>          | <span data-ttu-id="70983-139">Описание</span><span class="sxs-lookup"><span data-stu-id="70983-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="70983-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70983-140">Authorization</span></span> | <span data-ttu-id="70983-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70983-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="70983-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="70983-143">If-None-Match</span></span> | <span data-ttu-id="70983-144">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="70983-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="70983-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="70983-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="70983-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="70983-146">Response</span></span>

<span data-ttu-id="70983-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="70983-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="70983-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="70983-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="70983-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="70983-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="70983-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="70983-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="70983-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="70983-151">Report Refresh Date</span></span>
- <span data-ttu-id="70983-152">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="70983-152">Site URL</span></span>
- <span data-ttu-id="70983-153">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="70983-153">Owner Display Name</span></span>
- <span data-ttu-id="70983-154">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="70983-154">Is Deleted</span></span>
- <span data-ttu-id="70983-155">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="70983-155">Last Activity Date</span></span>
- <span data-ttu-id="70983-156">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="70983-156">File Count</span></span>
- <span data-ttu-id="70983-157">Active File Count (количество активных файлов)</span><span class="sxs-lookup"><span data-stu-id="70983-157">Active File Count</span></span>
- <span data-ttu-id="70983-158">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="70983-158">Storage Used (Byte)</span></span>
- <span data-ttu-id="70983-159">"Storage Allocated (Byte)" (Объем выделенного хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="70983-159">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="70983-160">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="70983-160">Owner Principal Name</span></span>
- <span data-ttu-id="70983-161">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="70983-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="70983-162">Пример</span><span class="sxs-lookup"><span data-stu-id="70983-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="70983-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="70983-163">Request</span></span>

<span data-ttu-id="70983-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70983-164">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getonedriveusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="70983-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="70983-165">Response</span></span>

<span data-ttu-id="70983-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="70983-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="70983-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="70983-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Owner Principal Name,Report Period
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

