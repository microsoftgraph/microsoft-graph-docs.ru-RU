---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 531ef4002252c7c4a70b67d4326dbd9742b568f9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573013"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="da8b4-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="da8b4-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da8b4-105">Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации</span><span class="sxs-lookup"><span data-stu-id="da8b4-105">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="da8b4-106">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).</span><span class="sxs-lookup"><span data-stu-id="da8b4-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="da8b4-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="da8b4-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="da8b4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da8b4-108">Permissions</span></span>

<span data-ttu-id="da8b4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da8b4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da8b4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da8b4-111">Permission type</span></span>                        | <span data-ttu-id="da8b4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da8b4-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="da8b4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da8b4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="da8b4-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="da8b4-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="da8b4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da8b4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da8b4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da8b4-116">Not supported.</span></span>                           |
| <span data-ttu-id="da8b4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da8b4-117">Application</span></span>                            | <span data-ttu-id="da8b4-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="da8b4-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="da8b4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da8b4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="da8b4-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="da8b4-120">Function parameters</span></span>

<span data-ttu-id="da8b4-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="da8b4-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="da8b4-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="da8b4-122">Parameter</span></span> | <span data-ttu-id="da8b4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="da8b4-123">Type</span></span>   | <span data-ttu-id="da8b4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="da8b4-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="da8b4-125">period</span><span class="sxs-lookup"><span data-stu-id="da8b4-125">period</span></span>    | <span data-ttu-id="da8b4-126">строка</span><span class="sxs-lookup"><span data-stu-id="da8b4-126">string</span></span> | <span data-ttu-id="da8b4-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="da8b4-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="da8b4-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="da8b4-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="da8b4-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="da8b4-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="da8b4-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da8b4-130">Required.</span></span> |

<span data-ttu-id="da8b4-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="da8b4-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="da8b4-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="da8b4-132">The default output type is text/csv.</span></span> <span data-ttu-id="da8b4-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="da8b4-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da8b4-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da8b4-134">Request headers</span></span>

| <span data-ttu-id="da8b4-135">Имя</span><span class="sxs-lookup"><span data-stu-id="da8b4-135">Name</span></span>          | <span data-ttu-id="da8b4-136">Описание</span><span class="sxs-lookup"><span data-stu-id="da8b4-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="da8b4-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da8b4-137">Authorization</span></span> | <span data-ttu-id="da8b4-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da8b4-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="da8b4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="da8b4-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="da8b4-141">CSV</span><span class="sxs-lookup"><span data-stu-id="da8b4-141">CSV</span></span>

<span data-ttu-id="da8b4-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="da8b4-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="da8b4-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="da8b4-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="da8b4-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="da8b4-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="da8b4-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="da8b4-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="da8b4-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="da8b4-146">Report Refresh Date</span></span>
- <span data-ttu-id="da8b4-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="da8b4-147">Report Date</span></span>
- <span data-ttu-id="da8b4-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="da8b4-148">Report Period</span></span>
- <span data-ttu-id="da8b4-149">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="da8b4-149">IM</span></span>
- <span data-ttu-id="da8b4-150">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="da8b4-150">Audio/Video</span></span>
- <span data-ttu-id="da8b4-151">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="da8b4-151">App Sharing</span></span>
- <span data-ttu-id="da8b4-152">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="da8b4-152">Web</span></span>
- <span data-ttu-id="da8b4-153">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба);</span><span class="sxs-lookup"><span data-stu-id="da8b4-153">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="da8b4-154">JSON</span><span class="sxs-lookup"><span data-stu-id="da8b4-154">JSON</span></span>

<span data-ttu-id="da8b4-155">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="da8b4-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da8b4-156">Пример</span><span class="sxs-lookup"><span data-stu-id="da8b4-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="da8b4-157">CSV</span><span class="sxs-lookup"><span data-stu-id="da8b4-157">CSV</span></span>

<span data-ttu-id="da8b4-158">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="da8b4-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="da8b4-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="da8b4-159">Request</span></span>

<span data-ttu-id="da8b4-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da8b4-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="da8b4-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="da8b4-161">Response</span></span>

<span data-ttu-id="da8b4-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da8b4-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="da8b4-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="da8b4-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```

### <a name="json"></a><span data-ttu-id="da8b4-164">JSON</span><span class="sxs-lookup"><span data-stu-id="da8b4-164">JSON</span></span>

<span data-ttu-id="da8b4-165">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="da8b4-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="da8b4-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="da8b4-166">Request</span></span>

<span data-ttu-id="da8b4-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da8b4-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="da8b4-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="da8b4-168">Response</span></span>

<span data-ttu-id="da8b4-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da8b4-169">The following is an example of the response.</span></span>

> <span data-ttu-id="da8b4-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da8b4-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 301

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityUserCounts)", 
  "value": [
    {
      "im": 137, 
      "audioVideo": 196, 
      "appSharing": 214, 
      "web": 30, 
      "dialInOut3rdParty": 2, 
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
