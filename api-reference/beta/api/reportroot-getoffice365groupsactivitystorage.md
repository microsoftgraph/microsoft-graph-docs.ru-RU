---
title: 'reportRoot: getOffice365GroupsActivityStorage'
description: Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 92ddfefd0aba712afdd1fb85aa4bfc0e5f768118
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589043"
---
# <a name="reportroot-getoffice365groupsactivitystorage"></a><span data-ttu-id="23007-103">reportRoot: getOffice365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="23007-103">reportRoot: getOffice365GroupsActivityStorage</span></span>

<span data-ttu-id="23007-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23007-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23007-105">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="23007-105">Get the total storage used across all group mailboxes and group sites.</span></span>

> <span data-ttu-id="23007-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="23007-106">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="23007-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23007-107">Permissions</span></span>

<span data-ttu-id="23007-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23007-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23007-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23007-110">Permission type</span></span>                        | <span data-ttu-id="23007-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23007-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="23007-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23007-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="23007-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23007-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="23007-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23007-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23007-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23007-115">Not supported.</span></span>                           |
| <span data-ttu-id="23007-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23007-116">Application</span></span>                            | <span data-ttu-id="23007-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23007-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="23007-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="23007-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="23007-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="23007-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="23007-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23007-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="23007-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="23007-121">Function parameters</span></span>

<span data-ttu-id="23007-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="23007-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="23007-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="23007-123">Parameter</span></span> | <span data-ttu-id="23007-124">Тип</span><span class="sxs-lookup"><span data-stu-id="23007-124">Type</span></span>   | <span data-ttu-id="23007-125">Описание</span><span class="sxs-lookup"><span data-stu-id="23007-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="23007-126">period</span><span class="sxs-lookup"><span data-stu-id="23007-126">period</span></span>    | <span data-ttu-id="23007-127">string</span><span class="sxs-lookup"><span data-stu-id="23007-127">string</span></span> | <span data-ttu-id="23007-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="23007-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="23007-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="23007-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="23007-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="23007-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="23007-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23007-131">Required.</span></span> |

<span data-ttu-id="23007-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="23007-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="23007-133">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="23007-133">The default output type is text/csv.</span></span> <span data-ttu-id="23007-134">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="23007-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23007-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23007-135">Request headers</span></span>

| <span data-ttu-id="23007-136">Имя</span><span class="sxs-lookup"><span data-stu-id="23007-136">Name</span></span>          | <span data-ttu-id="23007-137">Описание</span><span class="sxs-lookup"><span data-stu-id="23007-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="23007-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23007-138">Authorization</span></span> | <span data-ttu-id="23007-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23007-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="23007-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="23007-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="23007-142">CSV</span><span class="sxs-lookup"><span data-stu-id="23007-142">CSV</span></span>

<span data-ttu-id="23007-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="23007-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="23007-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="23007-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="23007-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="23007-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="23007-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="23007-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="23007-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="23007-147">Report Refresh Date</span></span>
- <span data-ttu-id="23007-148">Mailbox Storage Used (Byte) [занято почтовыми ящиками (байт)]</span><span class="sxs-lookup"><span data-stu-id="23007-148">Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="23007-149">Site Storage Used (Byte) [занято сайтами (байт)]</span><span class="sxs-lookup"><span data-stu-id="23007-149">Site Storage Used (Byte)</span></span>
- <span data-ttu-id="23007-150">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="23007-150">Report Date</span></span>
- <span data-ttu-id="23007-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="23007-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="23007-152">JSON</span><span class="sxs-lookup"><span data-stu-id="23007-152">JSON</span></span>

<span data-ttu-id="23007-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23007-153">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23007-154">Пример</span><span class="sxs-lookup"><span data-stu-id="23007-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="23007-155">CSV</span><span class="sxs-lookup"><span data-stu-id="23007-155">CSV</span></span>

<span data-ttu-id="23007-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="23007-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="23007-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="23007-157">Request</span></span>

<span data-ttu-id="23007-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23007-158">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivitystorage_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityStorage(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="23007-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="23007-159">Response</span></span>

<span data-ttu-id="23007-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23007-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="23007-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="23007-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="23007-162">JSON</span><span class="sxs-lookup"><span data-stu-id="23007-162">JSON</span></span>

<span data-ttu-id="23007-163">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="23007-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="23007-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="23007-164">Request</span></span>

<span data-ttu-id="23007-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23007-165">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivitystorage_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityStorage(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="23007-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="23007-166">Response</span></span>

<span data-ttu-id="23007-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23007-167">The following is an example of the response.</span></span>

> <span data-ttu-id="23007-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23007-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
