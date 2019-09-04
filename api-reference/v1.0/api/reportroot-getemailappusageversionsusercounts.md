---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 1fb9b283d0788b0d6a92cef70b0ccf725c8b0d10
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728253"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="6abf7-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="6abf7-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

<span data-ttu-id="6abf7-104">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="6abf7-104">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="6abf7-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="6abf7-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="6abf7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6abf7-106">Permissions</span></span>

<span data-ttu-id="6abf7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6abf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6abf7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6abf7-109">Permission type</span></span>                        | <span data-ttu-id="6abf7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6abf7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6abf7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6abf7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6abf7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6abf7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6abf7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6abf7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6abf7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6abf7-114">Not supported.</span></span>                           |
| <span data-ttu-id="6abf7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6abf7-115">Application</span></span>                            | <span data-ttu-id="6abf7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6abf7-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6abf7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6abf7-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6abf7-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6abf7-118">Function parameters</span></span>

<span data-ttu-id="6abf7-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="6abf7-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6abf7-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="6abf7-120">Parameter</span></span> | <span data-ttu-id="6abf7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6abf7-121">Type</span></span>   | <span data-ttu-id="6abf7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6abf7-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6abf7-123">period</span><span class="sxs-lookup"><span data-stu-id="6abf7-123">period</span></span>    | <span data-ttu-id="6abf7-124">string</span><span class="sxs-lookup"><span data-stu-id="6abf7-124">string</span></span> | <span data-ttu-id="6abf7-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="6abf7-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6abf7-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="6abf7-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6abf7-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="6abf7-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6abf7-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6abf7-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6abf7-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6abf7-129">Request headers</span></span>

| <span data-ttu-id="6abf7-130">Имя</span><span class="sxs-lookup"><span data-stu-id="6abf7-130">Name</span></span>          | <span data-ttu-id="6abf7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6abf7-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6abf7-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6abf7-132">Authorization</span></span> | <span data-ttu-id="6abf7-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6abf7-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6abf7-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6abf7-135">If-None-Match</span></span> | <span data-ttu-id="6abf7-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="6abf7-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6abf7-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6abf7-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6abf7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6abf7-138">Response</span></span>

<span data-ttu-id="6abf7-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6abf7-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6abf7-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6abf7-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6abf7-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6abf7-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6abf7-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6abf7-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6abf7-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="6abf7-143">Report Refresh Date</span></span>
- <span data-ttu-id="6abf7-144">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="6abf7-144">Outlook 2016</span></span>
- <span data-ttu-id="6abf7-145">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="6abf7-145">Outlook 2013</span></span>
- <span data-ttu-id="6abf7-146">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="6abf7-146">Outlook 2010</span></span>
- <span data-ttu-id="6abf7-147">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="6abf7-147">Outlook 2007</span></span>
- <span data-ttu-id="6abf7-148">Undetermined (не определено)</span><span class="sxs-lookup"><span data-stu-id="6abf7-148">Undetermined</span></span>
- <span data-ttu-id="6abf7-149">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="6abf7-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="6abf7-150">Пример</span><span class="sxs-lookup"><span data-stu-id="6abf7-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6abf7-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="6abf7-151">Request</span></span>

<span data-ttu-id="6abf7-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6abf7-152">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6abf7-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="6abf7-153">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageversionsusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageVersionsUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6abf7-154">C#</span><span class="sxs-lookup"><span data-stu-id="6abf7-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageversionsusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6abf7-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6abf7-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageversionsusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6abf7-156">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6abf7-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageversionsusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6abf7-157">Java</span><span class="sxs-lookup"><span data-stu-id="6abf7-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailappusageversionsusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6abf7-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="6abf7-158">Response</span></span>

<span data-ttu-id="6abf7-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6abf7-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="6abf7-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6abf7-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period
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
