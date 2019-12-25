---
title: 'reportRoot: getYammerDeviceUsageDistributionUserCounts'
description: Получите сведения о количестве пользователей с разбивкой по типам устройств.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 89d267e7a17f97256a3ca45e63415d5f8b26f7fb
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865211"
---
# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="ce013-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="ce013-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="ce013-104">Получите сведения о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="ce013-104">Get the number of users by device type.</span></span>

> <span data-ttu-id="ce013-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="ce013-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce013-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce013-106">Permissions</span></span>

<span data-ttu-id="ce013-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce013-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce013-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce013-109">Permission type</span></span>                        | <span data-ttu-id="ce013-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce013-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ce013-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce013-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce013-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce013-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ce013-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce013-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce013-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce013-114">Not supported.</span></span>                           |
| <span data-ttu-id="ce013-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce013-115">Application</span></span>                            | <span data-ttu-id="ce013-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce013-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="ce013-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ce013-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ce013-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ce013-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ce013-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce013-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ce013-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ce013-120">Function parameters</span></span>

<span data-ttu-id="ce013-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ce013-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ce013-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="ce013-122">Parameter</span></span> | <span data-ttu-id="ce013-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ce013-123">Type</span></span>   | <span data-ttu-id="ce013-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ce013-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ce013-125">period</span><span class="sxs-lookup"><span data-stu-id="ce013-125">period</span></span>    | <span data-ttu-id="ce013-126">string</span><span class="sxs-lookup"><span data-stu-id="ce013-126">string</span></span> | <span data-ttu-id="ce013-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ce013-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ce013-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ce013-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ce013-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ce013-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ce013-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce013-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ce013-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce013-131">Request headers</span></span>

| <span data-ttu-id="ce013-132">Имя</span><span class="sxs-lookup"><span data-stu-id="ce013-132">Name</span></span>          | <span data-ttu-id="ce013-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ce013-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ce013-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce013-134">Authorization</span></span> | <span data-ttu-id="ce013-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce013-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ce013-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ce013-137">If-None-Match</span></span> | <span data-ttu-id="ce013-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="ce013-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ce013-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ce013-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ce013-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce013-140">Response</span></span>

<span data-ttu-id="ce013-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ce013-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ce013-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ce013-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ce013-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ce013-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ce013-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ce013-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ce013-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ce013-145">Report Refresh Date</span></span>
- <span data-ttu-id="ce013-146">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="ce013-146">Web</span></span>
- <span data-ttu-id="ce013-147">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="ce013-147">Windows Phone</span></span>
- <span data-ttu-id="ce013-148">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="ce013-148">Android Phone</span></span>
- <span data-ttu-id="ce013-149">iPhone</span><span class="sxs-lookup"><span data-stu-id="ce013-149">iPhone</span></span>
- <span data-ttu-id="ce013-150">iPad</span><span class="sxs-lookup"><span data-stu-id="ce013-150">iPad</span></span>
- <span data-ttu-id="ce013-151">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="ce013-151">Other</span></span>
- <span data-ttu-id="ce013-152">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="ce013-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ce013-153">Пример</span><span class="sxs-lookup"><span data-stu-id="ce013-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ce013-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce013-154">Request</span></span>

<span data-ttu-id="ce013-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce013-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ce013-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce013-156">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusagedistributionusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ce013-157">C#</span><span class="sxs-lookup"><span data-stu-id="ce013-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusagedistributionusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce013-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce013-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusagedistributionusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ce013-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce013-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusagedistributionusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ce013-160">Java</span><span class="sxs-lookup"><span data-stu-id="ce013-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammerdeviceusagedistributionusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ce013-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce013-161">Response</span></span>

<span data-ttu-id="ce013-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ce013-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="ce013-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ce013-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Period
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
