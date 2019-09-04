---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Получите сведения о пользователях, которые активировали Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 6a2485653f69fb9c403a3b5bf893c7cf6ee150e7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723072"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="d4657-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="d4657-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4657-104">Получите сведения о пользователях, которые активировали Office 365.</span><span class="sxs-lookup"><span data-stu-id="d4657-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="d4657-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="d4657-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4657-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4657-106">Permissions</span></span>

<span data-ttu-id="d4657-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4657-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4657-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4657-109">Permission type</span></span>                        | <span data-ttu-id="d4657-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4657-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d4657-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4657-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4657-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4657-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d4657-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4657-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4657-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4657-114">Not supported.</span></span>                           |
| <span data-ttu-id="d4657-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4657-115">Application</span></span>                            | <span data-ttu-id="d4657-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4657-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d4657-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4657-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="d4657-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="d4657-118">Query parameters</span></span>

<span data-ttu-id="d4657-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d4657-119">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d4657-120">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="d4657-120">The default output type is text/csv.</span></span> <span data-ttu-id="d4657-121">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="d4657-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4657-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4657-122">Request headers</span></span>

| <span data-ttu-id="d4657-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d4657-123">Name</span></span>          | <span data-ttu-id="d4657-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d4657-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d4657-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4657-125">Authorization</span></span> | <span data-ttu-id="d4657-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4657-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d4657-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4657-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d4657-129">CSV</span><span class="sxs-lookup"><span data-stu-id="d4657-129">CSV</span></span>

<span data-ttu-id="d4657-130">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="d4657-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d4657-131">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="d4657-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d4657-132">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d4657-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d4657-133">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="d4657-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d4657-134">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="d4657-134">Report Refresh Date</span></span>
- <span data-ttu-id="d4657-135">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="d4657-135">User Principal Name</span></span>
- <span data-ttu-id="d4657-136">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="d4657-136">Display Name</span></span>
- <span data-ttu-id="d4657-137">Product Type (тип продукта)</span><span class="sxs-lookup"><span data-stu-id="d4657-137">Product Type</span></span>
- <span data-ttu-id="d4657-138">Last Activated Date (дата последней активации)</span><span class="sxs-lookup"><span data-stu-id="d4657-138">Last Activated Date</span></span>
- <span data-ttu-id="d4657-139">Windows</span><span class="sxs-lookup"><span data-stu-id="d4657-139">Windows</span></span>
- <span data-ttu-id="d4657-140">Mac</span><span class="sxs-lookup"><span data-stu-id="d4657-140">Mac</span></span>
- <span data-ttu-id="d4657-141">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="d4657-141">Windows 10 Mobile</span></span>
- <span data-ttu-id="d4657-142">iOS</span><span class="sxs-lookup"><span data-stu-id="d4657-142">iOS</span></span>
- <span data-ttu-id="d4657-143">Android</span><span class="sxs-lookup"><span data-stu-id="d4657-143">Android</span></span>
- <span data-ttu-id="d4657-144">Активирован на общем компьютере</span><span class="sxs-lookup"><span data-stu-id="d4657-144">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="d4657-145">JSON</span><span class="sxs-lookup"><span data-stu-id="d4657-145">JSON</span></span>

<span data-ttu-id="d4657-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4657-146">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="d4657-147">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="d4657-147">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="d4657-148">Пример</span><span class="sxs-lookup"><span data-stu-id="d4657-148">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d4657-149">CSV</span><span class="sxs-lookup"><span data-stu-id="d4657-149">CSV</span></span>

<span data-ttu-id="d4657-150">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="d4657-150">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d4657-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4657-151">Request</span></span>

<span data-ttu-id="d4657-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4657-152">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d4657-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4657-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d4657-154">C#</span><span class="sxs-lookup"><span data-stu-id="d4657-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4657-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4657-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d4657-156">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d4657-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d4657-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4657-157">Response</span></span>

<span data-ttu-id="d4657-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d4657-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d4657-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="d4657-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
```

### <a name="json"></a><span data-ttu-id="d4657-160">JSON</span><span class="sxs-lookup"><span data-stu-id="d4657-160">JSON</span></span>

<span data-ttu-id="d4657-161">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="d4657-161">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d4657-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4657-162">Request</span></span>

<span data-ttu-id="d4657-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4657-163">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d4657-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4657-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d4657-165">C#</span><span class="sxs-lookup"><span data-stu-id="d4657-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4657-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4657-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d4657-167">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d4657-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d4657-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4657-168">Response</span></span>

<span data-ttu-id="d4657-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d4657-169">The following is an example of the response.</span></span>

> <span data-ttu-id="d4657-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4657-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationsUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "userActivationCounts": [
        {
          "productType": "Project Client", 
          "lastActivatedDate": "2017-08-20", 
          "windows": 5, 
          "mac": 0, 
          "windows10Mobile": 0, 
          "ios": 0, 
          "android": 2,
          "activatedOnSharedComputer": true
        }
      ]
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
