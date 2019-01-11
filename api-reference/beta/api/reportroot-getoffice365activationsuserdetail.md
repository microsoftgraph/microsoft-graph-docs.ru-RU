---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Получите сведения о пользователях, которые активировали Office 365.
localization_priority: Normal
ms.openlocfilehash: 686a27f0942f89a9d173544d565c2562622c6e05
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835282"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="ef9c3-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="ef9c3-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

> <span data-ttu-id="ef9c3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef9c3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef9c3-106">Получите сведения о пользователях, которые активировали Office 365.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-106">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="ef9c3-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="ef9c3-107">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef9c3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef9c3-108">Permissions</span></span>

<span data-ttu-id="ef9c3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef9c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef9c3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef9c3-111">Permission type</span></span>                        | <span data-ttu-id="ef9c3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef9c3-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ef9c3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef9c3-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef9c3-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef9c3-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ef9c3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef9c3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef9c3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-116">Not supported.</span></span>                           |
| <span data-ttu-id="ef9c3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef9c3-117">Application</span></span>                            | <span data-ttu-id="ef9c3-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef9c3-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ef9c3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef9c3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="ef9c3-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="ef9c3-120">Query parameters</span></span>

<span data-ttu-id="ef9c3-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-121">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ef9c3-122">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-122">The default output type is text/csv.</span></span> <span data-ttu-id="ef9c3-123">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef9c3-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef9c3-124">Request headers</span></span>

| <span data-ttu-id="ef9c3-125">Имя</span><span class="sxs-lookup"><span data-stu-id="ef9c3-125">Name</span></span>          | <span data-ttu-id="ef9c3-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ef9c3-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ef9c3-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef9c3-127">Authorization</span></span> | <span data-ttu-id="ef9c3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ef9c3-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef9c3-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ef9c3-131">CSV</span><span class="sxs-lookup"><span data-stu-id="ef9c3-131">CSV</span></span>

<span data-ttu-id="ef9c3-132">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ef9c3-133">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ef9c3-134">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ef9c3-135">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ef9c3-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ef9c3-136">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ef9c3-136">Report Refresh Date</span></span>
- <span data-ttu-id="ef9c3-137">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="ef9c3-137">User Principal Name</span></span>
- <span data-ttu-id="ef9c3-138">Display Name (отображаемое имя)</span><span class="sxs-lookup"><span data-stu-id="ef9c3-138">Display Name</span></span>
- <span data-ttu-id="ef9c3-139">Product Type (тип продукта)</span><span class="sxs-lookup"><span data-stu-id="ef9c3-139">Product Type</span></span>
- <span data-ttu-id="ef9c3-140">Last Activated Date (дата последней активации)</span><span class="sxs-lookup"><span data-stu-id="ef9c3-140">Last Activated Date</span></span>
- <span data-ttu-id="ef9c3-141">Windows</span><span class="sxs-lookup"><span data-stu-id="ef9c3-141">Windows</span></span>
- <span data-ttu-id="ef9c3-142">Mac</span><span class="sxs-lookup"><span data-stu-id="ef9c3-142">Mac</span></span>
- <span data-ttu-id="ef9c3-143">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="ef9c3-143">Windows 10 Mobile</span></span>
- <span data-ttu-id="ef9c3-144">iOS</span><span class="sxs-lookup"><span data-stu-id="ef9c3-144">iOS</span></span>
- <span data-ttu-id="ef9c3-145">Android</span><span class="sxs-lookup"><span data-stu-id="ef9c3-145">Android</span></span>
- <span data-ttu-id="ef9c3-146">Активированные на совместно используемый компьютер</span><span class="sxs-lookup"><span data-stu-id="ef9c3-146">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="ef9c3-147">JSON</span><span class="sxs-lookup"><span data-stu-id="ef9c3-147">JSON</span></span>

<span data-ttu-id="ef9c3-148">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-148">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="ef9c3-149">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-149">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="ef9c3-150">Пример</span><span class="sxs-lookup"><span data-stu-id="ef9c3-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ef9c3-151">CSV</span><span class="sxs-lookup"><span data-stu-id="ef9c3-151">CSV</span></span>

<span data-ttu-id="ef9c3-152">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ef9c3-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef9c3-153">Request</span></span>

<span data-ttu-id="ef9c3-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="ef9c3-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef9c3-155">Response</span></span>

<span data-ttu-id="ef9c3-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-156">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ef9c3-157">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="ef9c3-158">JSON</span><span class="sxs-lookup"><span data-stu-id="ef9c3-158">JSON</span></span>

<span data-ttu-id="ef9c3-159">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-159">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ef9c3-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef9c3-160">Request</span></span>

<span data-ttu-id="ef9c3-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="ef9c3-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef9c3-162">Response</span></span>

<span data-ttu-id="ef9c3-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-163">The following is an example of the response.</span></span>

> <span data-ttu-id="ef9c3-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef9c3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
