---
title: 'reportRoot: getSkypeForBusinessActivityUserCounts'
description: Отследите, как меняется количество уникальных организаторов и участников сеансов конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов.
localization_priority: Normal
ms.openlocfilehash: a012045c58acea9539a9ab92aee55e5d8bb106d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806386"
---
# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="cd4ff-104">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="cd4ff-104">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

> <span data-ttu-id="cd4ff-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd4ff-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd4ff-107">Отследите, как меняется количество уникальных организаторов и участников сеансов конференций, проводимых в вашей организации через Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-107">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="cd4ff-108">Отчет также включает количество одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-108">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="cd4ff-109">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="cd4ff-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd4ff-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd4ff-110">Permissions</span></span>

<span data-ttu-id="cd4ff-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd4ff-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cd4ff-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd4ff-113">Permission type</span></span>                        | <span data-ttu-id="cd4ff-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd4ff-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cd4ff-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd4ff-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd4ff-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd4ff-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cd4ff-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd4ff-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd4ff-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-118">Not supported.</span></span>                           |
| <span data-ttu-id="cd4ff-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd4ff-119">Application</span></span>                            | <span data-ttu-id="cd4ff-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd4ff-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cd4ff-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd4ff-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cd4ff-122">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="cd4ff-122">Function parameters</span></span>

<span data-ttu-id="cd4ff-123">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cd4ff-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="cd4ff-124">Parameter</span></span> | <span data-ttu-id="cd4ff-125">Тип</span><span class="sxs-lookup"><span data-stu-id="cd4ff-125">Type</span></span>   | <span data-ttu-id="cd4ff-126">Описание</span><span class="sxs-lookup"><span data-stu-id="cd4ff-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cd4ff-127">period</span><span class="sxs-lookup"><span data-stu-id="cd4ff-127">period</span></span>    | <span data-ttu-id="cd4ff-128">строка</span><span class="sxs-lookup"><span data-stu-id="cd4ff-128">string</span></span> | <span data-ttu-id="cd4ff-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cd4ff-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cd4ff-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cd4ff-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-132">Required.</span></span> |

<span data-ttu-id="cd4ff-133">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cd4ff-134">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-134">The default output type is text/csv.</span></span> <span data-ttu-id="cd4ff-135">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd4ff-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd4ff-136">Request headers</span></span>

| <span data-ttu-id="cd4ff-137">Имя</span><span class="sxs-lookup"><span data-stu-id="cd4ff-137">Name</span></span>          | <span data-ttu-id="cd4ff-138">Описание</span><span class="sxs-lookup"><span data-stu-id="cd4ff-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cd4ff-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd4ff-139">Authorization</span></span> | <span data-ttu-id="cd4ff-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cd4ff-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd4ff-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="cd4ff-143">CSV</span><span class="sxs-lookup"><span data-stu-id="cd4ff-143">CSV</span></span>

<span data-ttu-id="cd4ff-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cd4ff-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cd4ff-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cd4ff-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="cd4ff-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cd4ff-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="cd4ff-148">Report Refresh Date</span></span>
- <span data-ttu-id="cd4ff-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="cd4ff-149">Report Date</span></span>
- <span data-ttu-id="cd4ff-150">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="cd4ff-150">Report Period</span></span>
- <span data-ttu-id="cd4ff-151">"Peer-to-peer" (Одноранговый сеанс);</span><span class="sxs-lookup"><span data-stu-id="cd4ff-151">Peer-to-peer</span></span>
- <span data-ttu-id="cd4ff-152">"Organized" (Организаторы);</span><span class="sxs-lookup"><span data-stu-id="cd4ff-152">Organized</span></span>
- <span data-ttu-id="cd4ff-153">"Participated" (Участники).</span><span class="sxs-lookup"><span data-stu-id="cd4ff-153">Participated</span></span>

### <a name="json"></a><span data-ttu-id="cd4ff-154">JSON</span><span class="sxs-lookup"><span data-stu-id="cd4ff-154">JSON</span></span>

<span data-ttu-id="cd4ff-155">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd4ff-156">Пример</span><span class="sxs-lookup"><span data-stu-id="cd4ff-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="cd4ff-157">CSV</span><span class="sxs-lookup"><span data-stu-id="cd4ff-157">CSV</span></span>

<span data-ttu-id="cd4ff-158">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cd4ff-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd4ff-159">Request</span></span>

<span data-ttu-id="cd4ff-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="cd4ff-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd4ff-161">Response</span></span>

<span data-ttu-id="cd4ff-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cd4ff-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```

### <a name="json"></a><span data-ttu-id="cd4ff-164">JSON</span><span class="sxs-lookup"><span data-stu-id="cd4ff-164">JSON</span></span>

<span data-ttu-id="cd4ff-165">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cd4ff-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd4ff-166">Request</span></span>

<span data-ttu-id="cd4ff-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="cd4ff-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd4ff-168">Response</span></span>

<span data-ttu-id="cd4ff-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-169">The following is an example of the response.</span></span>

> <span data-ttu-id="cd4ff-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd4ff-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 266

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityUserCounts)", 
  "value": [
    {
      "peerToPeer": 413, 
      "organized": 30, 
      "participated": 91, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
