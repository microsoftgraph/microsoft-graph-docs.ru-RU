---
title: 'reportRoot: getYammerActivityUserCounts'
description: Отслеживайте динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer.
ms.openlocfilehash: 6df8a0f16e8cb4c10e05484eeecf1f4e60c4c889
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082882"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="1c0f5-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="1c0f5-103">reportRoot: getYammerActivityUserCounts</span></span>

> <span data-ttu-id="1c0f5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c0f5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c0f5-106">Отслеживайте динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-106">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="1c0f5-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="1c0f5-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c0f5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c0f5-108">Permissions</span></span>

<span data-ttu-id="1c0f5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c0f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c0f5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c0f5-111">Permission type</span></span>                        | <span data-ttu-id="1c0f5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c0f5-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1c0f5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c0f5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c0f5-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c0f5-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1c0f5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c0f5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c0f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-116">Not supported.</span></span>                           |
| <span data-ttu-id="1c0f5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c0f5-117">Application</span></span>                            | <span data-ttu-id="1c0f5-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c0f5-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1c0f5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c0f5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1c0f5-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="1c0f5-120">Function parameters</span></span>

<span data-ttu-id="1c0f5-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1c0f5-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="1c0f5-122">Parameter</span></span> | <span data-ttu-id="1c0f5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="1c0f5-123">Type</span></span>   | <span data-ttu-id="1c0f5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1c0f5-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1c0f5-125">period</span><span class="sxs-lookup"><span data-stu-id="1c0f5-125">period</span></span>    | <span data-ttu-id="1c0f5-126">строка</span><span class="sxs-lookup"><span data-stu-id="1c0f5-126">string</span></span> | <span data-ttu-id="1c0f5-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1c0f5-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1c0f5-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1c0f5-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-130">Required.</span></span> |

<span data-ttu-id="1c0f5-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1c0f5-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-132">The default output type is text/csv.</span></span> <span data-ttu-id="1c0f5-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c0f5-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c0f5-134">Request headers</span></span>

| <span data-ttu-id="1c0f5-135">Имя</span><span class="sxs-lookup"><span data-stu-id="1c0f5-135">Name</span></span>          | <span data-ttu-id="1c0f5-136">Описание</span><span class="sxs-lookup"><span data-stu-id="1c0f5-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1c0f5-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c0f5-137">Authorization</span></span> | <span data-ttu-id="1c0f5-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1c0f5-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c0f5-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1c0f5-141">CSV</span><span class="sxs-lookup"><span data-stu-id="1c0f5-141">CSV</span></span>

<span data-ttu-id="1c0f5-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1c0f5-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1c0f5-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1c0f5-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="1c0f5-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1c0f5-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="1c0f5-146">Report Refresh Date</span></span>
- <span data-ttu-id="1c0f5-147">"Liked" (Понравилось);</span><span class="sxs-lookup"><span data-stu-id="1c0f5-147">Liked</span></span>
- <span data-ttu-id="1c0f5-148">"Posted" (Опубликовано);</span><span class="sxs-lookup"><span data-stu-id="1c0f5-148">Posted</span></span>
- <span data-ttu-id="1c0f5-149">"Read" (Чтение);</span><span class="sxs-lookup"><span data-stu-id="1c0f5-149">Read</span></span>
- <span data-ttu-id="1c0f5-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="1c0f5-150">Report Date</span></span>
- <span data-ttu-id="1c0f5-151">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="1c0f5-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1c0f5-152">JSON</span><span class="sxs-lookup"><span data-stu-id="1c0f5-152">JSON</span></span>

<span data-ttu-id="1c0f5-153">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[yammerActivitySummary](../resources/yammeractivitysummary.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-153">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c0f5-154">Пример</span><span class="sxs-lookup"><span data-stu-id="1c0f5-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1c0f5-155">CSV</span><span class="sxs-lookup"><span data-stu-id="1c0f5-155">CSV</span></span>

<span data-ttu-id="1c0f5-156">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1c0f5-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c0f5-157">Request</span></span>

<span data-ttu-id="1c0f5-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1c0f5-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c0f5-159">Response</span></span>

<span data-ttu-id="1c0f5-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1c0f5-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="1c0f5-162">JSON</span><span class="sxs-lookup"><span data-stu-id="1c0f5-162">JSON</span></span>

<span data-ttu-id="1c0f5-163">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1c0f5-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c0f5-164">Request</span></span>

<span data-ttu-id="1c0f5-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1c0f5-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c0f5-166">Response</span></span>

<span data-ttu-id="1c0f5-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-167">The following is an example of the response.</span></span>

> <span data-ttu-id="1c0f5-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c0f5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 40, 
      "posted": 54, 
      "read": 28, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
