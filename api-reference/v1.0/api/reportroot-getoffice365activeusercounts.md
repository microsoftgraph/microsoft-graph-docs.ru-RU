---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Получение количества активных пользователей за каждый день отчетного периода по продукту.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a031018a55e29b9237fa6c4a9ebca51c069d7917
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459218"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="bb635-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="bb635-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="bb635-104">Получение количества активных пользователей за каждый день отчетного периода по продукту.</span><span class="sxs-lookup"><span data-stu-id="bb635-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="bb635-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="bb635-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb635-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb635-106">Permissions</span></span>

<span data-ttu-id="bb635-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb635-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb635-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb635-109">Permission type</span></span>                        | <span data-ttu-id="bb635-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb635-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bb635-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb635-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb635-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb635-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bb635-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb635-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb635-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb635-114">Not supported.</span></span>                           |
| <span data-ttu-id="bb635-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb635-115">Application</span></span>                            | <span data-ttu-id="bb635-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb635-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bb635-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb635-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bb635-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb635-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bb635-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="bb635-119">Function parameters</span></span>

<span data-ttu-id="bb635-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="bb635-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bb635-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="bb635-121">Parameter</span></span> | <span data-ttu-id="bb635-122">Тип</span><span class="sxs-lookup"><span data-stu-id="bb635-122">Type</span></span>   | <span data-ttu-id="bb635-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bb635-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bb635-124">period</span><span class="sxs-lookup"><span data-stu-id="bb635-124">period</span></span>    | <span data-ttu-id="bb635-125">string</span><span class="sxs-lookup"><span data-stu-id="bb635-125">string</span></span> | <span data-ttu-id="bb635-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="bb635-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bb635-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="bb635-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bb635-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="bb635-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bb635-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb635-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="bb635-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb635-130">Request headers</span></span>

| <span data-ttu-id="bb635-131">Имя</span><span class="sxs-lookup"><span data-stu-id="bb635-131">Name</span></span>          | <span data-ttu-id="bb635-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bb635-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bb635-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb635-133">Authorization</span></span> | <span data-ttu-id="bb635-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb635-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bb635-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb635-136">Response</span></span>

<span data-ttu-id="bb635-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="bb635-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bb635-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="bb635-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bb635-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bb635-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bb635-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="bb635-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bb635-141">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="bb635-141">Report Refresh Date</span></span>
- <span data-ttu-id="bb635-142">Office 365</span><span class="sxs-lookup"><span data-stu-id="bb635-142">Office 365</span></span>
- <span data-ttu-id="bb635-143">Exchange</span><span class="sxs-lookup"><span data-stu-id="bb635-143">Exchange</span></span>
- <span data-ttu-id="bb635-144">OneDrive;</span><span class="sxs-lookup"><span data-stu-id="bb635-144">OneDrive</span></span>
- <span data-ttu-id="bb635-145">SharePoint;</span><span class="sxs-lookup"><span data-stu-id="bb635-145">SharePoint</span></span>
- <span data-ttu-id="bb635-146">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="bb635-146">Skype For Business</span></span> 
- <span data-ttu-id="bb635-147">Yammer</span><span class="sxs-lookup"><span data-stu-id="bb635-147">Yammer</span></span>
- <span data-ttu-id="bb635-148">Teams</span><span class="sxs-lookup"><span data-stu-id="bb635-148">Teams</span></span>
- <span data-ttu-id="bb635-149">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="bb635-149">Report Date</span></span>
- <span data-ttu-id="bb635-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="bb635-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="bb635-151">Пример</span><span class="sxs-lookup"><span data-stu-id="bb635-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bb635-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb635-152">Request</span></span>

<span data-ttu-id="bb635-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb635-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb635-154">C#</span><span class="sxs-lookup"><span data-stu-id="bb635-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb635-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="bb635-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb635-156">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bb635-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bb635-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb635-157">Response</span></span>

<span data-ttu-id="bb635-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb635-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="bb635-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="bb635-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
