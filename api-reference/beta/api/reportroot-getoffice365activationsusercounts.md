---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Получите количество пользователей, включенных, и пользователей, активировав подписку Office на настольных компьютерах или общих компьютерах.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: f8ec6ccaf9421994fad1585dd243ab7d6ba599c9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049795"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="4a63c-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="4a63c-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="4a63c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a63c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a63c-105">Получите количество пользователей, включенных, и пользователей, активировав подписку Office на настольных компьютерах или общих компьютерах.</span><span class="sxs-lookup"><span data-stu-id="4a63c-105">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="4a63c-106">**Примечание:** Сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов — Microsoft Office активаций.](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)</span><span class="sxs-lookup"><span data-stu-id="4a63c-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a63c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a63c-107">Permissions</span></span>

<span data-ttu-id="4a63c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a63c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a63c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a63c-110">Permission type</span></span>                        | <span data-ttu-id="4a63c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a63c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4a63c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a63c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a63c-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a63c-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4a63c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a63c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a63c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a63c-115">Not supported.</span></span>                           |
| <span data-ttu-id="4a63c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a63c-116">Application</span></span>                            | <span data-ttu-id="4a63c-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a63c-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="4a63c-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4a63c-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="4a63c-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="4a63c-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="4a63c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a63c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="query-parameters"></a><span data-ttu-id="4a63c-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="4a63c-121">Query parameters</span></span>

<span data-ttu-id="4a63c-122">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4a63c-122">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4a63c-123">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="4a63c-123">The default output type is text/csv.</span></span> <span data-ttu-id="4a63c-124">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="4a63c-124">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a63c-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a63c-125">Request headers</span></span>

| <span data-ttu-id="4a63c-126">Имя</span><span class="sxs-lookup"><span data-stu-id="4a63c-126">Name</span></span>          | <span data-ttu-id="4a63c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4a63c-127">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4a63c-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a63c-128">Authorization</span></span> | <span data-ttu-id="4a63c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a63c-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4a63c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a63c-131">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4a63c-132">CSV</span><span class="sxs-lookup"><span data-stu-id="4a63c-132">CSV</span></span>

<span data-ttu-id="4a63c-133">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4a63c-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4a63c-134">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4a63c-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4a63c-135">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4a63c-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4a63c-136">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4a63c-136">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4a63c-137">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4a63c-137">Report Refresh Date</span></span>
- <span data-ttu-id="4a63c-138">"Product Type" (Тип продукта);</span><span class="sxs-lookup"><span data-stu-id="4a63c-138">Product Type</span></span>
- <span data-ttu-id="4a63c-139">"Assigned" (Назначенные);</span><span class="sxs-lookup"><span data-stu-id="4a63c-139">Assigned</span></span>
- <span data-ttu-id="4a63c-140">"Activated" (Активированные).</span><span class="sxs-lookup"><span data-stu-id="4a63c-140">Activated</span></span>
- <span data-ttu-id="4a63c-141">Активация общего компьютера</span><span class="sxs-lookup"><span data-stu-id="4a63c-141">Shared Computer Activation</span></span>

### <a name="json"></a><span data-ttu-id="4a63c-142">JSON</span><span class="sxs-lookup"><span data-stu-id="4a63c-142">JSON</span></span>

<span data-ttu-id="4a63c-143">В случае успешной работы этот метод возвращает код отклика и `200 OK` **[объект Office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4a63c-143">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a63c-144">Пример</span><span class="sxs-lookup"><span data-stu-id="4a63c-144">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4a63c-145">CSV</span><span class="sxs-lookup"><span data-stu-id="4a63c-145">CSV</span></span>

<span data-ttu-id="4a63c-146">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="4a63c-146">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4a63c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a63c-147">Request</span></span>

<span data-ttu-id="4a63c-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a63c-148">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationsusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="4a63c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a63c-149">Response</span></span>

<span data-ttu-id="4a63c-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a63c-150">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4a63c-151">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4a63c-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="4a63c-152">JSON</span><span class="sxs-lookup"><span data-stu-id="4a63c-152">JSON</span></span>

<span data-ttu-id="4a63c-153">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="4a63c-153">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4a63c-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a63c-154">Request</span></span>

<span data-ttu-id="4a63c-155">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a63c-155">The following example shows the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationsusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="4a63c-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a63c-156">Response</span></span>

<span data-ttu-id="4a63c-157">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a63c-157">The following example shows the response.</span></span>

> <span data-ttu-id="4a63c-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4a63c-158">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "productType": "Microsoft 365 Apps for enterprise", 
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


