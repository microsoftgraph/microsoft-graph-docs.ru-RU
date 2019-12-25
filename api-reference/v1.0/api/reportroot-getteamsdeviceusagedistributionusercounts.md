---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a12e88a2011a98539b442b3321fb0c99b80b6726
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865258"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="ddacd-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="ddacd-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="ddacd-104">Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="ddacd-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddacd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ddacd-105">Permissions</span></span>

<span data-ttu-id="ddacd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddacd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddacd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddacd-108">Permission type</span></span>                        | <span data-ttu-id="ddacd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddacd-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ddacd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddacd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ddacd-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddacd-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ddacd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddacd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddacd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddacd-113">Not supported.</span></span>                           |
| <span data-ttu-id="ddacd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddacd-114">Application</span></span>                            | <span data-ttu-id="ddacd-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddacd-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="ddacd-116">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ddacd-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ddacd-117">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ddacd-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ddacd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddacd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ddacd-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ddacd-119">Function parameters</span></span>

<span data-ttu-id="ddacd-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ddacd-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ddacd-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="ddacd-121">Parameter</span></span> | <span data-ttu-id="ddacd-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ddacd-122">Type</span></span>   | <span data-ttu-id="ddacd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ddacd-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ddacd-124">period</span><span class="sxs-lookup"><span data-stu-id="ddacd-124">period</span></span>    | <span data-ttu-id="ddacd-125">string</span><span class="sxs-lookup"><span data-stu-id="ddacd-125">string</span></span> | <span data-ttu-id="ddacd-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ddacd-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ddacd-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ddacd-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ddacd-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ddacd-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ddacd-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddacd-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ddacd-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddacd-130">Request headers</span></span>

| <span data-ttu-id="ddacd-131">Имя</span><span class="sxs-lookup"><span data-stu-id="ddacd-131">Name</span></span>          | <span data-ttu-id="ddacd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ddacd-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ddacd-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddacd-133">Authorization</span></span> | <span data-ttu-id="ddacd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddacd-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ddacd-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddacd-136">Response</span></span>

<span data-ttu-id="ddacd-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ddacd-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ddacd-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ddacd-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ddacd-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ddacd-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ddacd-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ddacd-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="ddacd-141">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ddacd-141">Report Refresh Date</span></span>
- <span data-ttu-id="ddacd-142">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="ddacd-142">Web</span></span>
- <span data-ttu-id="ddacd-143">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="ddacd-143">Windows Phone</span></span>
- <span data-ttu-id="ddacd-144">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="ddacd-144">Android Phone</span></span>
- <span data-ttu-id="ddacd-145">"iOS";</span><span class="sxs-lookup"><span data-stu-id="ddacd-145">iOS</span></span>
- <span data-ttu-id="ddacd-146">"Mac";</span><span class="sxs-lookup"><span data-stu-id="ddacd-146">Mac</span></span>
- <span data-ttu-id="ddacd-147">"Windows";</span><span class="sxs-lookup"><span data-stu-id="ddacd-147">Windows</span></span>
- <span data-ttu-id="ddacd-148">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="ddacd-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ddacd-149">Пример</span><span class="sxs-lookup"><span data-stu-id="ddacd-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ddacd-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddacd-150">Request</span></span>

<span data-ttu-id="ddacd-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddacd-151">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ddacd-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddacd-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ddacd-153">C#</span><span class="sxs-lookup"><span data-stu-id="ddacd-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ddacd-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddacd-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ddacd-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddacd-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ddacd-156">Java</span><span class="sxs-lookup"><span data-stu-id="ddacd-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusagedistributionusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddacd-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="ddacd-157">Response</span></span>

<span data-ttu-id="ddacd-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ddacd-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="ddacd-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ddacd-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
