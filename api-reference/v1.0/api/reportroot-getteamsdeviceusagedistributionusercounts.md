---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 6cf2014dd422dcbedfeb509b008122d84b56a844
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510083"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="95adf-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="95adf-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="95adf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95adf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95adf-105">Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="95adf-105">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="95adf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95adf-106">Permissions</span></span>

<span data-ttu-id="95adf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95adf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95adf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95adf-109">Permission type</span></span>                        | <span data-ttu-id="95adf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95adf-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="95adf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95adf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="95adf-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="95adf-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="95adf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95adf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95adf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95adf-114">Not supported.</span></span>                           |
| <span data-ttu-id="95adf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95adf-115">Application</span></span>                            | <span data-ttu-id="95adf-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="95adf-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="95adf-117">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="95adf-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="95adf-118">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="95adf-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="95adf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95adf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="95adf-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="95adf-120">Function parameters</span></span>

<span data-ttu-id="95adf-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="95adf-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="95adf-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="95adf-122">Parameter</span></span> | <span data-ttu-id="95adf-123">Тип</span><span class="sxs-lookup"><span data-stu-id="95adf-123">Type</span></span>   | <span data-ttu-id="95adf-124">Описание</span><span class="sxs-lookup"><span data-stu-id="95adf-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="95adf-125">period</span><span class="sxs-lookup"><span data-stu-id="95adf-125">period</span></span>    | <span data-ttu-id="95adf-126">string</span><span class="sxs-lookup"><span data-stu-id="95adf-126">string</span></span> | <span data-ttu-id="95adf-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="95adf-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="95adf-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="95adf-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="95adf-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="95adf-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="95adf-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95adf-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="95adf-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95adf-131">Request headers</span></span>

| <span data-ttu-id="95adf-132">Имя</span><span class="sxs-lookup"><span data-stu-id="95adf-132">Name</span></span>          | <span data-ttu-id="95adf-133">Описание</span><span class="sxs-lookup"><span data-stu-id="95adf-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="95adf-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95adf-134">Authorization</span></span> | <span data-ttu-id="95adf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95adf-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="95adf-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="95adf-137">Response</span></span>

<span data-ttu-id="95adf-138">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="95adf-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="95adf-139">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="95adf-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="95adf-140">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="95adf-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="95adf-141">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="95adf-141">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="95adf-142">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="95adf-142">Report Refresh Date</span></span>
- <span data-ttu-id="95adf-143">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="95adf-143">Web</span></span>
- <span data-ttu-id="95adf-144">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="95adf-144">Windows Phone</span></span>
- <span data-ttu-id="95adf-145">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="95adf-145">Android Phone</span></span>
- <span data-ttu-id="95adf-146">"iOS";</span><span class="sxs-lookup"><span data-stu-id="95adf-146">iOS</span></span>
- <span data-ttu-id="95adf-147">"Mac";</span><span class="sxs-lookup"><span data-stu-id="95adf-147">Mac</span></span>
- <span data-ttu-id="95adf-148">"Windows";</span><span class="sxs-lookup"><span data-stu-id="95adf-148">Windows</span></span>
- <span data-ttu-id="95adf-149">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="95adf-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="95adf-150">Пример</span><span class="sxs-lookup"><span data-stu-id="95adf-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="95adf-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="95adf-151">Request</span></span>

<span data-ttu-id="95adf-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95adf-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="95adf-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="95adf-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="95adf-154">C#</span><span class="sxs-lookup"><span data-stu-id="95adf-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95adf-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95adf-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95adf-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95adf-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95adf-157">Java</span><span class="sxs-lookup"><span data-stu-id="95adf-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusagedistributionusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="95adf-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="95adf-158">Response</span></span>

<span data-ttu-id="95adf-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="95adf-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="95adf-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="95adf-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
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
