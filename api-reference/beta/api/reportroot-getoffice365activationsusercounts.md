---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Получение числа пользователей, для которых включено и те, которые активации подписки Office на настольных ПК или устройства или на общедоступном компьютере.
ms.openlocfilehash: 4d7d75d084408e4d0d8af0473397252fdcbe7aa9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074609"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="32cdb-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="32cdb-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

> <span data-ttu-id="32cdb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="32cdb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32cdb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32cdb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32cdb-106">Получение числа пользователей, для которых включено и те, которые активации подписки Office на настольных ПК или устройства или на общедоступном компьютере.</span><span class="sxs-lookup"><span data-stu-id="32cdb-106">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="32cdb-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="32cdb-107">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="32cdb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32cdb-108">Permissions</span></span>

<span data-ttu-id="32cdb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32cdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32cdb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32cdb-111">Permission type</span></span>                        | <span data-ttu-id="32cdb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32cdb-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="32cdb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32cdb-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="32cdb-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="32cdb-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="32cdb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32cdb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32cdb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32cdb-116">Not supported.</span></span>                           |
| <span data-ttu-id="32cdb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32cdb-117">Application</span></span>                            | <span data-ttu-id="32cdb-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="32cdb-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="32cdb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32cdb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="query-parameters"></a><span data-ttu-id="32cdb-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="32cdb-120">Query parameters</span></span>

<span data-ttu-id="32cdb-121">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="32cdb-121">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="32cdb-122">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="32cdb-122">The default output type is text/csv.</span></span> <span data-ttu-id="32cdb-123">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="32cdb-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32cdb-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32cdb-124">Request headers</span></span>

| <span data-ttu-id="32cdb-125">Имя</span><span class="sxs-lookup"><span data-stu-id="32cdb-125">Name</span></span>          | <span data-ttu-id="32cdb-126">Описание</span><span class="sxs-lookup"><span data-stu-id="32cdb-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="32cdb-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32cdb-127">Authorization</span></span> | <span data-ttu-id="32cdb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32cdb-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="32cdb-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="32cdb-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="32cdb-131">CSV</span><span class="sxs-lookup"><span data-stu-id="32cdb-131">CSV</span></span>

<span data-ttu-id="32cdb-132">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="32cdb-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="32cdb-133">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="32cdb-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="32cdb-134">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="32cdb-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="32cdb-135">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="32cdb-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="32cdb-136">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="32cdb-136">Report Refresh Date</span></span>
- <span data-ttu-id="32cdb-137">"Product Type" (Тип продукта);</span><span class="sxs-lookup"><span data-stu-id="32cdb-137">Product Type</span></span>
- <span data-ttu-id="32cdb-138">"Assigned" (Назначенные);</span><span class="sxs-lookup"><span data-stu-id="32cdb-138">Assigned</span></span>
- <span data-ttu-id="32cdb-139">"Activated" (Активированные).</span><span class="sxs-lookup"><span data-stu-id="32cdb-139">Activated</span></span>
- <span data-ttu-id="32cdb-140">Активация совместно используемый компьютер</span><span class="sxs-lookup"><span data-stu-id="32cdb-140">Shared Computer Activation</span></span>

### <a name="json"></a><span data-ttu-id="32cdb-141">JSON</span><span class="sxs-lookup"><span data-stu-id="32cdb-141">JSON</span></span>

<span data-ttu-id="32cdb-142">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="32cdb-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32cdb-143">Пример</span><span class="sxs-lookup"><span data-stu-id="32cdb-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="32cdb-144">CSV</span><span class="sxs-lookup"><span data-stu-id="32cdb-144">CSV</span></span>

<span data-ttu-id="32cdb-145">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="32cdb-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="32cdb-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="32cdb-146">Request</span></span>

<span data-ttu-id="32cdb-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32cdb-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="32cdb-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="32cdb-148">Response</span></span>

<span data-ttu-id="32cdb-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="32cdb-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="32cdb-150">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="32cdb-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="32cdb-151">JSON</span><span class="sxs-lookup"><span data-stu-id="32cdb-151">JSON</span></span>

<span data-ttu-id="32cdb-152">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="32cdb-152">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="32cdb-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="32cdb-153">Request</span></span>

<span data-ttu-id="32cdb-154">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32cdb-154">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="32cdb-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="32cdb-155">Response</span></span>

<span data-ttu-id="32cdb-156">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="32cdb-156">The following example shows the response.</span></span>

> <span data-ttu-id="32cdb-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32cdb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
