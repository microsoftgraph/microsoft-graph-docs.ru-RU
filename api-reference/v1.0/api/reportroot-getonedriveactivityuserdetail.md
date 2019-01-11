---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Получите сведения о действиях в OneDrive с разбивкой по пользователям.
localization_priority: Normal
ms.openlocfilehash: 279c7f4e417b9314d0ed7b6a5dbcf85454d4f0c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826427"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="4c21e-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="4c21e-103">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="4c21e-104">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="4c21e-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="4c21e-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="4c21e-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c21e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c21e-106">Permissions</span></span>

<span data-ttu-id="4c21e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c21e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c21e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c21e-109">Permission type</span></span>                        | <span data-ttu-id="4c21e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c21e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4c21e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c21e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c21e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c21e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4c21e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c21e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c21e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c21e-114">Not supported.</span></span>                           |
| <span data-ttu-id="4c21e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c21e-115">Application</span></span>                            | <span data-ttu-id="4c21e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c21e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4c21e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c21e-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="4c21e-118">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="4c21e-118">Function parameters</span></span>

<span data-ttu-id="4c21e-119">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4c21e-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="4c21e-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="4c21e-120">Parameter</span></span> | <span data-ttu-id="4c21e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4c21e-121">Type</span></span>   | <span data-ttu-id="4c21e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4c21e-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4c21e-123">period</span><span class="sxs-lookup"><span data-stu-id="4c21e-123">period</span></span>    | <span data-ttu-id="4c21e-124">строка</span><span class="sxs-lookup"><span data-stu-id="4c21e-124">string</span></span> | <span data-ttu-id="4c21e-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4c21e-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4c21e-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4c21e-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4c21e-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4c21e-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="4c21e-128">date</span><span class="sxs-lookup"><span data-stu-id="4c21e-128">date</span></span>      | <span data-ttu-id="4c21e-129">Date</span><span class="sxs-lookup"><span data-stu-id="4c21e-129">Date</span></span>   | <span data-ttu-id="4c21e-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="4c21e-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="4c21e-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="4c21e-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="4c21e-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="4c21e-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="4c21e-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="4c21e-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c21e-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c21e-134">Request headers</span></span>

| <span data-ttu-id="4c21e-135">Имя</span><span class="sxs-lookup"><span data-stu-id="4c21e-135">Name</span></span>          | <span data-ttu-id="4c21e-136">Описание</span><span class="sxs-lookup"><span data-stu-id="4c21e-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4c21e-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c21e-137">Authorization</span></span> | <span data-ttu-id="4c21e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c21e-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4c21e-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4c21e-140">If-None-Match</span></span> | <span data-ttu-id="4c21e-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="4c21e-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4c21e-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4c21e-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4c21e-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c21e-143">Response</span></span>

<span data-ttu-id="4c21e-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4c21e-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4c21e-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4c21e-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4c21e-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4c21e-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4c21e-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4c21e-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4c21e-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4c21e-148">Report Refresh Date</span></span>
- <span data-ttu-id="4c21e-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="4c21e-149">User Principal Name</span></span>
- <span data-ttu-id="4c21e-150">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="4c21e-150">Is Deleted</span></span>
- <span data-ttu-id="4c21e-151">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="4c21e-151">Deleted Date</span></span>
- <span data-ttu-id="4c21e-152">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="4c21e-152">Last Activity Date</span></span>
- <span data-ttu-id="4c21e-153">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="4c21e-153">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="4c21e-154">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="4c21e-154">Synced File Count</span></span>
- <span data-ttu-id="4c21e-155">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="4c21e-155">Shared Internally File Count</span></span>
- <span data-ttu-id="4c21e-156">"Shared Externally File Count" (Количество файлов, к которым предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="4c21e-156">Shared Externally File Count</span></span>
- <span data-ttu-id="4c21e-157">"Assigned Products" (Назначенные продукты);</span><span class="sxs-lookup"><span data-stu-id="4c21e-157">Assigned Products</span></span>
- <span data-ttu-id="4c21e-158">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="4c21e-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4c21e-159">Пример</span><span class="sxs-lookup"><span data-stu-id="4c21e-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4c21e-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c21e-160">Request</span></span>

<span data-ttu-id="4c21e-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c21e-161">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="4c21e-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c21e-162">Response</span></span>

<span data-ttu-id="4c21e-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4c21e-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="4c21e-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4c21e-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```
