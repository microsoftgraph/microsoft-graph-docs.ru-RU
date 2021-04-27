---
title: 'reportRoot: getYammerActivityCounts'
description: Отслеживайте динамику активности пользователей в Yammer по количеству опубликованных, прочитанных и понравившихся сообщений.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 0562789163e27b46d5e45dbd087c850aec80cf88
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054989"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="a5a4c-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="a5a4c-103">reportRoot: getYammerActivityCounts</span></span>

<span data-ttu-id="a5a4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5a4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5a4c-105">Отследите динамику использования Yammer в организации по количеству опубликованных, прочитанных и понравившихся сообщений.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-105">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="a5a4c-106">**Примечание:** Подробные сведения о различных представлениях и именах [отчетов см. в Microsoft 365 отчеты - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="a5a4c-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="a5a4c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5a4c-107">Permissions</span></span>

<span data-ttu-id="a5a4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5a4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5a4c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5a4c-110">Permission type</span></span>                        | <span data-ttu-id="a5a4c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5a4c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a5a4c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5a4c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5a4c-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5a4c-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a5a4c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5a4c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5a4c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-115">Not supported.</span></span>                           |
| <span data-ttu-id="a5a4c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5a4c-116">Application</span></span>                            | <span data-ttu-id="a5a4c-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5a4c-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="a5a4c-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a5a4c-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a5a4c-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a5a4c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5a4c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a5a4c-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="a5a4c-121">Function parameters</span></span>

<span data-ttu-id="a5a4c-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a5a4c-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="a5a4c-123">Parameter</span></span> | <span data-ttu-id="a5a4c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a5a4c-124">Type</span></span>   | <span data-ttu-id="a5a4c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a5a4c-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a5a4c-126">period</span><span class="sxs-lookup"><span data-stu-id="a5a4c-126">period</span></span>    | <span data-ttu-id="a5a4c-127">string</span><span class="sxs-lookup"><span data-stu-id="a5a4c-127">string</span></span> | <span data-ttu-id="a5a4c-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a5a4c-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a5a4c-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a5a4c-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-131">Required.</span></span> |

<span data-ttu-id="a5a4c-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a5a4c-133">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-133">The default output type is text/csv.</span></span> <span data-ttu-id="a5a4c-134">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5a4c-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5a4c-135">Request headers</span></span>

| <span data-ttu-id="a5a4c-136">Имя</span><span class="sxs-lookup"><span data-stu-id="a5a4c-136">Name</span></span>          | <span data-ttu-id="a5a4c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="a5a4c-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a5a4c-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5a4c-138">Authorization</span></span> | <span data-ttu-id="a5a4c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a5a4c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5a4c-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a5a4c-142">CSV</span><span class="sxs-lookup"><span data-stu-id="a5a4c-142">CSV</span></span>

<span data-ttu-id="a5a4c-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a5a4c-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a5a4c-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a5a4c-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="a5a4c-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a5a4c-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="a5a4c-147">Report Refresh Date</span></span>
- <span data-ttu-id="a5a4c-148">"Liked" (Понравилось);</span><span class="sxs-lookup"><span data-stu-id="a5a4c-148">Liked</span></span>
- <span data-ttu-id="a5a4c-149">"Posted" (Опубликовано);</span><span class="sxs-lookup"><span data-stu-id="a5a4c-149">Posted</span></span>
- <span data-ttu-id="a5a4c-150">"Read" (Чтение);</span><span class="sxs-lookup"><span data-stu-id="a5a4c-150">Read</span></span>
- <span data-ttu-id="a5a4c-151">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="a5a4c-151">Report Date</span></span>
- <span data-ttu-id="a5a4c-152">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="a5a4c-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a5a4c-153">JSON</span><span class="sxs-lookup"><span data-stu-id="a5a4c-153">JSON</span></span>

<span data-ttu-id="a5a4c-154">В случае успешной работы этот метод возвращает код ответа и `200 OK` **[объект yammerActivitySummary](../resources/yammeractivitysummary.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-154">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5a4c-155">Пример</span><span class="sxs-lookup"><span data-stu-id="a5a4c-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a5a4c-156">CSV</span><span class="sxs-lookup"><span data-stu-id="a5a4c-156">CSV</span></span>

<span data-ttu-id="a5a4c-157">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a5a4c-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5a4c-158">Request</span></span>

<span data-ttu-id="a5a4c-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-159">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammeractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="a5a4c-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5a4c-160">Response</span></span>

<span data-ttu-id="a5a4c-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a5a4c-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="a5a4c-163">JSON</span><span class="sxs-lookup"><span data-stu-id="a5a4c-163">JSON</span></span>

<span data-ttu-id="a5a4c-164">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a5a4c-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5a4c-165">Request</span></span>

<span data-ttu-id="a5a4c-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-166">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammeractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="a5a4c-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5a4c-167">Response</span></span>

<span data-ttu-id="a5a4c-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-168">The following is an example of the response.</span></span>

> <span data-ttu-id="a5a4c-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a5a4c-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 47, 
      "posted": 59, 
      "read": 986, 
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


