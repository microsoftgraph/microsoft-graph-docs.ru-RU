---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Получение сведений о пользователях, которые активировали Microsoft 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 83a8f5737bb80654f3c6bb10fcba9dc85c578612
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896331"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="2375f-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="2375f-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="2375f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2375f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2375f-105">Получение сведений о пользователях, которые активировали Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2375f-105">Get details about users who have activated Microsoft 365.</span></span>

> <span data-ttu-id="2375f-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports — активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="2375f-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="2375f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2375f-107">Permissions</span></span>

<span data-ttu-id="2375f-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="2375f-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2375f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2375f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2375f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2375f-110">Permission type</span></span>                        | <span data-ttu-id="2375f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2375f-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2375f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2375f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2375f-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2375f-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2375f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2375f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2375f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2375f-115">Not supported.</span></span>                           |
| <span data-ttu-id="2375f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2375f-116">Application</span></span>                            | <span data-ttu-id="2375f-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2375f-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="2375f-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2375f-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="2375f-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="2375f-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="2375f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2375f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="2375f-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="2375f-121">Query parameters</span></span>

<span data-ttu-id="2375f-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2375f-122">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2375f-123">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="2375f-123">The default output type is text/csv.</span></span> <span data-ttu-id="2375f-124">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="2375f-124">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2375f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2375f-125">Request headers</span></span>

| <span data-ttu-id="2375f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="2375f-126">Name</span></span>          | <span data-ttu-id="2375f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="2375f-127">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2375f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2375f-128">Authorization</span></span> | <span data-ttu-id="2375f-129">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="2375f-129">Bearer {token}.</span></span> <span data-ttu-id="2375f-130">Required.</span><span class="sxs-lookup"><span data-stu-id="2375f-130">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2375f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2375f-131">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2375f-132">CSV</span><span class="sxs-lookup"><span data-stu-id="2375f-132">CSV</span></span>

<span data-ttu-id="2375f-133">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="2375f-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2375f-134">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="2375f-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2375f-135">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2375f-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2375f-136">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="2375f-136">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2375f-137">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="2375f-137">Report Refresh Date</span></span>
- <span data-ttu-id="2375f-138">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="2375f-138">User Principal Name</span></span>
- <span data-ttu-id="2375f-139">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="2375f-139">Display Name</span></span>
- <span data-ttu-id="2375f-140">Product Type (тип продукта)</span><span class="sxs-lookup"><span data-stu-id="2375f-140">Product Type</span></span>
- <span data-ttu-id="2375f-141">Last Activated Date (дата последней активации)</span><span class="sxs-lookup"><span data-stu-id="2375f-141">Last Activated Date</span></span>
- <span data-ttu-id="2375f-142">Windows</span><span class="sxs-lookup"><span data-stu-id="2375f-142">Windows</span></span>
- <span data-ttu-id="2375f-143">Mac</span><span class="sxs-lookup"><span data-stu-id="2375f-143">Mac</span></span>
- <span data-ttu-id="2375f-144">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="2375f-144">Windows 10 Mobile</span></span>
- <span data-ttu-id="2375f-145">iOS</span><span class="sxs-lookup"><span data-stu-id="2375f-145">iOS</span></span>
- <span data-ttu-id="2375f-146">Android</span><span class="sxs-lookup"><span data-stu-id="2375f-146">Android</span></span>
- <span data-ttu-id="2375f-147">Активирован на общем компьютере</span><span class="sxs-lookup"><span data-stu-id="2375f-147">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="2375f-148">JSON</span><span class="sxs-lookup"><span data-stu-id="2375f-148">JSON</span></span>

<span data-ttu-id="2375f-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2375f-149">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="2375f-150">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="2375f-150">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="2375f-151">Пример</span><span class="sxs-lookup"><span data-stu-id="2375f-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2375f-152">CSV</span><span class="sxs-lookup"><span data-stu-id="2375f-152">CSV</span></span>

<span data-ttu-id="2375f-153">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="2375f-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2375f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="2375f-154">Request</span></span>

<span data-ttu-id="2375f-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2375f-155">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="2375f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="2375f-156">Response</span></span>

<span data-ttu-id="2375f-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2375f-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2375f-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="2375f-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="2375f-159">JSON</span><span class="sxs-lookup"><span data-stu-id="2375f-159">JSON</span></span>

<span data-ttu-id="2375f-160">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="2375f-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2375f-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="2375f-161">Request</span></span>

<span data-ttu-id="2375f-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2375f-162">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="2375f-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="2375f-163">Response</span></span>

<span data-ttu-id="2375f-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2375f-164">The following is an example of the response.</span></span>

> <span data-ttu-id="2375f-165">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="2375f-165">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2375f-166">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="2375f-166">All the properties will be returned from an actual call.</span></span>

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
