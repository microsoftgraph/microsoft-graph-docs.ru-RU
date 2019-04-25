---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityUserCounts'
description: Получение сведений о том, как меняется количество уникальных пользователей и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: af6d72466e58e7b56f3a667ce282d220a638c9f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545820"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="8f6a4-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8f6a4-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f6a4-105">Получение сведений о том, как меняется количество уникальных пользователей и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-105">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="8f6a4-106">Типы сеансов конференц-связи включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба или корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="8f6a4-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="8f6a4-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия организатора конференций в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="8f6a4-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f6a4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f6a4-108">Permissions</span></span>

<span data-ttu-id="8f6a4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f6a4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f6a4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f6a4-111">Permission type</span></span>                        | <span data-ttu-id="8f6a4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f6a4-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8f6a4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f6a4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f6a4-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f6a4-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8f6a4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f6a4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f6a4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-116">Not supported.</span></span>                           |
| <span data-ttu-id="8f6a4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f6a4-117">Application</span></span>                            | <span data-ttu-id="8f6a4-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f6a4-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8f6a4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f6a4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8f6a4-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="8f6a4-120">Function parameters</span></span>

<span data-ttu-id="8f6a4-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8f6a4-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="8f6a4-122">Parameter</span></span> | <span data-ttu-id="8f6a4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8f6a4-123">Type</span></span>   | <span data-ttu-id="8f6a4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8f6a4-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8f6a4-125">period</span><span class="sxs-lookup"><span data-stu-id="8f6a4-125">period</span></span>    | <span data-ttu-id="8f6a4-126">string</span><span class="sxs-lookup"><span data-stu-id="8f6a4-126">string</span></span> | <span data-ttu-id="8f6a4-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8f6a4-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8f6a4-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8f6a4-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-130">Required.</span></span> |

<span data-ttu-id="8f6a4-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8f6a4-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-132">The default output type is text/csv.</span></span> <span data-ttu-id="8f6a4-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f6a4-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f6a4-134">Request headers</span></span>

| <span data-ttu-id="8f6a4-135">Имя</span><span class="sxs-lookup"><span data-stu-id="8f6a4-135">Name</span></span>          | <span data-ttu-id="8f6a4-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8f6a4-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8f6a4-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f6a4-137">Authorization</span></span> | <span data-ttu-id="8f6a4-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8f6a4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f6a4-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8f6a4-141">CSV</span><span class="sxs-lookup"><span data-stu-id="8f6a4-141">CSV</span></span>

<span data-ttu-id="8f6a4-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8f6a4-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8f6a4-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8f6a4-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="8f6a4-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8f6a4-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="8f6a4-146">Report Refresh Date</span></span>
- <span data-ttu-id="8f6a4-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="8f6a4-147">Report Date</span></span>
- <span data-ttu-id="8f6a4-148">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="8f6a4-148">Report Period</span></span>
- <span data-ttu-id="8f6a4-149">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="8f6a4-149">IM</span></span>
- <span data-ttu-id="8f6a4-150">"Audio/Video" (Аудио и видео);</span><span class="sxs-lookup"><span data-stu-id="8f6a4-150">Audio/Video</span></span>
- <span data-ttu-id="8f6a4-151">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="8f6a4-151">App Sharing</span></span>
- <span data-ttu-id="8f6a4-152">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="8f6a4-152">Web</span></span>
- <span data-ttu-id="8f6a4-153">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба);</span><span class="sxs-lookup"><span data-stu-id="8f6a4-153">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="8f6a4-154">"Dial-in/out Microsoft" (Конференции с возможностью присоединения по прямому или обратному звонку, корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="8f6a4-154">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="8f6a4-155">JSON</span><span class="sxs-lookup"><span data-stu-id="8f6a4-155">JSON</span></span>

<span data-ttu-id="8f6a4-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессорганизерактивитюсеркаунтс](../resources/skypeforbusinessorganizeractivityusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f6a4-157">Пример</span><span class="sxs-lookup"><span data-stu-id="8f6a4-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8f6a4-158">CSV</span><span class="sxs-lookup"><span data-stu-id="8f6a4-158">CSV</span></span>

<span data-ttu-id="8f6a4-159">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8f6a4-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f6a4-160">Request</span></span>

<span data-ttu-id="8f6a4-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="8f6a4-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f6a4-162">Response</span></span>

<span data-ttu-id="8f6a4-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8f6a4-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="8f6a4-165">JSON</span><span class="sxs-lookup"><span data-stu-id="8f6a4-165">JSON</span></span>

<span data-ttu-id="8f6a4-166">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8f6a4-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f6a4-167">Request</span></span>

<span data-ttu-id="8f6a4-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="8f6a4-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f6a4-169">Response</span></span>

<span data-ttu-id="8f6a4-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-170">The following is an example of the response.</span></span>

> <span data-ttu-id="8f6a4-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 319

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityUserCounts)", 
  "value": [
    {
      "im": 37, 
      "audioVideo": 42, 
      "appSharing": 35, 
      "web": 3, 
      "dialInOut3rdParty": 0, 
      "dialInOutMicrosoft": 36, 
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
