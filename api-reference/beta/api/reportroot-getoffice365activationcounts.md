---
title: 'reportRoot: getOffice365ActivationCounts'
description: Получите количество активаций Microsoft 365 на настольных компьютерах и устройствах.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 21444eddb72e12f52d1ab462e649be87436ff0ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049802"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="210ad-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="210ad-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="210ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="210ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="210ad-105">Получите количество активаций Microsoft 365 на настольных компьютерах и устройствах.</span><span class="sxs-lookup"><span data-stu-id="210ad-105">Get the count of Microsoft 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="210ad-106">**Примечание:** Сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов — Microsoft Office активаций.](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)</span><span class="sxs-lookup"><span data-stu-id="210ad-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="210ad-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="210ad-107">Permissions</span></span>

<span data-ttu-id="210ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="210ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="210ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="210ad-110">Permission type</span></span>                        | <span data-ttu-id="210ad-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="210ad-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="210ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="210ad-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="210ad-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="210ad-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="210ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="210ad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="210ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="210ad-115">Not supported.</span></span>                           |
| <span data-ttu-id="210ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="210ad-116">Application</span></span>                            | <span data-ttu-id="210ad-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="210ad-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="210ad-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="210ad-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="210ad-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="210ad-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="210ad-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="210ad-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="210ad-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="210ad-121">Query parameters</span></span>

<span data-ttu-id="210ad-122">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="210ad-122">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="210ad-123">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="210ad-123">The default output type is text/csv.</span></span> <span data-ttu-id="210ad-124">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="210ad-124">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="210ad-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="210ad-125">Request headers</span></span>

| <span data-ttu-id="210ad-126">Имя</span><span class="sxs-lookup"><span data-stu-id="210ad-126">Name</span></span>          | <span data-ttu-id="210ad-127">Описание</span><span class="sxs-lookup"><span data-stu-id="210ad-127">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="210ad-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="210ad-128">Authorization</span></span> | <span data-ttu-id="210ad-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="210ad-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="210ad-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="210ad-131">Response</span></span>

### <a name="csv"></a><span data-ttu-id="210ad-132">CSV</span><span class="sxs-lookup"><span data-stu-id="210ad-132">CSV</span></span>

<span data-ttu-id="210ad-133">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="210ad-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="210ad-134">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="210ad-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="210ad-135">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="210ad-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="210ad-136">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="210ad-136">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="210ad-137">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="210ad-137">Report Refresh Date</span></span>
- <span data-ttu-id="210ad-138">Product Type (Тип продукта)</span><span class="sxs-lookup"><span data-stu-id="210ad-138">Product Type</span></span>
- <span data-ttu-id="210ad-139">Windows</span><span class="sxs-lookup"><span data-stu-id="210ad-139">Windows</span></span>
- <span data-ttu-id="210ad-140">Mac</span><span class="sxs-lookup"><span data-stu-id="210ad-140">Mac</span></span>
- <span data-ttu-id="210ad-141">Android</span><span class="sxs-lookup"><span data-stu-id="210ad-141">Android</span></span>
- <span data-ttu-id="210ad-142">iOS</span><span class="sxs-lookup"><span data-stu-id="210ad-142">iOS</span></span>
- <span data-ttu-id="210ad-143">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="210ad-143">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="210ad-144">JSON</span><span class="sxs-lookup"><span data-stu-id="210ad-144">JSON</span></span>

<span data-ttu-id="210ad-145">В случае успешной работы этот метод возвращает код отклика и `200 OK` **[объект Office365ActivationCounts](../resources/office365activationcounts.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="210ad-145">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="210ad-146">Пример</span><span class="sxs-lookup"><span data-stu-id="210ad-146">Example</span></span>

### <a name="csv"></a><span data-ttu-id="210ad-147">CSV</span><span class="sxs-lookup"><span data-stu-id="210ad-147">CSV</span></span>

<span data-ttu-id="210ad-148">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="210ad-148">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="210ad-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="210ad-149">Request</span></span>

<span data-ttu-id="210ad-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="210ad-150">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="210ad-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="210ad-151">Response</span></span>

<span data-ttu-id="210ad-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="210ad-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="210ad-153">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="210ad-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="210ad-154">JSON</span><span class="sxs-lookup"><span data-stu-id="210ad-154">JSON</span></span>

<span data-ttu-id="210ad-155">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="210ad-155">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="210ad-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="210ad-156">Request</span></span>

<span data-ttu-id="210ad-157">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="210ad-157">The following example shows the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="210ad-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="210ad-158">Response</span></span>

<span data-ttu-id="210ad-159">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="210ad-159">The following example shows the response.</span></span>

> <span data-ttu-id="210ad-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="210ad-160">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "productType": "Microsoft 365 Apps for enterprise", 
      "windows": 9157, 
      "mac": 576, 
      "android": 358, 
      "ios": 1452, 
      "windows10Mobile": 2309
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


