---
title: 'reportRoot: getSharePointActivityPages'
description: Узнайте, сколько уникальных страниц посетили пользователи.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 19830e4efb221e2951d093ea097ad3073c7a9f23
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728092"
---
# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="c1594-103">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="c1594-103">reportRoot: getSharePointActivityPages</span></span>

<span data-ttu-id="c1594-104">Узнайте, сколько уникальных страниц посетили пользователи.</span><span class="sxs-lookup"><span data-stu-id="c1594-104">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="c1594-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="c1594-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1594-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1594-106">Permissions</span></span>

<span data-ttu-id="c1594-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1594-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1594-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1594-109">Permission type</span></span>                        | <span data-ttu-id="c1594-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1594-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c1594-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1594-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1594-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1594-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c1594-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1594-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1594-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1594-114">Not supported.</span></span>                           |
| <span data-ttu-id="c1594-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1594-115">Application</span></span>                            | <span data-ttu-id="c1594-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1594-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c1594-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1594-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c1594-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c1594-118">Function parameters</span></span>

<span data-ttu-id="c1594-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c1594-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c1594-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="c1594-120">Parameter</span></span> | <span data-ttu-id="c1594-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c1594-121">Type</span></span>   | <span data-ttu-id="c1594-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c1594-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c1594-123">period</span><span class="sxs-lookup"><span data-stu-id="c1594-123">period</span></span>    | <span data-ttu-id="c1594-124">string</span><span class="sxs-lookup"><span data-stu-id="c1594-124">string</span></span> | <span data-ttu-id="c1594-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c1594-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c1594-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c1594-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c1594-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c1594-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c1594-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1594-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c1594-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1594-129">Request headers</span></span>

| <span data-ttu-id="c1594-130">Имя</span><span class="sxs-lookup"><span data-stu-id="c1594-130">Name</span></span>          | <span data-ttu-id="c1594-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c1594-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c1594-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1594-132">Authorization</span></span> | <span data-ttu-id="c1594-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1594-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c1594-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c1594-135">If-None-Match</span></span> | <span data-ttu-id="c1594-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="c1594-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c1594-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c1594-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c1594-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1594-138">Response</span></span>

<span data-ttu-id="c1594-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c1594-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c1594-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c1594-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c1594-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c1594-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c1594-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c1594-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c1594-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c1594-143">Report Refresh Date</span></span>
- <span data-ttu-id="c1594-144">Visited Page Count (количество посещенных страниц)</span><span class="sxs-lookup"><span data-stu-id="c1594-144">Visited Page Count</span></span>
- <span data-ttu-id="c1594-145">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="c1594-145">Report Date</span></span>
- <span data-ttu-id="c1594-146">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="c1594-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c1594-147">Пример</span><span class="sxs-lookup"><span data-stu-id="c1594-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c1594-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1594-148">Request</span></span>

<span data-ttu-id="c1594-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1594-149">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c1594-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1594-150">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivitypages"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityPages(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1594-151">C#</span><span class="sxs-lookup"><span data-stu-id="c1594-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivitypages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1594-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1594-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivitypages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1594-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c1594-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivitypages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c1594-154">Java</span><span class="sxs-lookup"><span data-stu-id="c1594-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivitypages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1594-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1594-155">Response</span></span>

<span data-ttu-id="c1594-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1594-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="c1594-157">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c1594-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page Count,Report Date,Report Period
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
