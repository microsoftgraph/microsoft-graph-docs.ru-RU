---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу конференций, в которых участвовали сотрудники организации (аудио и видео).
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 70a61da1f0402ee8c97337ac42f7f006db5e21aa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525936"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="418dd-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="418dd-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="418dd-105">Отслеживайте динамику использования по продолжительности (в минутах) и типу конференций, в которых участвовали сотрудники организации</span><span class="sxs-lookup"><span data-stu-id="418dd-105">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="418dd-106">(аудио и видео).</span><span class="sxs-lookup"><span data-stu-id="418dd-106">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="418dd-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="418dd-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="418dd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="418dd-108">Permissions</span></span>

<span data-ttu-id="418dd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="418dd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="418dd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="418dd-111">Permission type</span></span>                        | <span data-ttu-id="418dd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="418dd-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="418dd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="418dd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="418dd-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="418dd-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="418dd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="418dd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="418dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="418dd-116">Not supported.</span></span>                           |
| <span data-ttu-id="418dd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="418dd-117">Application</span></span>                            | <span data-ttu-id="418dd-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="418dd-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="418dd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="418dd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="418dd-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="418dd-120">Function parameters</span></span>

<span data-ttu-id="418dd-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="418dd-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="418dd-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="418dd-122">Parameter</span></span> | <span data-ttu-id="418dd-123">Тип</span><span class="sxs-lookup"><span data-stu-id="418dd-123">Type</span></span>   | <span data-ttu-id="418dd-124">Описание</span><span class="sxs-lookup"><span data-stu-id="418dd-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="418dd-125">period</span><span class="sxs-lookup"><span data-stu-id="418dd-125">period</span></span>    | <span data-ttu-id="418dd-126">строка</span><span class="sxs-lookup"><span data-stu-id="418dd-126">string</span></span> | <span data-ttu-id="418dd-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="418dd-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="418dd-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="418dd-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="418dd-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="418dd-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="418dd-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="418dd-130">Required.</span></span> |

<span data-ttu-id="418dd-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="418dd-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="418dd-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="418dd-132">The default output type is text/csv.</span></span> <span data-ttu-id="418dd-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="418dd-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="418dd-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="418dd-134">Request headers</span></span>

| <span data-ttu-id="418dd-135">Имя</span><span class="sxs-lookup"><span data-stu-id="418dd-135">Name</span></span>          | <span data-ttu-id="418dd-136">Описание</span><span class="sxs-lookup"><span data-stu-id="418dd-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="418dd-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="418dd-137">Authorization</span></span> | <span data-ttu-id="418dd-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="418dd-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="418dd-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="418dd-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="418dd-141">CSV</span><span class="sxs-lookup"><span data-stu-id="418dd-141">CSV</span></span>

<span data-ttu-id="418dd-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="418dd-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="418dd-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="418dd-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="418dd-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="418dd-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="418dd-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="418dd-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="418dd-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="418dd-146">Report Refresh Date</span></span>
- <span data-ttu-id="418dd-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="418dd-147">Report Date</span></span>
- <span data-ttu-id="418dd-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="418dd-148">Report Period</span></span>
- <span data-ttu-id="418dd-149">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="418dd-149">Audio/Video</span></span>

### <a name="json"></a><span data-ttu-id="418dd-150">JSON</span><span class="sxs-lookup"><span data-stu-id="418dd-150">JSON</span></span>

<span data-ttu-id="418dd-151">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="418dd-151">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="418dd-152">Пример</span><span class="sxs-lookup"><span data-stu-id="418dd-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="418dd-153">CSV</span><span class="sxs-lookup"><span data-stu-id="418dd-153">CSV</span></span>

<span data-ttu-id="418dd-154">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="418dd-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="418dd-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="418dd-155">Request</span></span>

<span data-ttu-id="418dd-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="418dd-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="418dd-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="418dd-157">Response</span></span>

<span data-ttu-id="418dd-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="418dd-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="418dd-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="418dd-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
```

### <a name="json"></a><span data-ttu-id="418dd-160">JSON</span><span class="sxs-lookup"><span data-stu-id="418dd-160">JSON</span></span>

<span data-ttu-id="418dd-161">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="418dd-161">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="418dd-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="418dd-162">Request</span></span>

<span data-ttu-id="418dd-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="418dd-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="418dd-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="418dd-164">Response</span></span>

<span data-ttu-id="418dd-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="418dd-165">The following is an example of the response.</span></span>

> <span data-ttu-id="418dd-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="418dd-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts)", 
  "value": [
    {
      "audiovideo": 6267, 
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
