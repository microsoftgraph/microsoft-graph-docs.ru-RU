---
title: 'reportRoot: getOffice365ActivationCounts'
description: Получите количество активаций Office 365 на компьютерах и мобильных устройствах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f71a38c9c3d2264a0414bf03041d7a9132bfccb9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869155"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="6f668-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="6f668-103">reportRoot: getOffice365ActivationCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f668-104">Получите количество активаций Office 365 на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="6f668-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="6f668-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="6f668-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="6f668-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f668-106">Permissions</span></span>

<span data-ttu-id="6f668-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f668-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f668-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f668-109">Permission type</span></span>                        | <span data-ttu-id="6f668-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f668-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6f668-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f668-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f668-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f668-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6f668-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f668-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f668-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f668-114">Not supported.</span></span>                           |
| <span data-ttu-id="6f668-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f668-115">Application</span></span>                            | <span data-ttu-id="6f668-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f668-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="6f668-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6f668-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="6f668-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="6f668-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="6f668-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f668-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="6f668-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="6f668-120">Query parameters</span></span>

<span data-ttu-id="6f668-121">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6f668-121">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6f668-122">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="6f668-122">The default output type is text/csv.</span></span> <span data-ttu-id="6f668-123">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="6f668-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f668-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f668-124">Request headers</span></span>

| <span data-ttu-id="6f668-125">Имя</span><span class="sxs-lookup"><span data-stu-id="6f668-125">Name</span></span>          | <span data-ttu-id="6f668-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6f668-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6f668-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f668-127">Authorization</span></span> | <span data-ttu-id="6f668-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f668-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6f668-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f668-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6f668-131">CSV</span><span class="sxs-lookup"><span data-stu-id="6f668-131">CSV</span></span>

<span data-ttu-id="6f668-132">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6f668-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6f668-133">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6f668-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6f668-134">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6f668-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6f668-135">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6f668-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6f668-136">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="6f668-136">Report Refresh Date</span></span>
- <span data-ttu-id="6f668-137">Product Type (Тип продукта)</span><span class="sxs-lookup"><span data-stu-id="6f668-137">Product Type</span></span>
- <span data-ttu-id="6f668-138">Windows</span><span class="sxs-lookup"><span data-stu-id="6f668-138">Windows</span></span>
- <span data-ttu-id="6f668-139">Mac</span><span class="sxs-lookup"><span data-stu-id="6f668-139">Mac</span></span>
- <span data-ttu-id="6f668-140">Android</span><span class="sxs-lookup"><span data-stu-id="6f668-140">Android</span></span>
- <span data-ttu-id="6f668-141">iOS</span><span class="sxs-lookup"><span data-stu-id="6f668-141">iOS</span></span>
- <span data-ttu-id="6f668-142">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="6f668-142">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="6f668-143">JSON</span><span class="sxs-lookup"><span data-stu-id="6f668-143">JSON</span></span>

<span data-ttu-id="6f668-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365ActivationCounts](../resources/office365activationcounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f668-144">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f668-145">Пример</span><span class="sxs-lookup"><span data-stu-id="6f668-145">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6f668-146">CSV</span><span class="sxs-lookup"><span data-stu-id="6f668-146">CSV</span></span>

<span data-ttu-id="6f668-147">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="6f668-147">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6f668-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f668-148">Request</span></span>

<span data-ttu-id="6f668-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f668-149">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6f668-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f668-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6f668-151">C#</span><span class="sxs-lookup"><span data-stu-id="6f668-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f668-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f668-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6f668-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f668-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f668-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f668-154">Response</span></span>

<span data-ttu-id="6f668-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6f668-155">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6f668-156">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6f668-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="6f668-157">JSON</span><span class="sxs-lookup"><span data-stu-id="6f668-157">JSON</span></span>

<span data-ttu-id="6f668-158">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="6f668-158">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6f668-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f668-159">Request</span></span>

<span data-ttu-id="6f668-160">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f668-160">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6f668-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f668-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6f668-162">C#</span><span class="sxs-lookup"><span data-stu-id="6f668-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f668-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f668-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6f668-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f668-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f668-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f668-165">Response</span></span>

<span data-ttu-id="6f668-166">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6f668-166">The following example shows the response.</span></span>

> <span data-ttu-id="6f668-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f668-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
