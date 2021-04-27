---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов (аудио и видео).
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: ace9f2bbd8f6afe6b1db67b432f20e98ef7686e0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052763"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="4c55f-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="4c55f-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

<span data-ttu-id="4c55f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c55f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c55f-106">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов</span><span class="sxs-lookup"><span data-stu-id="4c55f-106">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="4c55f-107">(аудио и видео).</span><span class="sxs-lookup"><span data-stu-id="4c55f-107">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="4c55f-108">**Примечание:** Подробные сведения о различных представлениях и именах отчетов см. в Microsoft 365 отчетов — Skype для бизнеса одноранговых [действий.](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)</span><span class="sxs-lookup"><span data-stu-id="4c55f-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c55f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c55f-109">Permissions</span></span>

<span data-ttu-id="4c55f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c55f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c55f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c55f-112">Permission type</span></span>                        | <span data-ttu-id="4c55f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c55f-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4c55f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c55f-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c55f-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c55f-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4c55f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c55f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c55f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c55f-117">Not supported.</span></span>                           |
| <span data-ttu-id="4c55f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c55f-118">Application</span></span>                            | <span data-ttu-id="4c55f-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c55f-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="4c55f-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4c55f-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="4c55f-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="4c55f-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="4c55f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c55f-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4c55f-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4c55f-123">Function parameters</span></span>

<span data-ttu-id="4c55f-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4c55f-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4c55f-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="4c55f-125">Parameter</span></span> | <span data-ttu-id="4c55f-126">Тип</span><span class="sxs-lookup"><span data-stu-id="4c55f-126">Type</span></span>   | <span data-ttu-id="4c55f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4c55f-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4c55f-128">period</span><span class="sxs-lookup"><span data-stu-id="4c55f-128">period</span></span>    | <span data-ttu-id="4c55f-129">string</span><span class="sxs-lookup"><span data-stu-id="4c55f-129">string</span></span> | <span data-ttu-id="4c55f-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4c55f-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4c55f-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4c55f-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4c55f-132">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4c55f-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4c55f-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c55f-133">Required.</span></span> |

<span data-ttu-id="4c55f-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4c55f-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4c55f-135">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="4c55f-135">The default output type is text/csv.</span></span> <span data-ttu-id="4c55f-136">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="4c55f-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c55f-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c55f-137">Request headers</span></span>

| <span data-ttu-id="4c55f-138">Имя</span><span class="sxs-lookup"><span data-stu-id="4c55f-138">Name</span></span>          | <span data-ttu-id="4c55f-139">Описание</span><span class="sxs-lookup"><span data-stu-id="4c55f-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4c55f-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c55f-140">Authorization</span></span> | <span data-ttu-id="4c55f-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c55f-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4c55f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c55f-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4c55f-144">CSV</span><span class="sxs-lookup"><span data-stu-id="4c55f-144">CSV</span></span>

<span data-ttu-id="4c55f-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4c55f-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4c55f-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4c55f-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4c55f-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4c55f-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4c55f-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4c55f-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4c55f-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4c55f-149">Report Refresh Date</span></span>
- <span data-ttu-id="4c55f-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="4c55f-150">Report Date</span></span>
- <span data-ttu-id="4c55f-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="4c55f-151">Report Period</span></span>
- <span data-ttu-id="4c55f-152">Audio (аудио)</span><span class="sxs-lookup"><span data-stu-id="4c55f-152">Audio</span></span>
- <span data-ttu-id="4c55f-153">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="4c55f-153">Video</span></span>

### <a name="json"></a><span data-ttu-id="4c55f-154">JSON</span><span class="sxs-lookup"><span data-stu-id="4c55f-154">JSON</span></span>

<span data-ttu-id="4c55f-155">В случае успеха этот метод возвращает код отклика и `200 OK` **[объект SkypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4c55f-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c55f-156">Пример</span><span class="sxs-lookup"><span data-stu-id="4c55f-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4c55f-157">CSV</span><span class="sxs-lookup"><span data-stu-id="4c55f-157">CSV</span></span>

<span data-ttu-id="4c55f-158">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="4c55f-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4c55f-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c55f-159">Request</span></span>

<span data-ttu-id="4c55f-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c55f-160">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="4c55f-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c55f-161">Response</span></span>

<span data-ttu-id="4c55f-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c55f-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4c55f-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4c55f-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
```

### <a name="json"></a><span data-ttu-id="4c55f-164">JSON</span><span class="sxs-lookup"><span data-stu-id="4c55f-164">JSON</span></span>

<span data-ttu-id="4c55f-165">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="4c55f-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4c55f-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c55f-166">Request</span></span>

<span data-ttu-id="4c55f-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c55f-167">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="4c55f-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c55f-168">Response</span></span>

<span data-ttu-id="4c55f-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4c55f-169">The following is an example of the response.</span></span>

> <span data-ttu-id="4c55f-170">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4c55f-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts)", 
  "value": [
    {
      "audio": 836, 
      "video": 35, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


