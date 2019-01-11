---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Получите сведения об активности в группах Yammer.
localization_priority: Normal
ms.openlocfilehash: 58410ef714f09dd3bb47c0eb5cb1e076c510875b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867867"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="54d98-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="54d98-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="54d98-104">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="54d98-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="54d98-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="54d98-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="54d98-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54d98-106">Permissions</span></span>

<span data-ttu-id="54d98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54d98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54d98-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54d98-109">Permission type</span></span>                        | <span data-ttu-id="54d98-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54d98-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="54d98-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54d98-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="54d98-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="54d98-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="54d98-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54d98-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54d98-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54d98-114">Not supported.</span></span>                           |
| <span data-ttu-id="54d98-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54d98-115">Application</span></span>                            | <span data-ttu-id="54d98-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="54d98-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="54d98-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54d98-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="54d98-118">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="54d98-118">Function parameters</span></span>

<span data-ttu-id="54d98-119">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="54d98-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="54d98-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="54d98-120">Parameter</span></span> | <span data-ttu-id="54d98-121">Тип</span><span class="sxs-lookup"><span data-stu-id="54d98-121">Type</span></span>   | <span data-ttu-id="54d98-122">Описание</span><span class="sxs-lookup"><span data-stu-id="54d98-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="54d98-123">period</span><span class="sxs-lookup"><span data-stu-id="54d98-123">period</span></span>    | <span data-ttu-id="54d98-124">строка</span><span class="sxs-lookup"><span data-stu-id="54d98-124">string</span></span> | <span data-ttu-id="54d98-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="54d98-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="54d98-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="54d98-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="54d98-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="54d98-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="54d98-128">date</span><span class="sxs-lookup"><span data-stu-id="54d98-128">date</span></span>      | <span data-ttu-id="54d98-129">Date</span><span class="sxs-lookup"><span data-stu-id="54d98-129">Date</span></span>   | <span data-ttu-id="54d98-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="54d98-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="54d98-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="54d98-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="54d98-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="54d98-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="54d98-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="54d98-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54d98-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54d98-134">Request headers</span></span>

| <span data-ttu-id="54d98-135">Имя</span><span class="sxs-lookup"><span data-stu-id="54d98-135">Name</span></span>          | <span data-ttu-id="54d98-136">Описание</span><span class="sxs-lookup"><span data-stu-id="54d98-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="54d98-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54d98-137">Authorization</span></span> | <span data-ttu-id="54d98-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54d98-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="54d98-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="54d98-140">If-None-Match</span></span> | <span data-ttu-id="54d98-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="54d98-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="54d98-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="54d98-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="54d98-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="54d98-143">Response</span></span>

<span data-ttu-id="54d98-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="54d98-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="54d98-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="54d98-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="54d98-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="54d98-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="54d98-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="54d98-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="54d98-148">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="54d98-148">Report Refresh Date</span></span>
- <span data-ttu-id="54d98-149">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="54d98-149">Group Display Name</span></span>
- <span data-ttu-id="54d98-150">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="54d98-150">Is Deleted</span></span>
- <span data-ttu-id="54d98-151">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="54d98-151">Owner Principal Name</span></span>
- <span data-ttu-id="54d98-152">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="54d98-152">Last Activity Date</span></span>
- <span data-ttu-id="54d98-153">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="54d98-153">Group Type</span></span>
- <span data-ttu-id="54d98-154">Office 365 Connected (подключены к Office 365)</span><span class="sxs-lookup"><span data-stu-id="54d98-154">Office 365 Connected</span></span>
- <span data-ttu-id="54d98-155">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="54d98-155">Member Count</span></span>
- <span data-ttu-id="54d98-156">Posted Count (количество опубликованных сообщений)</span><span class="sxs-lookup"><span data-stu-id="54d98-156">Posted Count</span></span>
- <span data-ttu-id="54d98-157">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="54d98-157">Read Count</span></span>
- <span data-ttu-id="54d98-158">Liked Count (количество понравившихся сообщений)</span><span class="sxs-lookup"><span data-stu-id="54d98-158">Liked Count</span></span>
- <span data-ttu-id="54d98-159">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="54d98-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="54d98-160">Пример</span><span class="sxs-lookup"><span data-stu-id="54d98-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="54d98-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="54d98-161">Request</span></span>

<span data-ttu-id="54d98-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54d98-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="54d98-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="54d98-163">Response</span></span>

<span data-ttu-id="54d98-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="54d98-164">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="54d98-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="54d98-165">Request</span></span>
<span data-ttu-id="54d98-166">При вызове с `date`, пределах отчета активности на данной даты.</span><span class="sxs-lookup"><span data-stu-id="54d98-166">If called with a `date`, the report is scoped to activity on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="54d98-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="54d98-167">Response</span></span>

<span data-ttu-id="54d98-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="54d98-168">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="54d98-169">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="54d98-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```
