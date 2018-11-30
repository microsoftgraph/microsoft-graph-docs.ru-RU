---
title: 'reportRoot: getOffice365ActivationCounts'
description: Получите количество активаций Office 365 на компьютерах и мобильных устройствах.
ms.openlocfilehash: c75b957f02eb5d5fa77f5e3dfa696f3086f9d817
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076408"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="3e447-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="3e447-103">reportRoot: getOffice365ActivationCounts</span></span>

> <span data-ttu-id="3e447-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3e447-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e447-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e447-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e447-106">Получите количество активаций Office 365 на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="3e447-106">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="3e447-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="3e447-107">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e447-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e447-108">Permissions</span></span>

<span data-ttu-id="3e447-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e447-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e447-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e447-111">Permission type</span></span>                        | <span data-ttu-id="3e447-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e447-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3e447-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e447-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e447-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e447-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3e447-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e447-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e447-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e447-116">Not supported.</span></span>                           |
| <span data-ttu-id="3e447-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e447-117">Application</span></span>                            | <span data-ttu-id="3e447-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e447-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3e447-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e447-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="3e447-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="3e447-120">Query parameters</span></span>

<span data-ttu-id="3e447-121">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3e447-121">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3e447-122">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="3e447-122">The default output type is text/csv.</span></span> <span data-ttu-id="3e447-123">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="3e447-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e447-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e447-124">Request headers</span></span>

| <span data-ttu-id="3e447-125">Имя</span><span class="sxs-lookup"><span data-stu-id="3e447-125">Name</span></span>          | <span data-ttu-id="3e447-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3e447-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3e447-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e447-127">Authorization</span></span> | <span data-ttu-id="3e447-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e447-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3e447-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e447-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3e447-131">CSV</span><span class="sxs-lookup"><span data-stu-id="3e447-131">CSV</span></span>

<span data-ttu-id="3e447-132">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3e447-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3e447-133">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3e447-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3e447-134">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3e447-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3e447-135">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3e447-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3e447-136">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3e447-136">Report Refresh Date</span></span>
- <span data-ttu-id="3e447-137">Product Type (Тип продукта)</span><span class="sxs-lookup"><span data-stu-id="3e447-137">Product Type</span></span>
- <span data-ttu-id="3e447-138">Windows</span><span class="sxs-lookup"><span data-stu-id="3e447-138">Windows</span></span>
- <span data-ttu-id="3e447-139">Mac</span><span class="sxs-lookup"><span data-stu-id="3e447-139">Mac</span></span>
- <span data-ttu-id="3e447-140">Android</span><span class="sxs-lookup"><span data-stu-id="3e447-140">Android</span></span>
- <span data-ttu-id="3e447-141">iOS</span><span class="sxs-lookup"><span data-stu-id="3e447-141">iOS</span></span>
- <span data-ttu-id="3e447-142">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="3e447-142">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="3e447-143">JSON</span><span class="sxs-lookup"><span data-stu-id="3e447-143">JSON</span></span>

<span data-ttu-id="3e447-144">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[office365ActivationCounts](../resources/office365activationcounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3e447-144">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e447-145">Пример</span><span class="sxs-lookup"><span data-stu-id="3e447-145">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3e447-146">CSV</span><span class="sxs-lookup"><span data-stu-id="3e447-146">CSV</span></span>

<span data-ttu-id="3e447-147">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="3e447-147">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3e447-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e447-148">Request</span></span>

<span data-ttu-id="3e447-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e447-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="3e447-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e447-150">Response</span></span>

<span data-ttu-id="3e447-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3e447-151">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3e447-152">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3e447-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="3e447-153">JSON</span><span class="sxs-lookup"><span data-stu-id="3e447-153">JSON</span></span>

<span data-ttu-id="3e447-154">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="3e447-154">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3e447-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e447-155">Request</span></span>

<span data-ttu-id="3e447-156">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e447-156">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="3e447-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e447-157">Response</span></span>

<span data-ttu-id="3e447-158">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3e447-158">The following example shows the response.</span></span>

> <span data-ttu-id="3e447-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e447-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
