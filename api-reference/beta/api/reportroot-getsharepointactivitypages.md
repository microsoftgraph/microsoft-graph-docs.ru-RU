---
title: 'reportRoot: getSharePointActivityPages'
description: Узнайте, сколько уникальных страниц посетили пользователи.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3152512ae1fc0ab24c783e90120e4f799747b3bc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331800"
---
# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="1bc77-103">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="1bc77-103">reportRoot: getSharePointActivityPages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bc77-104">Узнайте, сколько уникальных страниц посетили пользователи.</span><span class="sxs-lookup"><span data-stu-id="1bc77-104">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="1bc77-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="1bc77-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="1bc77-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bc77-106">Permissions</span></span>

<span data-ttu-id="1bc77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bc77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1bc77-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bc77-109">Permission type</span></span>                        | <span data-ttu-id="1bc77-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bc77-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1bc77-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bc77-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1bc77-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bc77-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1bc77-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bc77-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bc77-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bc77-114">Not supported.</span></span>                           |
| <span data-ttu-id="1bc77-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bc77-115">Application</span></span>                            | <span data-ttu-id="1bc77-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bc77-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1bc77-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bc77-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1bc77-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="1bc77-118">Function parameters</span></span>

<span data-ttu-id="1bc77-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="1bc77-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1bc77-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="1bc77-120">Parameter</span></span> | <span data-ttu-id="1bc77-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1bc77-121">Type</span></span>   | <span data-ttu-id="1bc77-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1bc77-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1bc77-123">period</span><span class="sxs-lookup"><span data-stu-id="1bc77-123">period</span></span>    | <span data-ttu-id="1bc77-124">string</span><span class="sxs-lookup"><span data-stu-id="1bc77-124">string</span></span> | <span data-ttu-id="1bc77-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="1bc77-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1bc77-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="1bc77-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1bc77-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="1bc77-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1bc77-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bc77-128">Required.</span></span> |

<span data-ttu-id="1bc77-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1bc77-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1bc77-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="1bc77-130">The default output type is text/csv.</span></span> <span data-ttu-id="1bc77-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="1bc77-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1bc77-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bc77-132">Request headers</span></span>

| <span data-ttu-id="1bc77-133">Имя</span><span class="sxs-lookup"><span data-stu-id="1bc77-133">Name</span></span>          | <span data-ttu-id="1bc77-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1bc77-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1bc77-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1bc77-135">Authorization</span></span> | <span data-ttu-id="1bc77-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bc77-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1bc77-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bc77-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1bc77-139">CSV</span><span class="sxs-lookup"><span data-stu-id="1bc77-139">CSV</span></span>

<span data-ttu-id="1bc77-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="1bc77-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1bc77-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="1bc77-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1bc77-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1bc77-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1bc77-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="1bc77-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1bc77-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="1bc77-144">Report Refresh Date</span></span>
- <span data-ttu-id="1bc77-145">Visited Page Count (количество посещенных страниц)</span><span class="sxs-lookup"><span data-stu-id="1bc77-145">Visited Page Count</span></span>
- <span data-ttu-id="1bc77-146">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="1bc77-146">Report Date</span></span>
- <span data-ttu-id="1bc77-147">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="1bc77-147">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1bc77-148">JSON</span><span class="sxs-lookup"><span data-stu-id="1bc77-148">JSON</span></span>

<span data-ttu-id="1bc77-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[шарепоинтактивитипажес](../resources/sharepointactivitypages.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1bc77-149">If successful, this method returns a `200 OK` response code and a **[sharePointActivityPages](../resources/sharepointactivitypages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bc77-150">Пример</span><span class="sxs-lookup"><span data-stu-id="1bc77-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1bc77-151">CSV</span><span class="sxs-lookup"><span data-stu-id="1bc77-151">CSV</span></span>

<span data-ttu-id="1bc77-152">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="1bc77-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1bc77-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bc77-153">Request</span></span>

<span data-ttu-id="1bc77-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bc77-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1bc77-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bc77-155">Response</span></span>

<span data-ttu-id="1bc77-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1bc77-156">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1bc77-157">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="1bc77-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page Count,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="1bc77-158">JSON</span><span class="sxs-lookup"><span data-stu-id="1bc77-158">JSON</span></span>

<span data-ttu-id="1bc77-159">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="1bc77-159">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1bc77-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bc77-160">Request</span></span>

<span data-ttu-id="1bc77-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bc77-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1bc77-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bc77-162">Response</span></span>

<span data-ttu-id="1bc77-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1bc77-163">The following is an example of the response.</span></span>

> <span data-ttu-id="1bc77-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bc77-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityPages)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPageCount": 195, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
