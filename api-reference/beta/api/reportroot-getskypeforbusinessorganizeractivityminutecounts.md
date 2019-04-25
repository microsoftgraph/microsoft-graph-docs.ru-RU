---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций (аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7b20fd8dd9636b55bd614ebee8b1a3c19f38d7b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537873"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="e31ff-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="e31ff-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e31ff-105">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций</span><span class="sxs-lookup"><span data-stu-id="e31ff-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="e31ff-106">(аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="e31ff-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="e31ff-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="e31ff-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="e31ff-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e31ff-108">Permissions</span></span>

<span data-ttu-id="e31ff-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e31ff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e31ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e31ff-111">Permission type</span></span>                        | <span data-ttu-id="e31ff-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e31ff-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e31ff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e31ff-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e31ff-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e31ff-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e31ff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e31ff-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e31ff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e31ff-116">Not supported.</span></span>                           |
| <span data-ttu-id="e31ff-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e31ff-117">Application</span></span>                            | <span data-ttu-id="e31ff-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e31ff-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e31ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e31ff-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e31ff-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="e31ff-120">Function parameters</span></span>

<span data-ttu-id="e31ff-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="e31ff-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e31ff-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="e31ff-122">Parameter</span></span> | <span data-ttu-id="e31ff-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e31ff-123">Type</span></span>   | <span data-ttu-id="e31ff-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e31ff-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e31ff-125">period</span><span class="sxs-lookup"><span data-stu-id="e31ff-125">period</span></span>    | <span data-ttu-id="e31ff-126">string</span><span class="sxs-lookup"><span data-stu-id="e31ff-126">string</span></span> | <span data-ttu-id="e31ff-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="e31ff-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e31ff-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="e31ff-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e31ff-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="e31ff-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e31ff-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e31ff-130">Required.</span></span> |

<span data-ttu-id="e31ff-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e31ff-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e31ff-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="e31ff-132">The default output type is text/csv.</span></span> <span data-ttu-id="e31ff-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="e31ff-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e31ff-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e31ff-134">Request headers</span></span>

| <span data-ttu-id="e31ff-135">Имя</span><span class="sxs-lookup"><span data-stu-id="e31ff-135">Name</span></span>          | <span data-ttu-id="e31ff-136">Описание</span><span class="sxs-lookup"><span data-stu-id="e31ff-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e31ff-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e31ff-137">Authorization</span></span> | <span data-ttu-id="e31ff-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e31ff-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e31ff-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e31ff-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e31ff-141">CSV</span><span class="sxs-lookup"><span data-stu-id="e31ff-141">CSV</span></span>

<span data-ttu-id="e31ff-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="e31ff-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e31ff-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="e31ff-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e31ff-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e31ff-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e31ff-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="e31ff-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e31ff-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="e31ff-146">Report Refresh Date</span></span>
- <span data-ttu-id="e31ff-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="e31ff-147">Report Date</span></span>
- <span data-ttu-id="e31ff-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="e31ff-148">Report Period</span></span>
- <span data-ttu-id="e31ff-149">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="e31ff-149">Audio/Video</span></span>
- <span data-ttu-id="e31ff-150">Dial-in Microsoft (с телефонным подключением через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e31ff-150">Dial-in Microsoft</span></span>
- <span data-ttu-id="e31ff-151">Dial-out Microsoft (с присоединением обратным звонком через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e31ff-151">Dial-out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="e31ff-152">JSON</span><span class="sxs-lookup"><span data-stu-id="e31ff-152">JSON</span></span>

<span data-ttu-id="e31ff-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессорганизерактивитиминутекаунтс](../resources/skypeforbusinessorganizeractivityminutecounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e31ff-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e31ff-154">Пример</span><span class="sxs-lookup"><span data-stu-id="e31ff-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e31ff-155">CSV</span><span class="sxs-lookup"><span data-stu-id="e31ff-155">CSV</span></span>

<span data-ttu-id="e31ff-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="e31ff-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e31ff-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="e31ff-157">Request</span></span>

<span data-ttu-id="e31ff-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e31ff-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e31ff-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="e31ff-159">Response</span></span>

<span data-ttu-id="e31ff-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e31ff-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e31ff-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="e31ff-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
```

### <a name="json"></a><span data-ttu-id="e31ff-162">JSON</span><span class="sxs-lookup"><span data-stu-id="e31ff-162">JSON</span></span>

<span data-ttu-id="e31ff-163">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="e31ff-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e31ff-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="e31ff-164">Request</span></span>

<span data-ttu-id="e31ff-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e31ff-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e31ff-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="e31ff-166">Response</span></span>

<span data-ttu-id="e31ff-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e31ff-167">The following is an example of the response.</span></span>

> <span data-ttu-id="e31ff-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e31ff-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts)", 
  "value": [
    {
      "audioVideo": 1912, 
      "dialInMicrosoft": 108, 
      "dialOutMicrosoft": 0, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
