---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса. Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9d9fbb9b48b59ad80ec38d52c2e4744037210b84
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33604989"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="25c79-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="25c79-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="25c79-105">Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="25c79-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="25c79-106">Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.</span><span class="sxs-lookup"><span data-stu-id="25c79-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="25c79-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="25c79-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="25c79-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25c79-108">Permissions</span></span>

<span data-ttu-id="25c79-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25c79-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25c79-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25c79-111">Permission type</span></span>                        | <span data-ttu-id="25c79-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25c79-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="25c79-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25c79-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="25c79-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="25c79-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="25c79-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25c79-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25c79-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25c79-116">Not supported.</span></span>                           |
| <span data-ttu-id="25c79-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25c79-117">Application</span></span>                            | <span data-ttu-id="25c79-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="25c79-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="25c79-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25c79-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="25c79-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="25c79-120">Function parameters</span></span>

<span data-ttu-id="25c79-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="25c79-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="25c79-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="25c79-122">Parameter</span></span> | <span data-ttu-id="25c79-123">Тип</span><span class="sxs-lookup"><span data-stu-id="25c79-123">Type</span></span>   | <span data-ttu-id="25c79-124">Описание</span><span class="sxs-lookup"><span data-stu-id="25c79-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="25c79-125">period</span><span class="sxs-lookup"><span data-stu-id="25c79-125">period</span></span>    | <span data-ttu-id="25c79-126">string</span><span class="sxs-lookup"><span data-stu-id="25c79-126">string</span></span> | <span data-ttu-id="25c79-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="25c79-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="25c79-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="25c79-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="25c79-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="25c79-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="25c79-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25c79-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="25c79-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25c79-131">Request headers</span></span>

| <span data-ttu-id="25c79-132">Имя</span><span class="sxs-lookup"><span data-stu-id="25c79-132">Name</span></span>          | <span data-ttu-id="25c79-133">Описание</span><span class="sxs-lookup"><span data-stu-id="25c79-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="25c79-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25c79-134">Authorization</span></span> | <span data-ttu-id="25c79-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25c79-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="25c79-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="25c79-137">If-None-Match</span></span> | <span data-ttu-id="25c79-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="25c79-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="25c79-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="25c79-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="25c79-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="25c79-140">Response</span></span>

<span data-ttu-id="25c79-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="25c79-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="25c79-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="25c79-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="25c79-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="25c79-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="25c79-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="25c79-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="25c79-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="25c79-145">Report Refresh Date</span></span>
- <span data-ttu-id="25c79-146">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="25c79-146">Site Type</span></span>
- <span data-ttu-id="25c79-147">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="25c79-147">Total</span></span>
- <span data-ttu-id="25c79-148">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="25c79-148">Active</span></span>
- <span data-ttu-id="25c79-149">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="25c79-149">Report Date</span></span>
- <span data-ttu-id="25c79-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="25c79-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="25c79-151">Пример</span><span class="sxs-lookup"><span data-stu-id="25c79-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="25c79-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="25c79-152">Request</span></span>

<span data-ttu-id="25c79-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25c79-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageaccountcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="25c79-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="25c79-154">Response</span></span>

<span data-ttu-id="25c79-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="25c79-155">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="25c79-156">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="25c79-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="25c79-157">Языках</span><span class="sxs-lookup"><span data-stu-id="25c79-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountcounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25c79-158">Язык</span><span class="sxs-lookup"><span data-stu-id="25c79-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountcounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="25c79-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="25c79-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
    "Error: /api-reference/v1.0/api/reportroot-getonedriveusageaccountcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getonedriveusageaccountcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
