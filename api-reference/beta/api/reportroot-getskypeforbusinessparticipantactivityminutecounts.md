---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу конференций, в которых участвовали сотрудники организации (аудио и видео).
ms.openlocfilehash: 5d6b43d9fb989a57c206f95b9c4ee28dda439503
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076743"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="86774-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="86774-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

> <span data-ttu-id="86774-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="86774-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86774-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86774-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="86774-107">Отслеживайте динамику использования по продолжительности (в минутах) и типу конференций, в которых участвовали сотрудники организации</span><span class="sxs-lookup"><span data-stu-id="86774-107">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="86774-108">(аудио и видео).</span><span class="sxs-lookup"><span data-stu-id="86774-108">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="86774-109">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="86774-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="86774-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86774-110">Permissions</span></span>

<span data-ttu-id="86774-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86774-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86774-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86774-113">Permission type</span></span>                        | <span data-ttu-id="86774-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86774-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="86774-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86774-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="86774-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="86774-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="86774-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86774-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86774-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86774-118">Not supported.</span></span>                           |
| <span data-ttu-id="86774-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86774-119">Application</span></span>                            | <span data-ttu-id="86774-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="86774-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="86774-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86774-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="86774-122">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="86774-122">Function parameters</span></span>

<span data-ttu-id="86774-123">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="86774-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="86774-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="86774-124">Parameter</span></span> | <span data-ttu-id="86774-125">Тип</span><span class="sxs-lookup"><span data-stu-id="86774-125">Type</span></span>   | <span data-ttu-id="86774-126">Описание</span><span class="sxs-lookup"><span data-stu-id="86774-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="86774-127">period</span><span class="sxs-lookup"><span data-stu-id="86774-127">period</span></span>    | <span data-ttu-id="86774-128">строка</span><span class="sxs-lookup"><span data-stu-id="86774-128">string</span></span> | <span data-ttu-id="86774-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="86774-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="86774-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="86774-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="86774-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="86774-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="86774-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86774-132">Required.</span></span> |

<span data-ttu-id="86774-133">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="86774-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="86774-134">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="86774-134">The default output type is text/csv.</span></span> <span data-ttu-id="86774-135">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="86774-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86774-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86774-136">Request headers</span></span>

| <span data-ttu-id="86774-137">Имя</span><span class="sxs-lookup"><span data-stu-id="86774-137">Name</span></span>          | <span data-ttu-id="86774-138">Описание</span><span class="sxs-lookup"><span data-stu-id="86774-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="86774-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86774-139">Authorization</span></span> | <span data-ttu-id="86774-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86774-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="86774-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="86774-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="86774-143">CSV</span><span class="sxs-lookup"><span data-stu-id="86774-143">CSV</span></span>

<span data-ttu-id="86774-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="86774-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="86774-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="86774-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="86774-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="86774-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="86774-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="86774-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="86774-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="86774-148">Report Refresh Date</span></span>
- <span data-ttu-id="86774-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="86774-149">Report Date</span></span>
- <span data-ttu-id="86774-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="86774-150">Report Period</span></span>
- <span data-ttu-id="86774-151">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="86774-151">Audio/Video</span></span>

### <a name="json"></a><span data-ttu-id="86774-152">JSON</span><span class="sxs-lookup"><span data-stu-id="86774-152">JSON</span></span>

<span data-ttu-id="86774-153">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="86774-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86774-154">Пример</span><span class="sxs-lookup"><span data-stu-id="86774-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="86774-155">CSV</span><span class="sxs-lookup"><span data-stu-id="86774-155">CSV</span></span>

<span data-ttu-id="86774-156">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="86774-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="86774-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="86774-157">Request</span></span>

<span data-ttu-id="86774-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86774-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="86774-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="86774-159">Response</span></span>

<span data-ttu-id="86774-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="86774-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="86774-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="86774-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="86774-162">JSON</span><span class="sxs-lookup"><span data-stu-id="86774-162">JSON</span></span>

<span data-ttu-id="86774-163">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="86774-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="86774-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="86774-164">Request</span></span>

<span data-ttu-id="86774-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86774-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="86774-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="86774-166">Response</span></span>

<span data-ttu-id="86774-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="86774-167">The following is an example of the response.</span></span>

> <span data-ttu-id="86774-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86774-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
