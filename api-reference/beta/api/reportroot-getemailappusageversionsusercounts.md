---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.
ms.openlocfilehash: fd172e97b5c7c036fb33e3d4ab0e8088d9d0af7e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081704"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="f7855-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="f7855-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

> <span data-ttu-id="f7855-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f7855-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7855-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7855-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f7855-106">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="f7855-106">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="f7855-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="f7855-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7855-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7855-108">Permissions</span></span>

<span data-ttu-id="f7855-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7855-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7855-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7855-111">Permission type</span></span>                        | <span data-ttu-id="f7855-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7855-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f7855-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7855-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7855-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7855-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f7855-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7855-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7855-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7855-116">Not supported.</span></span>                           |
| <span data-ttu-id="f7855-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7855-117">Application</span></span>                            | <span data-ttu-id="f7855-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7855-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f7855-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7855-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f7855-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="f7855-120">Function parameters</span></span>

<span data-ttu-id="f7855-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="f7855-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f7855-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="f7855-122">Parameter</span></span> | <span data-ttu-id="f7855-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f7855-123">Type</span></span>   | <span data-ttu-id="f7855-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f7855-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f7855-125">period</span><span class="sxs-lookup"><span data-stu-id="f7855-125">period</span></span>    | <span data-ttu-id="f7855-126">строка</span><span class="sxs-lookup"><span data-stu-id="f7855-126">string</span></span> | <span data-ttu-id="f7855-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f7855-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f7855-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="f7855-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f7855-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="f7855-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f7855-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7855-130">Required.</span></span> |

<span data-ttu-id="f7855-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f7855-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f7855-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="f7855-132">The default output type is text/csv.</span></span> <span data-ttu-id="f7855-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="f7855-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7855-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7855-134">Request headers</span></span>

| <span data-ttu-id="f7855-135">Имя</span><span class="sxs-lookup"><span data-stu-id="f7855-135">Name</span></span>          | <span data-ttu-id="f7855-136">Описание</span><span class="sxs-lookup"><span data-stu-id="f7855-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f7855-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7855-137">Authorization</span></span> | <span data-ttu-id="f7855-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7855-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f7855-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7855-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f7855-141">CSV</span><span class="sxs-lookup"><span data-stu-id="f7855-141">CSV</span></span>

<span data-ttu-id="f7855-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="f7855-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f7855-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="f7855-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f7855-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f7855-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f7855-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="f7855-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f7855-146">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="f7855-146">Report Refresh Date</span></span>
- <span data-ttu-id="f7855-147">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="f7855-147">Outlook 2016</span></span>
- <span data-ttu-id="f7855-148">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="f7855-148">Outlook 2013</span></span>
- <span data-ttu-id="f7855-149">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="f7855-149">Outlook 2010</span></span>
- <span data-ttu-id="f7855-150">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="f7855-150">Outlook 2007</span></span>
- <span data-ttu-id="f7855-151">Undetermined (не определено)</span><span class="sxs-lookup"><span data-stu-id="f7855-151">Undetermined</span></span>
- <span data-ttu-id="f7855-152">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="f7855-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f7855-153">JSON</span><span class="sxs-lookup"><span data-stu-id="f7855-153">JSON</span></span>

<span data-ttu-id="f7855-154">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f7855-154">If successful, this method returns a `200 OK` response code and an **[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7855-155">Пример</span><span class="sxs-lookup"><span data-stu-id="f7855-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f7855-156">CSV</span><span class="sxs-lookup"><span data-stu-id="f7855-156">CSV</span></span>

<span data-ttu-id="f7855-157">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="f7855-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f7855-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7855-158">Request</span></span>

<span data-ttu-id="f7855-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7855-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f7855-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7855-160">Response</span></span>

<span data-ttu-id="f7855-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f7855-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f7855-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="f7855-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period
```

### <a name="json"></a><span data-ttu-id="f7855-163">JSON</span><span class="sxs-lookup"><span data-stu-id="f7855-163">JSON</span></span>

<span data-ttu-id="f7855-164">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="f7855-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f7855-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7855-165">Request</span></span>

<span data-ttu-id="f7855-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7855-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f7855-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7855-167">Response</span></span>

<span data-ttu-id="f7855-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7855-168">The following is an example of the response.</span></span>

> <span data-ttu-id="f7855-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7855-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageVersionsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "outlook2016": 1554, 
      "outlook2013": 64, 
      "outlook2010": 1, 
      "outlook2007": 0, 
      "undetermined": 1259, 
      "reportPeriod": "7"
    }
  ]
}
```
