---
title: 'reportRoot: getOneDriveUsageStorage'
description: Получение сведений о том, как меняется используемый объем хранилища в OneDrive для бизнеса.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4981e33a939d4def10212b74e9a125b6ce5efade
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33604564"
---
# <a name="reportroot-getonedriveusagestorage"></a><span data-ttu-id="1ade7-103">reportRoot: getOneDriveUsageStorage</span><span class="sxs-lookup"><span data-stu-id="1ade7-103">reportRoot: getOneDriveUsageStorage</span></span>

<span data-ttu-id="1ade7-104">Получение сведений о том, как меняется используемый объем хранилища в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1ade7-104">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span>

> <span data-ttu-id="1ade7-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="1ade7-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="1ade7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ade7-106">Permissions</span></span>

<span data-ttu-id="1ade7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ade7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ade7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ade7-109">Permission type</span></span>                        | <span data-ttu-id="1ade7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ade7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1ade7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ade7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ade7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ade7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1ade7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ade7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ade7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ade7-114">Not supported.</span></span>                           |
| <span data-ttu-id="1ade7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ade7-115">Application</span></span>                            | <span data-ttu-id="1ade7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ade7-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1ade7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ade7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1ade7-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="1ade7-118">Function parameters</span></span>

<span data-ttu-id="1ade7-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="1ade7-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1ade7-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="1ade7-120">Parameter</span></span> | <span data-ttu-id="1ade7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1ade7-121">Type</span></span>   | <span data-ttu-id="1ade7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1ade7-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1ade7-123">period</span><span class="sxs-lookup"><span data-stu-id="1ade7-123">period</span></span>    | <span data-ttu-id="1ade7-124">string</span><span class="sxs-lookup"><span data-stu-id="1ade7-124">string</span></span> | <span data-ttu-id="1ade7-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="1ade7-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1ade7-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="1ade7-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1ade7-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="1ade7-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1ade7-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ade7-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1ade7-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ade7-129">Request headers</span></span>

| <span data-ttu-id="1ade7-130">Имя</span><span class="sxs-lookup"><span data-stu-id="1ade7-130">Name</span></span>          | <span data-ttu-id="1ade7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1ade7-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="1ade7-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ade7-132">Authorization</span></span> | <span data-ttu-id="1ade7-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ade7-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="1ade7-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1ade7-135">If-None-Match</span></span> | <span data-ttu-id="1ade7-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="1ade7-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1ade7-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1ade7-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1ade7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ade7-138">Response</span></span>

<span data-ttu-id="1ade7-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="1ade7-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1ade7-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="1ade7-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1ade7-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1ade7-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1ade7-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="1ade7-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1ade7-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="1ade7-143">Report Refresh Date</span></span>
- <span data-ttu-id="1ade7-144">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="1ade7-144">Site Type</span></span>
- <span data-ttu-id="1ade7-145">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="1ade7-145">Storage Used (Byte)</span></span>
- <span data-ttu-id="1ade7-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="1ade7-146">Report Date</span></span>
- <span data-ttu-id="1ade7-147">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="1ade7-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="1ade7-148">Пример</span><span class="sxs-lookup"><span data-stu-id="1ade7-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1ade7-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ade7-149">Request</span></span>

<span data-ttu-id="1ade7-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ade7-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusagestorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageStorage(period='D7')
```

#### <a name="response"></a><span data-ttu-id="1ade7-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ade7-151">Response</span></span>

<span data-ttu-id="1ade7-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ade7-152">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1ade7-153">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="1ade7-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1ade7-154">Языках</span><span class="sxs-lookup"><span data-stu-id="1ade7-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusagestorage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ade7-155">Язык</span><span class="sxs-lookup"><span data-stu-id="1ade7-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusagestorage-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="1ade7-156">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="1ade7-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getonedriveusagestorage.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getonedriveusagestorage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
