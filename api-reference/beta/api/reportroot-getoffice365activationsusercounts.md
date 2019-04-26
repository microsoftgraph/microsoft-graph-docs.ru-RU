---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Получите число включенных пользователей, которые активировали подписку на Office на настольных компьютерах, устройствах или общих компьютерах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: dbe1fadf92e4a5ef033070bdfceaf8790fc58e8b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336734"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="0c42d-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="0c42d-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c42d-104">Получите число включенных пользователей, которые активировали подписку на Office на настольных компьютерах, устройствах или общих компьютерах.</span><span class="sxs-lookup"><span data-stu-id="0c42d-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="0c42d-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="0c42d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c42d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c42d-106">Permissions</span></span>

<span data-ttu-id="0c42d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c42d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c42d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c42d-109">Permission type</span></span>                        | <span data-ttu-id="0c42d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c42d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0c42d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c42d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c42d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c42d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0c42d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c42d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c42d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c42d-114">Not supported.</span></span>                           |
| <span data-ttu-id="0c42d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c42d-115">Application</span></span>                            | <span data-ttu-id="0c42d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c42d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0c42d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c42d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="query-parameters"></a><span data-ttu-id="0c42d-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="0c42d-118">Query parameters</span></span>

<span data-ttu-id="0c42d-119">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0c42d-119">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0c42d-120">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="0c42d-120">The default output type is text/csv.</span></span> <span data-ttu-id="0c42d-121">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="0c42d-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c42d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c42d-122">Request headers</span></span>

| <span data-ttu-id="0c42d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="0c42d-123">Name</span></span>          | <span data-ttu-id="0c42d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0c42d-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0c42d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c42d-125">Authorization</span></span> | <span data-ttu-id="0c42d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c42d-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0c42d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c42d-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0c42d-129">CSV</span><span class="sxs-lookup"><span data-stu-id="0c42d-129">CSV</span></span>

<span data-ttu-id="0c42d-130">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="0c42d-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0c42d-131">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="0c42d-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0c42d-132">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0c42d-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0c42d-133">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="0c42d-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0c42d-134">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="0c42d-134">Report Refresh Date</span></span>
- <span data-ttu-id="0c42d-135">"Product Type" (Тип продукта);</span><span class="sxs-lookup"><span data-stu-id="0c42d-135">Product Type</span></span>
- <span data-ttu-id="0c42d-136">"Assigned" (Назначенные);</span><span class="sxs-lookup"><span data-stu-id="0c42d-136">Assigned</span></span>
- <span data-ttu-id="0c42d-137">"Activated" (Активированные).</span><span class="sxs-lookup"><span data-stu-id="0c42d-137">Activated</span></span>
- <span data-ttu-id="0c42d-138">Активация на общем компьютере</span><span class="sxs-lookup"><span data-stu-id="0c42d-138">Shared Computer Activation</span></span>

### <a name="json"></a><span data-ttu-id="0c42d-139">JSON</span><span class="sxs-lookup"><span data-stu-id="0c42d-139">JSON</span></span>

<span data-ttu-id="0c42d-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c42d-140">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c42d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="0c42d-141">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0c42d-142">CSV</span><span class="sxs-lookup"><span data-stu-id="0c42d-142">CSV</span></span>

<span data-ttu-id="0c42d-143">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="0c42d-143">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0c42d-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c42d-144">Request</span></span>

<span data-ttu-id="0c42d-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c42d-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="0c42d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c42d-146">Response</span></span>

<span data-ttu-id="0c42d-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0c42d-147">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0c42d-148">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="0c42d-148">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="0c42d-149">JSON</span><span class="sxs-lookup"><span data-stu-id="0c42d-149">JSON</span></span>

<span data-ttu-id="0c42d-150">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="0c42d-150">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0c42d-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c42d-151">Request</span></span>

<span data-ttu-id="0c42d-152">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c42d-152">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="0c42d-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c42d-153">Response</span></span>

<span data-ttu-id="0c42d-154">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0c42d-154">The following example shows the response.</span></span>

> <span data-ttu-id="0c42d-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c42d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
