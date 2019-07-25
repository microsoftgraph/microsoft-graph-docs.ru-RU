---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса. Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 034ea9f80345b8dbf84c4570af49c9dac10c29e2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893735"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="64373-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="64373-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="64373-105">Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="64373-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="64373-106">Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.</span><span class="sxs-lookup"><span data-stu-id="64373-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="64373-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="64373-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="64373-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64373-108">Permissions</span></span>

<span data-ttu-id="64373-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64373-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64373-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64373-111">Permission type</span></span>                        | <span data-ttu-id="64373-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64373-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="64373-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64373-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="64373-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="64373-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="64373-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64373-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64373-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64373-116">Not supported.</span></span>                           |
| <span data-ttu-id="64373-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64373-117">Application</span></span>                            | <span data-ttu-id="64373-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="64373-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="64373-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64373-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="64373-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="64373-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="64373-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="64373-121">Function parameters</span></span>

<span data-ttu-id="64373-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="64373-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="64373-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="64373-123">Parameter</span></span> | <span data-ttu-id="64373-124">Тип</span><span class="sxs-lookup"><span data-stu-id="64373-124">Type</span></span>   | <span data-ttu-id="64373-125">Описание</span><span class="sxs-lookup"><span data-stu-id="64373-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="64373-126">period</span><span class="sxs-lookup"><span data-stu-id="64373-126">period</span></span>    | <span data-ttu-id="64373-127">string</span><span class="sxs-lookup"><span data-stu-id="64373-127">string</span></span> | <span data-ttu-id="64373-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="64373-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="64373-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="64373-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="64373-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="64373-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="64373-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64373-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="64373-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64373-132">Request headers</span></span>

| <span data-ttu-id="64373-133">Имя</span><span class="sxs-lookup"><span data-stu-id="64373-133">Name</span></span>          | <span data-ttu-id="64373-134">Описание</span><span class="sxs-lookup"><span data-stu-id="64373-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="64373-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64373-135">Authorization</span></span> | <span data-ttu-id="64373-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64373-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="64373-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="64373-138">If-None-Match</span></span> | <span data-ttu-id="64373-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="64373-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="64373-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="64373-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="64373-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="64373-141">Response</span></span>

<span data-ttu-id="64373-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="64373-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="64373-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="64373-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="64373-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="64373-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="64373-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="64373-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="64373-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="64373-146">Report Refresh Date</span></span>
- <span data-ttu-id="64373-147">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="64373-147">Site Type</span></span>
- <span data-ttu-id="64373-148">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="64373-148">Total</span></span>
- <span data-ttu-id="64373-149">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="64373-149">Active</span></span>
- <span data-ttu-id="64373-150">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="64373-150">Report Date</span></span>
- <span data-ttu-id="64373-151">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="64373-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="64373-152">Пример</span><span class="sxs-lookup"><span data-stu-id="64373-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="64373-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="64373-153">Request</span></span>

<span data-ttu-id="64373-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64373-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageaccountcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="64373-155">C#</span><span class="sxs-lookup"><span data-stu-id="64373-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64373-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="64373-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64373-157">Цель — C</span><span class="sxs-lookup"><span data-stu-id="64373-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="64373-158">Java</span><span class="sxs-lookup"><span data-stu-id="64373-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusageaccountcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="64373-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="64373-159">Response</span></span>

<span data-ttu-id="64373-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64373-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="64373-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="64373-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
