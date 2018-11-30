---
title: 'reportRoot: getSkypeForBusinessParticipantActivityCounts'
description: Отследите динамику использования по количеству и типу сеансов конференц-связи, в которых участвовали сотрудники организации. Такие типы включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба).
ms.openlocfilehash: ecb3938330b38492dbee6dd873421c96fbf23d56
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076744"
---
# <a name="reportroot-getskypeforbusinessparticipantactivitycounts"></a><span data-ttu-id="6dbcf-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="6dbcf-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span></span>

> <span data-ttu-id="6dbcf-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6dbcf-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6dbcf-107">Отследите динамику использования по количеству и типу сеансов конференц-связи, в которых участвовали сотрудники организации.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-107">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="6dbcf-108">Такие типы включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба).</span><span class="sxs-lookup"><span data-stu-id="6dbcf-108">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="6dbcf-109">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="6dbcf-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="6dbcf-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6dbcf-110">Permissions</span></span>

<span data-ttu-id="6dbcf-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dbcf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6dbcf-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dbcf-113">Permission type</span></span>                        | <span data-ttu-id="6dbcf-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dbcf-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6dbcf-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dbcf-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="6dbcf-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dbcf-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6dbcf-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dbcf-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dbcf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-118">Not supported.</span></span>                           |
| <span data-ttu-id="6dbcf-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6dbcf-119">Application</span></span>                            | <span data-ttu-id="6dbcf-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dbcf-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6dbcf-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dbcf-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6dbcf-122">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="6dbcf-122">Function parameters</span></span>

<span data-ttu-id="6dbcf-123">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6dbcf-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="6dbcf-124">Parameter</span></span> | <span data-ttu-id="6dbcf-125">Тип</span><span class="sxs-lookup"><span data-stu-id="6dbcf-125">Type</span></span>   | <span data-ttu-id="6dbcf-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6dbcf-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6dbcf-127">period</span><span class="sxs-lookup"><span data-stu-id="6dbcf-127">period</span></span>    | <span data-ttu-id="6dbcf-128">строка</span><span class="sxs-lookup"><span data-stu-id="6dbcf-128">string</span></span> | <span data-ttu-id="6dbcf-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6dbcf-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6dbcf-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6dbcf-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-132">Required.</span></span> |

<span data-ttu-id="6dbcf-133">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6dbcf-134">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-134">The default output type is text/csv.</span></span> <span data-ttu-id="6dbcf-135">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dbcf-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dbcf-136">Request headers</span></span>

| <span data-ttu-id="6dbcf-137">Имя</span><span class="sxs-lookup"><span data-stu-id="6dbcf-137">Name</span></span>          | <span data-ttu-id="6dbcf-138">Описание</span><span class="sxs-lookup"><span data-stu-id="6dbcf-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6dbcf-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6dbcf-139">Authorization</span></span> | <span data-ttu-id="6dbcf-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6dbcf-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="6dbcf-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6dbcf-143">CSV</span><span class="sxs-lookup"><span data-stu-id="6dbcf-143">CSV</span></span>

<span data-ttu-id="6dbcf-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6dbcf-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6dbcf-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6dbcf-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6dbcf-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6dbcf-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="6dbcf-148">Report Refresh Date</span></span>
- <span data-ttu-id="6dbcf-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="6dbcf-149">Report Date</span></span>
- <span data-ttu-id="6dbcf-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="6dbcf-150">Report Period</span></span>
- <span data-ttu-id="6dbcf-151">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="6dbcf-151">IM</span></span>
- <span data-ttu-id="6dbcf-152">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="6dbcf-152">Audio/Video</span></span>
- <span data-ttu-id="6dbcf-153">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="6dbcf-153">App Sharing</span></span>
- <span data-ttu-id="6dbcf-154">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="6dbcf-154">Web</span></span>
- <span data-ttu-id="6dbcf-155">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба);</span><span class="sxs-lookup"><span data-stu-id="6dbcf-155">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="6dbcf-156">JSON</span><span class="sxs-lookup"><span data-stu-id="6dbcf-156">JSON</span></span>

<span data-ttu-id="6dbcf-157">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dbcf-158">Пример</span><span class="sxs-lookup"><span data-stu-id="6dbcf-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6dbcf-159">CSV</span><span class="sxs-lookup"><span data-stu-id="6dbcf-159">CSV</span></span>

<span data-ttu-id="6dbcf-160">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6dbcf-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dbcf-161">Request</span></span>

<span data-ttu-id="6dbcf-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6dbcf-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="6dbcf-163">Response</span></span>

<span data-ttu-id="6dbcf-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6dbcf-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="6dbcf-166">JSON</span><span class="sxs-lookup"><span data-stu-id="6dbcf-166">JSON</span></span>

<span data-ttu-id="6dbcf-167">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6dbcf-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dbcf-168">Request</span></span>

<span data-ttu-id="6dbcf-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6dbcf-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="6dbcf-170">Response</span></span>

<span data-ttu-id="6dbcf-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-171">The following is an example of the response.</span></span>

> <span data-ttu-id="6dbcf-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6dbcf-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 296

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityCounts)", 
  "value": [
    {
      "im": 162, 
      "audioVideo": 156, 
      "appSharing": 45, 
      "web": 12, 
      "dialInOut3rdParty": 2, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
