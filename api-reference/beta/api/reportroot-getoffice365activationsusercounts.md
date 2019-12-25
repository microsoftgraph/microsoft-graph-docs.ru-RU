---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Получите число включенных пользователей, которые активировали подписку на Office на настольных компьютерах, устройствах или общих компьютерах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 543ec8169777918874035cadba968144f9f7e11f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867566"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="dcc02-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="dcc02-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcc02-104">Получите число включенных пользователей, которые активировали подписку на Office на настольных компьютерах, устройствах или общих компьютерах.</span><span class="sxs-lookup"><span data-stu-id="dcc02-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="dcc02-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="dcc02-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcc02-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dcc02-106">Permissions</span></span>

<span data-ttu-id="dcc02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcc02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcc02-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcc02-109">Permission type</span></span>                        | <span data-ttu-id="dcc02-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcc02-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dcc02-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcc02-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcc02-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcc02-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dcc02-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcc02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcc02-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcc02-114">Not supported.</span></span>                           |
| <span data-ttu-id="dcc02-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dcc02-115">Application</span></span>                            | <span data-ttu-id="dcc02-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcc02-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="dcc02-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dcc02-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="dcc02-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="dcc02-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="dcc02-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcc02-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="query-parameters"></a><span data-ttu-id="dcc02-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="dcc02-120">Query parameters</span></span>

<span data-ttu-id="dcc02-121">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="dcc02-121">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="dcc02-122">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="dcc02-122">The default output type is text/csv.</span></span> <span data-ttu-id="dcc02-123">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="dcc02-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcc02-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dcc02-124">Request headers</span></span>

| <span data-ttu-id="dcc02-125">Имя</span><span class="sxs-lookup"><span data-stu-id="dcc02-125">Name</span></span>          | <span data-ttu-id="dcc02-126">Описание</span><span class="sxs-lookup"><span data-stu-id="dcc02-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dcc02-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dcc02-127">Authorization</span></span> | <span data-ttu-id="dcc02-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcc02-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="dcc02-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcc02-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="dcc02-131">CSV</span><span class="sxs-lookup"><span data-stu-id="dcc02-131">CSV</span></span>

<span data-ttu-id="dcc02-132">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="dcc02-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dcc02-133">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="dcc02-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dcc02-134">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="dcc02-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dcc02-135">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="dcc02-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dcc02-136">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="dcc02-136">Report Refresh Date</span></span>
- <span data-ttu-id="dcc02-137">"Product Type" (Тип продукта);</span><span class="sxs-lookup"><span data-stu-id="dcc02-137">Product Type</span></span>
- <span data-ttu-id="dcc02-138">"Assigned" (Назначенные);</span><span class="sxs-lookup"><span data-stu-id="dcc02-138">Assigned</span></span>
- <span data-ttu-id="dcc02-139">"Activated" (Активированные).</span><span class="sxs-lookup"><span data-stu-id="dcc02-139">Activated</span></span>
- <span data-ttu-id="dcc02-140">Активация на общем компьютере</span><span class="sxs-lookup"><span data-stu-id="dcc02-140">Shared Computer Activation</span></span>

### <a name="json"></a><span data-ttu-id="dcc02-141">JSON</span><span class="sxs-lookup"><span data-stu-id="dcc02-141">JSON</span></span>

<span data-ttu-id="dcc02-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dcc02-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcc02-143">Пример</span><span class="sxs-lookup"><span data-stu-id="dcc02-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="dcc02-144">CSV</span><span class="sxs-lookup"><span data-stu-id="dcc02-144">CSV</span></span>

<span data-ttu-id="dcc02-145">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="dcc02-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="dcc02-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcc02-146">Request</span></span>

<span data-ttu-id="dcc02-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcc02-147">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dcc02-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcc02-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dcc02-149">C#</span><span class="sxs-lookup"><span data-stu-id="dcc02-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcc02-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcc02-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dcc02-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcc02-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dcc02-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcc02-152">Response</span></span>

<span data-ttu-id="dcc02-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dcc02-153">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="dcc02-154">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="dcc02-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```

### <a name="json"></a><span data-ttu-id="dcc02-155">JSON</span><span class="sxs-lookup"><span data-stu-id="dcc02-155">JSON</span></span>

<span data-ttu-id="dcc02-156">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="dcc02-156">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="dcc02-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcc02-157">Request</span></span>

<span data-ttu-id="dcc02-158">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcc02-158">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dcc02-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcc02-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dcc02-160">C#</span><span class="sxs-lookup"><span data-stu-id="dcc02-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcc02-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcc02-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dcc02-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcc02-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dcc02-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcc02-163">Response</span></span>

<span data-ttu-id="dcc02-164">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dcc02-164">The following example shows the response.</span></span>

> <span data-ttu-id="dcc02-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dcc02-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Office 365 ProPlus", 
      "assigned": 2679, 
      "activated": 1710,
      "sharedComputerActivation": 1024
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
