---
title: 'reportRoot: getOffice365GroupsActivityFileCounts'
description: Узнайте, сколько всего файлов на всех связанных с группой Office 365 сайтах и сколько из них были активны.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 436610cb30761087d0cab2da99d0afb5c0c20612
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459211"
---
# <a name="reportroot-getoffice365groupsactivityfilecounts"></a><span data-ttu-id="24709-103">reportRoot: getOffice365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="24709-103">reportRoot: getOffice365GroupsActivityFileCounts</span></span>

<span data-ttu-id="24709-104">Узнайте, сколько всего файлов на всех связанных с группой Office 365 сайтах и сколько из них были активны.</span><span class="sxs-lookup"><span data-stu-id="24709-104">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span>

> <span data-ttu-id="24709-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="24709-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="24709-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24709-106">Permissions</span></span>

<span data-ttu-id="24709-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24709-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24709-109">Permission type</span></span>                        | <span data-ttu-id="24709-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24709-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="24709-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24709-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="24709-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="24709-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="24709-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24709-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24709-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24709-114">Not supported.</span></span>                           |
| <span data-ttu-id="24709-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24709-115">Application</span></span>                            | <span data-ttu-id="24709-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="24709-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="24709-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24709-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="24709-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="24709-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="24709-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="24709-119">Function parameters</span></span>

<span data-ttu-id="24709-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="24709-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="24709-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="24709-121">Parameter</span></span> | <span data-ttu-id="24709-122">Тип</span><span class="sxs-lookup"><span data-stu-id="24709-122">Type</span></span>   | <span data-ttu-id="24709-123">Описание</span><span class="sxs-lookup"><span data-stu-id="24709-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="24709-124">period</span><span class="sxs-lookup"><span data-stu-id="24709-124">period</span></span>    | <span data-ttu-id="24709-125">string</span><span class="sxs-lookup"><span data-stu-id="24709-125">string</span></span> | <span data-ttu-id="24709-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="24709-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="24709-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="24709-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="24709-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="24709-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="24709-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24709-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="24709-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24709-130">Request headers</span></span>

| <span data-ttu-id="24709-131">Имя</span><span class="sxs-lookup"><span data-stu-id="24709-131">Name</span></span>          | <span data-ttu-id="24709-132">Описание</span><span class="sxs-lookup"><span data-stu-id="24709-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="24709-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24709-133">Authorization</span></span> | <span data-ttu-id="24709-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24709-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="24709-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="24709-136">If-None-Match</span></span> | <span data-ttu-id="24709-137">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="24709-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="24709-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="24709-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="24709-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="24709-139">Response</span></span>

<span data-ttu-id="24709-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="24709-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="24709-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="24709-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="24709-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="24709-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="24709-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="24709-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="24709-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="24709-144">Report Refresh Date</span></span>
- <span data-ttu-id="24709-145">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="24709-145">Total</span></span>
- <span data-ttu-id="24709-146">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="24709-146">Active</span></span>
- <span data-ttu-id="24709-147">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="24709-147">Report Date</span></span>
- <span data-ttu-id="24709-148">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="24709-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="24709-149">Пример</span><span class="sxs-lookup"><span data-stu-id="24709-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="24709-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="24709-150">Request</span></span>

<span data-ttu-id="24709-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24709-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityfilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityFileCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="24709-152">C#</span><span class="sxs-lookup"><span data-stu-id="24709-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivityfilecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24709-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="24709-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivityfilecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="24709-154">Цель — C</span><span class="sxs-lookup"><span data-stu-id="24709-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivityfilecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="24709-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="24709-155">Response</span></span>

<span data-ttu-id="24709-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="24709-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="24709-157">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="24709-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
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
