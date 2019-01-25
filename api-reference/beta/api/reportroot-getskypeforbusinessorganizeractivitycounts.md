---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: Получение сведений о том, как меняется количество и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации. Такие типы включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба или корпорация Майкрософт).
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3f8f8b84fbf1fd159c688511ef49ae4c1132a849
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525446"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="c5007-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="c5007-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5007-105">Получение сведений о том, как меняется количество и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации.</span><span class="sxs-lookup"><span data-stu-id="c5007-105">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="c5007-106">Такие типы включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба или корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="c5007-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="c5007-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия организатора конференций в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="c5007-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5007-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5007-108">Permissions</span></span>

<span data-ttu-id="c5007-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5007-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5007-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5007-111">Permission type</span></span>                        | <span data-ttu-id="c5007-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5007-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c5007-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5007-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5007-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5007-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c5007-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5007-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5007-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5007-116">Not supported.</span></span>                           |
| <span data-ttu-id="c5007-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5007-117">Application</span></span>                            | <span data-ttu-id="c5007-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5007-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c5007-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5007-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c5007-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c5007-120">Function parameters</span></span>

<span data-ttu-id="c5007-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c5007-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c5007-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="c5007-122">Parameter</span></span> | <span data-ttu-id="c5007-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c5007-123">Type</span></span>   | <span data-ttu-id="c5007-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c5007-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c5007-125">period</span><span class="sxs-lookup"><span data-stu-id="c5007-125">period</span></span>    | <span data-ttu-id="c5007-126">строка</span><span class="sxs-lookup"><span data-stu-id="c5007-126">string</span></span> | <span data-ttu-id="c5007-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c5007-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c5007-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c5007-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c5007-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c5007-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c5007-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5007-130">Required.</span></span> |

<span data-ttu-id="c5007-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c5007-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c5007-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="c5007-132">The default output type is text/csv.</span></span> <span data-ttu-id="c5007-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="c5007-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5007-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5007-134">Request headers</span></span>

| <span data-ttu-id="c5007-135">Имя</span><span class="sxs-lookup"><span data-stu-id="c5007-135">Name</span></span>          | <span data-ttu-id="c5007-136">Описание</span><span class="sxs-lookup"><span data-stu-id="c5007-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c5007-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5007-137">Authorization</span></span> | <span data-ttu-id="c5007-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5007-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c5007-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5007-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c5007-141">CSV</span><span class="sxs-lookup"><span data-stu-id="c5007-141">CSV</span></span>

<span data-ttu-id="c5007-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c5007-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c5007-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c5007-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c5007-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c5007-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c5007-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c5007-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c5007-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c5007-146">Report Refresh Date</span></span>
- <span data-ttu-id="c5007-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="c5007-147">Report Date</span></span>
- <span data-ttu-id="c5007-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="c5007-148">Report Period</span></span>
- <span data-ttu-id="c5007-149">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="c5007-149">IM</span></span>
- <span data-ttu-id="c5007-150">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="c5007-150">Audio/Video</span></span>
- <span data-ttu-id="c5007-151">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="c5007-151">App Sharing</span></span>
- <span data-ttu-id="c5007-152">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="c5007-152">Web</span></span>
- <span data-ttu-id="c5007-153">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба);</span><span class="sxs-lookup"><span data-stu-id="c5007-153">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="c5007-154">"Dial-in/out Microsoft" (Конференции с возможностью присоединения по прямому или обратному звонку, корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="c5007-154">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="c5007-155">JSON</span><span class="sxs-lookup"><span data-stu-id="c5007-155">JSON</span></span>

<span data-ttu-id="c5007-156">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c5007-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5007-157">Пример</span><span class="sxs-lookup"><span data-stu-id="c5007-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c5007-158">CSV</span><span class="sxs-lookup"><span data-stu-id="c5007-158">CSV</span></span>

<span data-ttu-id="c5007-159">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="c5007-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c5007-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5007-160">Request</span></span>

<span data-ttu-id="c5007-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5007-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="c5007-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5007-162">Response</span></span>

<span data-ttu-id="c5007-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c5007-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c5007-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c5007-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```

### <a name="json"></a><span data-ttu-id="c5007-165">JSON</span><span class="sxs-lookup"><span data-stu-id="c5007-165">JSON</span></span>

<span data-ttu-id="c5007-166">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="c5007-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c5007-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5007-167">Request</span></span>

<span data-ttu-id="c5007-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5007-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="c5007-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5007-169">Response</span></span>

<span data-ttu-id="c5007-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c5007-170">The following is an example of the response.</span></span>

> <span data-ttu-id="c5007-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5007-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityCounts)", 
  "value": [
    {
      "im": 20, 
      "audioVideo": 43, 
      "appSharing": 20, 
      "web": 6, 
      "dialInOut3rdParty": 0, 
      "dialInOutMicrosoft": 48, 
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
