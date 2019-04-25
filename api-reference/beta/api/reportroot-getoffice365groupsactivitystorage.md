---
title: 'reportRoot: getOffice365GroupsActivityStorage'
description: Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4248251bac7146334dc97e8101f29d53faacf2d5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545963"
---
# <a name="reportroot-getoffice365groupsactivitystorage"></a><span data-ttu-id="4c438-103">reportRoot: getOffice365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="4c438-103">reportRoot: getOffice365GroupsActivityStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c438-104">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="4c438-104">Get the total storage used across all group mailboxes and group sites.</span></span>

> <span data-ttu-id="4c438-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="4c438-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c438-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c438-106">Permissions</span></span>

<span data-ttu-id="4c438-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c438-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c438-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c438-109">Permission type</span></span>                        | <span data-ttu-id="4c438-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c438-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4c438-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c438-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c438-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c438-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4c438-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c438-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c438-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c438-114">Not supported.</span></span>                           |
| <span data-ttu-id="4c438-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c438-115">Application</span></span>                            | <span data-ttu-id="4c438-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c438-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4c438-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c438-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4c438-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4c438-118">Function parameters</span></span>

<span data-ttu-id="4c438-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4c438-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4c438-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="4c438-120">Parameter</span></span> | <span data-ttu-id="4c438-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4c438-121">Type</span></span>   | <span data-ttu-id="4c438-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4c438-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4c438-123">period</span><span class="sxs-lookup"><span data-stu-id="4c438-123">period</span></span>    | <span data-ttu-id="4c438-124">string</span><span class="sxs-lookup"><span data-stu-id="4c438-124">string</span></span> | <span data-ttu-id="4c438-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4c438-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4c438-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4c438-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4c438-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4c438-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4c438-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c438-128">Required.</span></span> |

<span data-ttu-id="4c438-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4c438-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4c438-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="4c438-130">The default output type is text/csv.</span></span> <span data-ttu-id="4c438-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="4c438-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c438-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c438-132">Request headers</span></span>

| <span data-ttu-id="4c438-133">Имя</span><span class="sxs-lookup"><span data-stu-id="4c438-133">Name</span></span>          | <span data-ttu-id="4c438-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4c438-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4c438-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c438-135">Authorization</span></span> | <span data-ttu-id="4c438-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c438-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4c438-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c438-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4c438-139">CSV</span><span class="sxs-lookup"><span data-stu-id="4c438-139">CSV</span></span>

<span data-ttu-id="4c438-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4c438-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4c438-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4c438-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4c438-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4c438-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4c438-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4c438-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4c438-144">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="4c438-144">Report Refresh Date</span></span>
- <span data-ttu-id="4c438-145">Mailbox Storage Used (Byte) [занято почтовыми ящиками (байт)]</span><span class="sxs-lookup"><span data-stu-id="4c438-145">Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="4c438-146">Site Storage Used (Byte) [занято сайтами (байт)]</span><span class="sxs-lookup"><span data-stu-id="4c438-146">Site Storage Used (Byte)</span></span>
- <span data-ttu-id="4c438-147">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="4c438-147">Report Date</span></span>
- <span data-ttu-id="4c438-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="4c438-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4c438-149">JSON</span><span class="sxs-lookup"><span data-stu-id="4c438-149">JSON</span></span>

<span data-ttu-id="4c438-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c438-150">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c438-151">Пример</span><span class="sxs-lookup"><span data-stu-id="4c438-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4c438-152">CSV</span><span class="sxs-lookup"><span data-stu-id="4c438-152">CSV</span></span>

<span data-ttu-id="4c438-153">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="4c438-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4c438-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c438-154">Request</span></span>

<span data-ttu-id="4c438-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c438-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitystorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4c438-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c438-156">Response</span></span>

<span data-ttu-id="4c438-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c438-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4c438-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4c438-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mailbox Storage Used (Byte),Site Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="4c438-159">JSON</span><span class="sxs-lookup"><span data-stu-id="4c438-159">JSON</span></span>

<span data-ttu-id="4c438-160">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="4c438-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4c438-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c438-161">Request</span></span>

<span data-ttu-id="4c438-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c438-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitystorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4c438-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c438-163">Response</span></span>

<span data-ttu-id="4c438-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c438-164">The following is an example of the response.</span></span>

> <span data-ttu-id="4c438-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c438-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailboxStorageUsedInBytes": 523143237898, 
      "siteStorageUsedInBytes": 31124384, 
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
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitystorage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
