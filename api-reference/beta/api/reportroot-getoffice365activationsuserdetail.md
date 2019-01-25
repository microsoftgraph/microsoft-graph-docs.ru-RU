---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Получите сведения о пользователях, которые активировали Office 365.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: c2cea0affc6cbbc67acbe38271bd9c0ac0fbb742
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529028"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="75dda-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="75dda-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75dda-104">Получите сведения о пользователях, которые активировали Office 365.</span><span class="sxs-lookup"><span data-stu-id="75dda-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="75dda-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="75dda-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="75dda-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75dda-106">Permissions</span></span>

<span data-ttu-id="75dda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75dda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75dda-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75dda-109">Permission type</span></span>                        | <span data-ttu-id="75dda-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75dda-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="75dda-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75dda-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="75dda-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="75dda-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="75dda-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75dda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75dda-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75dda-114">Not supported.</span></span>                           |
| <span data-ttu-id="75dda-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75dda-115">Application</span></span>                            | <span data-ttu-id="75dda-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="75dda-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="75dda-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75dda-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="75dda-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="75dda-118">Query parameters</span></span>

<span data-ttu-id="75dda-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="75dda-119">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="75dda-120">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="75dda-120">The default output type is text/csv.</span></span> <span data-ttu-id="75dda-121">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="75dda-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75dda-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75dda-122">Request headers</span></span>

| <span data-ttu-id="75dda-123">Имя</span><span class="sxs-lookup"><span data-stu-id="75dda-123">Name</span></span>          | <span data-ttu-id="75dda-124">Описание</span><span class="sxs-lookup"><span data-stu-id="75dda-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="75dda-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75dda-125">Authorization</span></span> | <span data-ttu-id="75dda-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75dda-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="75dda-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="75dda-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="75dda-129">CSV</span><span class="sxs-lookup"><span data-stu-id="75dda-129">CSV</span></span>

<span data-ttu-id="75dda-130">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="75dda-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="75dda-131">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="75dda-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="75dda-132">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="75dda-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="75dda-133">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="75dda-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="75dda-134">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="75dda-134">Report Refresh Date</span></span>
- <span data-ttu-id="75dda-135">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="75dda-135">User Principal Name</span></span>
- <span data-ttu-id="75dda-136">Display Name (отображаемое имя)</span><span class="sxs-lookup"><span data-stu-id="75dda-136">Display Name</span></span>
- <span data-ttu-id="75dda-137">Product Type (тип продукта)</span><span class="sxs-lookup"><span data-stu-id="75dda-137">Product Type</span></span>
- <span data-ttu-id="75dda-138">Last Activated Date (дата последней активации)</span><span class="sxs-lookup"><span data-stu-id="75dda-138">Last Activated Date</span></span>
- <span data-ttu-id="75dda-139">Windows</span><span class="sxs-lookup"><span data-stu-id="75dda-139">Windows</span></span>
- <span data-ttu-id="75dda-140">Mac</span><span class="sxs-lookup"><span data-stu-id="75dda-140">Mac</span></span>
- <span data-ttu-id="75dda-141">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="75dda-141">Windows 10 Mobile</span></span>
- <span data-ttu-id="75dda-142">iOS</span><span class="sxs-lookup"><span data-stu-id="75dda-142">iOS</span></span>
- <span data-ttu-id="75dda-143">Android</span><span class="sxs-lookup"><span data-stu-id="75dda-143">Android</span></span>
- <span data-ttu-id="75dda-144">Активированные на совместно используемый компьютер</span><span class="sxs-lookup"><span data-stu-id="75dda-144">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="75dda-145">JSON</span><span class="sxs-lookup"><span data-stu-id="75dda-145">JSON</span></span>

<span data-ttu-id="75dda-146">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="75dda-146">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="75dda-147">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="75dda-147">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="75dda-148">Пример</span><span class="sxs-lookup"><span data-stu-id="75dda-148">Example</span></span>

### <a name="csv"></a><span data-ttu-id="75dda-149">CSV</span><span class="sxs-lookup"><span data-stu-id="75dda-149">CSV</span></span>

<span data-ttu-id="75dda-150">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="75dda-150">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="75dda-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="75dda-151">Request</span></span>

<span data-ttu-id="75dda-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75dda-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="75dda-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="75dda-153">Response</span></span>

<span data-ttu-id="75dda-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="75dda-154">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="75dda-155">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="75dda-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="75dda-156">JSON</span><span class="sxs-lookup"><span data-stu-id="75dda-156">JSON</span></span>

<span data-ttu-id="75dda-157">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="75dda-157">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="75dda-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="75dda-158">Request</span></span>

<span data-ttu-id="75dda-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75dda-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="75dda-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="75dda-160">Response</span></span>

<span data-ttu-id="75dda-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75dda-161">The following is an example of the response.</span></span>

> <span data-ttu-id="75dda-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75dda-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activationsuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
