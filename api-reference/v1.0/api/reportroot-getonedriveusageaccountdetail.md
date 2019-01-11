---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Получите сведения об использовании OneDrive с разбивкой по учетным записям.
localization_priority: Normal
ms.openlocfilehash: 0a2dffabb1f5f4ba551615525b037c39f10d39ab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848316"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="3aee1-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="3aee1-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

<span data-ttu-id="3aee1-104">Получите сведения об использовании OneDrive с разбивкой по учетным записям.</span><span class="sxs-lookup"><span data-stu-id="3aee1-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="3aee1-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="3aee1-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="3aee1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3aee1-106">Permissions</span></span>

<span data-ttu-id="3aee1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aee1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3aee1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3aee1-109">Permission type</span></span>                        | <span data-ttu-id="3aee1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3aee1-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3aee1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3aee1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3aee1-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3aee1-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3aee1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3aee1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aee1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3aee1-114">Not supported.</span></span>                           |
| <span data-ttu-id="3aee1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3aee1-115">Application</span></span>                            | <span data-ttu-id="3aee1-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3aee1-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3aee1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3aee1-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="3aee1-118">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="3aee1-118">Function parameters</span></span>

<span data-ttu-id="3aee1-119">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3aee1-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="3aee1-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="3aee1-120">Parameter</span></span> | <span data-ttu-id="3aee1-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3aee1-121">Type</span></span>   | <span data-ttu-id="3aee1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3aee1-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3aee1-123">period</span><span class="sxs-lookup"><span data-stu-id="3aee1-123">period</span></span>    | <span data-ttu-id="3aee1-124">строка</span><span class="sxs-lookup"><span data-stu-id="3aee1-124">string</span></span> | <span data-ttu-id="3aee1-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3aee1-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3aee1-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3aee1-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3aee1-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3aee1-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="3aee1-128">date</span><span class="sxs-lookup"><span data-stu-id="3aee1-128">date</span></span>      | <span data-ttu-id="3aee1-129">Date</span><span class="sxs-lookup"><span data-stu-id="3aee1-129">Date</span></span>   | <span data-ttu-id="3aee1-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="3aee1-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="3aee1-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="3aee1-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="3aee1-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="3aee1-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="3aee1-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="3aee1-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3aee1-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3aee1-134">Request headers</span></span>

| <span data-ttu-id="3aee1-135">Имя</span><span class="sxs-lookup"><span data-stu-id="3aee1-135">Name</span></span>          | <span data-ttu-id="3aee1-136">Описание</span><span class="sxs-lookup"><span data-stu-id="3aee1-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3aee1-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3aee1-137">Authorization</span></span> | <span data-ttu-id="3aee1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3aee1-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3aee1-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3aee1-140">If-None-Match</span></span> | <span data-ttu-id="3aee1-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="3aee1-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3aee1-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3aee1-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3aee1-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="3aee1-143">Response</span></span>

<span data-ttu-id="3aee1-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3aee1-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3aee1-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3aee1-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3aee1-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3aee1-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3aee1-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3aee1-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3aee1-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3aee1-148">Report Refresh Date</span></span>
- <span data-ttu-id="3aee1-149">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="3aee1-149">Site URL</span></span>
- <span data-ttu-id="3aee1-150">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="3aee1-150">Owner Display Name</span></span>
- <span data-ttu-id="3aee1-151">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="3aee1-151">Is Deleted</span></span>
- <span data-ttu-id="3aee1-152">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="3aee1-152">Last Activity Date</span></span>
- <span data-ttu-id="3aee1-153">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="3aee1-153">File Count</span></span>
- <span data-ttu-id="3aee1-154">Active File Count (количество активных файлов)</span><span class="sxs-lookup"><span data-stu-id="3aee1-154">Active File Count</span></span>
- <span data-ttu-id="3aee1-155">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="3aee1-155">Storage Used (Byte)</span></span>
- <span data-ttu-id="3aee1-156">Storage Allocated (Byte) [выделено (байт)]</span><span class="sxs-lookup"><span data-stu-id="3aee1-156">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="3aee1-157">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="3aee1-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3aee1-158">Пример</span><span class="sxs-lookup"><span data-stu-id="3aee1-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3aee1-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="3aee1-159">Request</span></span>

<span data-ttu-id="3aee1-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3aee1-160">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="3aee1-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="3aee1-161">Response</span></span>

<span data-ttu-id="3aee1-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3aee1-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="3aee1-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3aee1-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Report Period
```
