---
title: 'reportRoot: getOffice365ActivationCounts'
description: Получите количество активаций Office 365 на компьютерах и мобильных устройствах.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 88ee061ba61f9a0be4c8faa35f966749bf65ae76
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509415"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="2baef-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="2baef-103">reportRoot: getOffice365ActivationCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2baef-104">Получите количество активаций Office 365 на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="2baef-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="2baef-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="2baef-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="2baef-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2baef-106">Permissions</span></span>

<span data-ttu-id="2baef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2baef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2baef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2baef-109">Permission type</span></span>                        | <span data-ttu-id="2baef-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2baef-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2baef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2baef-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2baef-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2baef-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2baef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2baef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2baef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2baef-114">Not supported.</span></span>                           |
| <span data-ttu-id="2baef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2baef-115">Application</span></span>                            | <span data-ttu-id="2baef-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2baef-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2baef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2baef-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="2baef-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="2baef-118">Query parameters</span></span>

<span data-ttu-id="2baef-119">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2baef-119">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2baef-120">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="2baef-120">The default output type is text/csv.</span></span> <span data-ttu-id="2baef-121">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="2baef-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2baef-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2baef-122">Request headers</span></span>

| <span data-ttu-id="2baef-123">Имя</span><span class="sxs-lookup"><span data-stu-id="2baef-123">Name</span></span>          | <span data-ttu-id="2baef-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2baef-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2baef-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2baef-125">Authorization</span></span> | <span data-ttu-id="2baef-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2baef-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2baef-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2baef-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2baef-129">CSV</span><span class="sxs-lookup"><span data-stu-id="2baef-129">CSV</span></span>

<span data-ttu-id="2baef-130">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="2baef-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2baef-131">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="2baef-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2baef-132">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2baef-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2baef-133">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="2baef-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2baef-134">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="2baef-134">Report Refresh Date</span></span>
- <span data-ttu-id="2baef-135">Product Type (Тип продукта)</span><span class="sxs-lookup"><span data-stu-id="2baef-135">Product Type</span></span>
- <span data-ttu-id="2baef-136">Windows</span><span class="sxs-lookup"><span data-stu-id="2baef-136">Windows</span></span>
- <span data-ttu-id="2baef-137">Mac</span><span class="sxs-lookup"><span data-stu-id="2baef-137">Mac</span></span>
- <span data-ttu-id="2baef-138">Android</span><span class="sxs-lookup"><span data-stu-id="2baef-138">Android</span></span>
- <span data-ttu-id="2baef-139">iOS</span><span class="sxs-lookup"><span data-stu-id="2baef-139">iOS</span></span>
- <span data-ttu-id="2baef-140">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="2baef-140">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="2baef-141">JSON</span><span class="sxs-lookup"><span data-stu-id="2baef-141">JSON</span></span>

<span data-ttu-id="2baef-142">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[office365ActivationCounts](../resources/office365activationcounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2baef-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2baef-143">Пример</span><span class="sxs-lookup"><span data-stu-id="2baef-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2baef-144">CSV</span><span class="sxs-lookup"><span data-stu-id="2baef-144">CSV</span></span>

<span data-ttu-id="2baef-145">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="2baef-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2baef-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="2baef-146">Request</span></span>

<span data-ttu-id="2baef-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2baef-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="2baef-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="2baef-148">Response</span></span>

<span data-ttu-id="2baef-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2baef-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2baef-150">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="2baef-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```

### <a name="json"></a><span data-ttu-id="2baef-151">JSON</span><span class="sxs-lookup"><span data-stu-id="2baef-151">JSON</span></span>

<span data-ttu-id="2baef-152">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="2baef-152">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2baef-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="2baef-153">Request</span></span>

<span data-ttu-id="2baef-154">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2baef-154">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="2baef-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="2baef-155">Response</span></span>

<span data-ttu-id="2baef-156">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2baef-156">The following example shows the response.</span></span>

> <span data-ttu-id="2baef-p105">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2baef-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Office 365 ProPlus", 
      "windows": 9157, 
      "mac": 576, 
      "android": 358, 
      "ios": 1452, 
      "windows10Mobile": 2309
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
