---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Получение количества активных пользователей за каждый день отчетного периода по продукту.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9b79493e60ea6e9fdc24496ff39d73ebb3959109
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268700"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="887b7-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="887b7-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="887b7-104">Получение количества активных пользователей за каждый день отчетного периода по продукту.</span><span class="sxs-lookup"><span data-stu-id="887b7-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="887b7-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="887b7-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="887b7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="887b7-106">Permissions</span></span>

<span data-ttu-id="887b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="887b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="887b7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="887b7-109">Permission type</span></span>                        | <span data-ttu-id="887b7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="887b7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="887b7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="887b7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="887b7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="887b7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="887b7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="887b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="887b7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="887b7-114">Not supported.</span></span>                           |
| <span data-ttu-id="887b7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="887b7-115">Application</span></span>                            | <span data-ttu-id="887b7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="887b7-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="887b7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="887b7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="887b7-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="887b7-118">Function parameters</span></span>

<span data-ttu-id="887b7-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="887b7-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="887b7-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="887b7-120">Parameter</span></span> | <span data-ttu-id="887b7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="887b7-121">Type</span></span>   | <span data-ttu-id="887b7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="887b7-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="887b7-123">period</span><span class="sxs-lookup"><span data-stu-id="887b7-123">period</span></span>    | <span data-ttu-id="887b7-124">string</span><span class="sxs-lookup"><span data-stu-id="887b7-124">string</span></span> | <span data-ttu-id="887b7-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="887b7-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="887b7-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="887b7-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="887b7-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="887b7-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="887b7-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="887b7-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="887b7-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="887b7-129">Request headers</span></span>

| <span data-ttu-id="887b7-130">Имя</span><span class="sxs-lookup"><span data-stu-id="887b7-130">Name</span></span>          | <span data-ttu-id="887b7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="887b7-131">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="887b7-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="887b7-132">Authorization</span></span> | <span data-ttu-id="887b7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="887b7-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="887b7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="887b7-135">Response</span></span>

<span data-ttu-id="887b7-136">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="887b7-136">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="887b7-137">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="887b7-137">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="887b7-138">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="887b7-138">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="887b7-139">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="887b7-139">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="887b7-140">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="887b7-140">Report Refresh Date</span></span>
- <span data-ttu-id="887b7-141">Office 365</span><span class="sxs-lookup"><span data-stu-id="887b7-141">Office 365</span></span>
- <span data-ttu-id="887b7-142">Exchange</span><span class="sxs-lookup"><span data-stu-id="887b7-142">Exchange</span></span>
- <span data-ttu-id="887b7-143">OneDrive;</span><span class="sxs-lookup"><span data-stu-id="887b7-143">OneDrive</span></span>
- <span data-ttu-id="887b7-144">SharePoint;</span><span class="sxs-lookup"><span data-stu-id="887b7-144">SharePoint</span></span>
- <span data-ttu-id="887b7-145">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="887b7-145">Skype For Business</span></span> 
- <span data-ttu-id="887b7-146">Yammer</span><span class="sxs-lookup"><span data-stu-id="887b7-146">Yammer</span></span>
- <span data-ttu-id="887b7-147">Teams</span><span class="sxs-lookup"><span data-stu-id="887b7-147">Teams</span></span>
- <span data-ttu-id="887b7-148">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="887b7-148">Report Date</span></span>
- <span data-ttu-id="887b7-149">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="887b7-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="887b7-150">Пример</span><span class="sxs-lookup"><span data-stu-id="887b7-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="887b7-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="887b7-151">Request</span></span>

<span data-ttu-id="887b7-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="887b7-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="887b7-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="887b7-153">Response</span></span>

<span data-ttu-id="887b7-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="887b7-154">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="887b7-155">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="887b7-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="887b7-156">C#</span><span class="sxs-lookup"><span data-stu-id="887b7-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="887b7-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="887b7-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="887b7-158">Цель — C</span><span class="sxs-lookup"><span data-stu-id="887b7-158">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="887b7-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="887b7-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
