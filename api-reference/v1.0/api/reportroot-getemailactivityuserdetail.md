---
title: 'reportRoot: getEmailActivityUserDetail'
description: Узнайте, какие действия пользователи выполняли с электронной почтой.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c2c0626fe53795dc2496a45d706bd934603cf18d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575085"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="83c4b-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="83c4b-103">reportRoot: getEmailActivityUserDetail</span></span>

<span data-ttu-id="83c4b-104">Узнайте, какие действия пользователи выполняли с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="83c4b-104">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="83c4b-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="83c4b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="83c4b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83c4b-106">Permissions</span></span>

<span data-ttu-id="83c4b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83c4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83c4b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83c4b-109">Permission type</span></span>                        | <span data-ttu-id="83c4b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83c4b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="83c4b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83c4b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="83c4b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="83c4b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="83c4b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83c4b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83c4b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83c4b-114">Not supported.</span></span>                           |
| <span data-ttu-id="83c4b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83c4b-115">Application</span></span>                            | <span data-ttu-id="83c4b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="83c4b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="83c4b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83c4b-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="83c4b-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="83c4b-118">Function parameters</span></span>

<span data-ttu-id="83c4b-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="83c4b-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="83c4b-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="83c4b-120">Parameter</span></span> | <span data-ttu-id="83c4b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="83c4b-121">Type</span></span>   | <span data-ttu-id="83c4b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="83c4b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="83c4b-123">period</span><span class="sxs-lookup"><span data-stu-id="83c4b-123">period</span></span>    | <span data-ttu-id="83c4b-124">string</span><span class="sxs-lookup"><span data-stu-id="83c4b-124">string</span></span> | <span data-ttu-id="83c4b-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="83c4b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="83c4b-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="83c4b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="83c4b-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="83c4b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="83c4b-128">date</span><span class="sxs-lookup"><span data-stu-id="83c4b-128">date</span></span>      | <span data-ttu-id="83c4b-129">Date</span><span class="sxs-lookup"><span data-stu-id="83c4b-129">Date</span></span>   | <span data-ttu-id="83c4b-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="83c4b-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="83c4b-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="83c4b-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="83c4b-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="83c4b-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="83c4b-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="83c4b-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83c4b-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83c4b-134">Request headers</span></span>

| <span data-ttu-id="83c4b-135">Имя</span><span class="sxs-lookup"><span data-stu-id="83c4b-135">Name</span></span>          | <span data-ttu-id="83c4b-136">Описание</span><span class="sxs-lookup"><span data-stu-id="83c4b-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="83c4b-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83c4b-137">Authorization</span></span> | <span data-ttu-id="83c4b-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83c4b-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="83c4b-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="83c4b-140">If-None-Match</span></span> | <span data-ttu-id="83c4b-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="83c4b-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="83c4b-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="83c4b-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="83c4b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="83c4b-143">Response</span></span>

<span data-ttu-id="83c4b-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="83c4b-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="83c4b-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="83c4b-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="83c4b-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="83c4b-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="83c4b-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="83c4b-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="83c4b-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="83c4b-148">Report Refresh Date</span></span>
- <span data-ttu-id="83c4b-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="83c4b-149">User Principal Name</span></span>
- <span data-ttu-id="83c4b-150">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="83c4b-150">Display Name</span></span>
- <span data-ttu-id="83c4b-151">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="83c4b-151">Is Deleted</span></span>
- <span data-ttu-id="83c4b-152">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="83c4b-152">Deleted Date</span></span>
- <span data-ttu-id="83c4b-153">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="83c4b-153">Last Activity Date</span></span>
- <span data-ttu-id="83c4b-154">Send Count (количество отправленных писем)</span><span class="sxs-lookup"><span data-stu-id="83c4b-154">Send Count</span></span>
- <span data-ttu-id="83c4b-155">Receive Count (количество полученных писем)</span><span class="sxs-lookup"><span data-stu-id="83c4b-155">Receive Count</span></span>
- <span data-ttu-id="83c4b-156">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="83c4b-156">Read Count</span></span>
- <span data-ttu-id="83c4b-157">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="83c4b-157">Assigned Products</span></span>
- <span data-ttu-id="83c4b-158">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="83c4b-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="83c4b-159">Пример</span><span class="sxs-lookup"><span data-stu-id="83c4b-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="83c4b-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="83c4b-160">Request</span></span>

<span data-ttu-id="83c4b-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83c4b-161">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="83c4b-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="83c4b-162">Response</span></span>

<span data-ttu-id="83c4b-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="83c4b-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="83c4b-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="83c4b-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
```
