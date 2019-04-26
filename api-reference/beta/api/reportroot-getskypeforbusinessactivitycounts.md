---
title: 'reportRoot: getSkypeForBusinessActivityCounts'
description: Отслеживайте, как меняется количество организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bcacb385f90afd39f0fb1f8caa8bbfbf79c8b79d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336521"
---
# <a name="reportroot-getskypeforbusinessactivitycounts"></a><span data-ttu-id="eb748-104">reportRoot: getSkypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="eb748-104">reportRoot: getSkypeForBusinessActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb748-105">Отслеживайте, как меняется количество организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="eb748-105">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="eb748-106">Отчет также включает количество одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="eb748-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="eb748-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="eb748-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb748-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb748-108">Permissions</span></span>

<span data-ttu-id="eb748-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb748-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb748-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb748-111">Permission type</span></span>                        | <span data-ttu-id="eb748-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb748-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="eb748-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb748-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb748-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb748-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="eb748-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb748-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb748-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb748-116">Not supported.</span></span>                           |
| <span data-ttu-id="eb748-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb748-117">Application</span></span>                            | <span data-ttu-id="eb748-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb748-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="eb748-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb748-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="eb748-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="eb748-120">Function parameters</span></span>

<span data-ttu-id="eb748-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="eb748-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="eb748-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="eb748-122">Parameter</span></span> | <span data-ttu-id="eb748-123">Тип</span><span class="sxs-lookup"><span data-stu-id="eb748-123">Type</span></span>   | <span data-ttu-id="eb748-124">Описание</span><span class="sxs-lookup"><span data-stu-id="eb748-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="eb748-125">period</span><span class="sxs-lookup"><span data-stu-id="eb748-125">period</span></span>    | <span data-ttu-id="eb748-126">string</span><span class="sxs-lookup"><span data-stu-id="eb748-126">string</span></span> | <span data-ttu-id="eb748-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="eb748-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="eb748-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="eb748-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="eb748-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="eb748-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="eb748-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb748-130">Required.</span></span> |

<span data-ttu-id="eb748-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="eb748-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="eb748-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="eb748-132">The default output type is text/csv.</span></span> <span data-ttu-id="eb748-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="eb748-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb748-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb748-134">Request headers</span></span>

| <span data-ttu-id="eb748-135">Имя</span><span class="sxs-lookup"><span data-stu-id="eb748-135">Name</span></span>          | <span data-ttu-id="eb748-136">Описание</span><span class="sxs-lookup"><span data-stu-id="eb748-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="eb748-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb748-137">Authorization</span></span> | <span data-ttu-id="eb748-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb748-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="eb748-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb748-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="eb748-141">CSV</span><span class="sxs-lookup"><span data-stu-id="eb748-141">CSV</span></span>

<span data-ttu-id="eb748-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="eb748-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="eb748-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="eb748-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="eb748-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="eb748-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="eb748-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="eb748-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="eb748-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="eb748-146">Report Refresh Date</span></span>
- <span data-ttu-id="eb748-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="eb748-147">Report Date</span></span>
- <span data-ttu-id="eb748-148">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="eb748-148">Report Period</span></span>
- <span data-ttu-id="eb748-149">"Peer-to-peer" (Одноранговый сеанс);</span><span class="sxs-lookup"><span data-stu-id="eb748-149">Peer-to-peer</span></span>
- <span data-ttu-id="eb748-150">"Organized" (Организаторы);</span><span class="sxs-lookup"><span data-stu-id="eb748-150">Organized</span></span>
- <span data-ttu-id="eb748-151">"Participated" (Участники).</span><span class="sxs-lookup"><span data-stu-id="eb748-151">Participated</span></span>

### <a name="json"></a><span data-ttu-id="eb748-152">JSON</span><span class="sxs-lookup"><span data-stu-id="eb748-152">JSON</span></span>

<span data-ttu-id="eb748-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессактивитикаунтс](../resources/skypeforbusinessactivitycounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb748-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb748-154">Пример</span><span class="sxs-lookup"><span data-stu-id="eb748-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="eb748-155">CSV</span><span class="sxs-lookup"><span data-stu-id="eb748-155">CSV</span></span>

<span data-ttu-id="eb748-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="eb748-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="eb748-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb748-157">Request</span></span>

<span data-ttu-id="eb748-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb748-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="eb748-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb748-159">Response</span></span>

<span data-ttu-id="eb748-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eb748-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="eb748-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="eb748-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="eb748-162">JSON</span><span class="sxs-lookup"><span data-stu-id="eb748-162">JSON</span></span>

<span data-ttu-id="eb748-163">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="eb748-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="eb748-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb748-164">Request</span></span>

<span data-ttu-id="eb748-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb748-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="eb748-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb748-166">Response</span></span>

<span data-ttu-id="eb748-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eb748-167">The following is an example of the response.</span></span>

> <span data-ttu-id="eb748-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb748-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityCounts)", 
  "value": [
    {
      "peerToPeer": 3436, 
      "organized": 58, 
      "participated": 209, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
