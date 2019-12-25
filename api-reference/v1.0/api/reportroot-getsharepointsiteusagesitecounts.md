---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e09cc1881b786b7cfdfff6057d1aff8663b8a1e4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865330"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="203cd-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="203cd-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="203cd-105">Узнайте, сколько всего файлов на всех сайтах и сколько из них активны.</span><span class="sxs-lookup"><span data-stu-id="203cd-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="203cd-106">Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="203cd-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="203cd-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="203cd-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="203cd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="203cd-108">Permissions</span></span>

<span data-ttu-id="203cd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="203cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="203cd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="203cd-111">Permission type</span></span>                        | <span data-ttu-id="203cd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="203cd-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="203cd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="203cd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="203cd-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="203cd-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="203cd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="203cd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="203cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="203cd-116">Not supported.</span></span>                           |
| <span data-ttu-id="203cd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="203cd-117">Application</span></span>                            | <span data-ttu-id="203cd-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="203cd-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="203cd-119">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="203cd-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="203cd-120">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="203cd-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="203cd-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="203cd-121">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="203cd-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="203cd-122">Function parameters</span></span>

<span data-ttu-id="203cd-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="203cd-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="203cd-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="203cd-124">Parameter</span></span> | <span data-ttu-id="203cd-125">Тип</span><span class="sxs-lookup"><span data-stu-id="203cd-125">Type</span></span>   | <span data-ttu-id="203cd-126">Описание</span><span class="sxs-lookup"><span data-stu-id="203cd-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="203cd-127">period</span><span class="sxs-lookup"><span data-stu-id="203cd-127">period</span></span>    | <span data-ttu-id="203cd-128">string</span><span class="sxs-lookup"><span data-stu-id="203cd-128">string</span></span> | <span data-ttu-id="203cd-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="203cd-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="203cd-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="203cd-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="203cd-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="203cd-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="203cd-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="203cd-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="203cd-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="203cd-133">Request headers</span></span>

| <span data-ttu-id="203cd-134">Имя</span><span class="sxs-lookup"><span data-stu-id="203cd-134">Name</span></span>          | <span data-ttu-id="203cd-135">Описание</span><span class="sxs-lookup"><span data-stu-id="203cd-135">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="203cd-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="203cd-136">Authorization</span></span> | <span data-ttu-id="203cd-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="203cd-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="203cd-139">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="203cd-139">If-None-Match</span></span> | <span data-ttu-id="203cd-140">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="203cd-140">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="203cd-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="203cd-141">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="203cd-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="203cd-142">Response</span></span>

<span data-ttu-id="203cd-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="203cd-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="203cd-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="203cd-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="203cd-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="203cd-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="203cd-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="203cd-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="203cd-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="203cd-147">Report Refresh Date</span></span>
- <span data-ttu-id="203cd-148">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="203cd-148">Site Type</span></span>
- <span data-ttu-id="203cd-149">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="203cd-149">Total</span></span>
- <span data-ttu-id="203cd-150">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="203cd-150">Active</span></span>
- <span data-ttu-id="203cd-151">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="203cd-151">Report Date</span></span>
- <span data-ttu-id="203cd-152">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="203cd-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="203cd-153">Пример</span><span class="sxs-lookup"><span data-stu-id="203cd-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="203cd-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="203cd-154">Request</span></span>

<span data-ttu-id="203cd-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="203cd-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="203cd-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="203cd-156">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="203cd-157">C#</span><span class="sxs-lookup"><span data-stu-id="203cd-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagesitecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="203cd-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="203cd-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagesitecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="203cd-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="203cd-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagesitecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="203cd-160">Java</span><span class="sxs-lookup"><span data-stu-id="203cd-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagesitecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="203cd-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="203cd-161">Response</span></span>

<span data-ttu-id="203cd-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="203cd-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="203cd-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="203cd-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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
