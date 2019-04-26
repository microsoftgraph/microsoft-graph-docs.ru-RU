---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Получите сведения о пользователях, которые активировали Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8f40f2ecc16dbea7c749b5932369063cdaaa85f1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336772"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="c1c03-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="c1c03-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1c03-104">Получите сведения о пользователях, которые активировали Office 365.</span><span class="sxs-lookup"><span data-stu-id="c1c03-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="c1c03-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="c1c03-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1c03-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1c03-106">Permissions</span></span>

<span data-ttu-id="c1c03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1c03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1c03-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1c03-109">Permission type</span></span>                        | <span data-ttu-id="c1c03-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1c03-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c1c03-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1c03-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1c03-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1c03-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c1c03-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1c03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1c03-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1c03-114">Not supported.</span></span>                           |
| <span data-ttu-id="c1c03-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1c03-115">Application</span></span>                            | <span data-ttu-id="c1c03-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1c03-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c1c03-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1c03-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="c1c03-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c1c03-118">Query parameters</span></span>

<span data-ttu-id="c1c03-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c1c03-119">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c1c03-120">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="c1c03-120">The default output type is text/csv.</span></span> <span data-ttu-id="c1c03-121">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="c1c03-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1c03-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1c03-122">Request headers</span></span>

| <span data-ttu-id="c1c03-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c1c03-123">Name</span></span>          | <span data-ttu-id="c1c03-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c1c03-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c1c03-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1c03-125">Authorization</span></span> | <span data-ttu-id="c1c03-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1c03-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c1c03-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1c03-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c1c03-129">CSV</span><span class="sxs-lookup"><span data-stu-id="c1c03-129">CSV</span></span>

<span data-ttu-id="c1c03-130">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c1c03-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c1c03-131">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c1c03-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c1c03-132">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c1c03-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c1c03-133">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c1c03-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c1c03-134">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c1c03-134">Report Refresh Date</span></span>
- <span data-ttu-id="c1c03-135">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="c1c03-135">User Principal Name</span></span>
- <span data-ttu-id="c1c03-136">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="c1c03-136">Display Name</span></span>
- <span data-ttu-id="c1c03-137">Product Type (тип продукта)</span><span class="sxs-lookup"><span data-stu-id="c1c03-137">Product Type</span></span>
- <span data-ttu-id="c1c03-138">Last Activated Date (дата последней активации)</span><span class="sxs-lookup"><span data-stu-id="c1c03-138">Last Activated Date</span></span>
- <span data-ttu-id="c1c03-139">Windows</span><span class="sxs-lookup"><span data-stu-id="c1c03-139">Windows</span></span>
- <span data-ttu-id="c1c03-140">Mac</span><span class="sxs-lookup"><span data-stu-id="c1c03-140">Mac</span></span>
- <span data-ttu-id="c1c03-141">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="c1c03-141">Windows 10 Mobile</span></span>
- <span data-ttu-id="c1c03-142">iOS</span><span class="sxs-lookup"><span data-stu-id="c1c03-142">iOS</span></span>
- <span data-ttu-id="c1c03-143">Android</span><span class="sxs-lookup"><span data-stu-id="c1c03-143">Android</span></span>
- <span data-ttu-id="c1c03-144">Активирован на общем компьютере</span><span class="sxs-lookup"><span data-stu-id="c1c03-144">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="c1c03-145">JSON</span><span class="sxs-lookup"><span data-stu-id="c1c03-145">JSON</span></span>

<span data-ttu-id="c1c03-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1c03-146">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="c1c03-147">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="c1c03-147">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="c1c03-148">Пример</span><span class="sxs-lookup"><span data-stu-id="c1c03-148">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c1c03-149">CSV</span><span class="sxs-lookup"><span data-stu-id="c1c03-149">CSV</span></span>

<span data-ttu-id="c1c03-150">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="c1c03-150">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c1c03-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1c03-151">Request</span></span>

<span data-ttu-id="c1c03-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1c03-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="c1c03-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1c03-153">Response</span></span>

<span data-ttu-id="c1c03-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1c03-154">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c1c03-155">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c1c03-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="c1c03-156">JSON</span><span class="sxs-lookup"><span data-stu-id="c1c03-156">JSON</span></span>

<span data-ttu-id="c1c03-157">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="c1c03-157">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c1c03-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1c03-158">Request</span></span>

<span data-ttu-id="c1c03-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1c03-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="c1c03-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1c03-160">Response</span></span>

<span data-ttu-id="c1c03-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1c03-161">The following is an example of the response.</span></span>

> <span data-ttu-id="c1c03-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1c03-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
