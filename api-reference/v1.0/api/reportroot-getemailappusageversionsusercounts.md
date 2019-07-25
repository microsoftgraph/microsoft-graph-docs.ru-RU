---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 74331d60b04c670d51ec8d1990b8ee666e5dc884
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880404"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="4a984-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="4a984-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

<span data-ttu-id="4a984-104">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="4a984-104">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="4a984-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="4a984-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a984-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a984-106">Permissions</span></span>

<span data-ttu-id="4a984-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a984-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a984-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a984-109">Permission type</span></span>                        | <span data-ttu-id="4a984-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a984-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4a984-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a984-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a984-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a984-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4a984-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a984-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a984-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a984-114">Not supported.</span></span>                           |
| <span data-ttu-id="4a984-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a984-115">Application</span></span>                            | <span data-ttu-id="4a984-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a984-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4a984-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a984-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4a984-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a984-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4a984-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4a984-119">Function parameters</span></span>

<span data-ttu-id="4a984-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4a984-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4a984-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="4a984-121">Parameter</span></span> | <span data-ttu-id="4a984-122">Тип</span><span class="sxs-lookup"><span data-stu-id="4a984-122">Type</span></span>   | <span data-ttu-id="4a984-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4a984-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4a984-124">period</span><span class="sxs-lookup"><span data-stu-id="4a984-124">period</span></span>    | <span data-ttu-id="4a984-125">string</span><span class="sxs-lookup"><span data-stu-id="4a984-125">string</span></span> | <span data-ttu-id="4a984-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4a984-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4a984-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4a984-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4a984-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4a984-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4a984-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a984-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4a984-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a984-130">Request headers</span></span>

| <span data-ttu-id="4a984-131">Имя</span><span class="sxs-lookup"><span data-stu-id="4a984-131">Name</span></span>          | <span data-ttu-id="4a984-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4a984-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4a984-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a984-133">Authorization</span></span> | <span data-ttu-id="4a984-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a984-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4a984-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4a984-136">If-None-Match</span></span> | <span data-ttu-id="4a984-137">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="4a984-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4a984-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4a984-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4a984-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a984-139">Response</span></span>

<span data-ttu-id="4a984-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4a984-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4a984-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4a984-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4a984-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4a984-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4a984-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4a984-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4a984-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4a984-144">Report Refresh Date</span></span>
- <span data-ttu-id="4a984-145">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="4a984-145">Outlook 2016</span></span>
- <span data-ttu-id="4a984-146">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="4a984-146">Outlook 2013</span></span>
- <span data-ttu-id="4a984-147">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="4a984-147">Outlook 2010</span></span>
- <span data-ttu-id="4a984-148">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="4a984-148">Outlook 2007</span></span>
- <span data-ttu-id="4a984-149">Undetermined (не определено)</span><span class="sxs-lookup"><span data-stu-id="4a984-149">Undetermined</span></span>
- <span data-ttu-id="4a984-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="4a984-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4a984-151">Пример</span><span class="sxs-lookup"><span data-stu-id="4a984-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4a984-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a984-152">Request</span></span>

<span data-ttu-id="4a984-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a984-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageversionsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageVersionsUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a984-154">C#</span><span class="sxs-lookup"><span data-stu-id="4a984-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageversionsusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a984-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="4a984-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageversionsusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a984-156">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4a984-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageversionsusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4a984-157">Java</span><span class="sxs-lookup"><span data-stu-id="4a984-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailappusageversionsusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4a984-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a984-158">Response</span></span>

<span data-ttu-id="4a984-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a984-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="4a984-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4a984-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
