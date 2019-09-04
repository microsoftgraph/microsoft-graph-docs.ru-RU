---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Узнайте, сколько пользователей были активны и неактивны в каждой службе.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 55a2d651f225cafbe6c49de29cf5e1125f40f999
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729674"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="50f9a-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="50f9a-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="50f9a-104">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="50f9a-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="50f9a-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="50f9a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="50f9a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50f9a-106">Permissions</span></span>

<span data-ttu-id="50f9a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50f9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50f9a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50f9a-109">Permission type</span></span>                        | <span data-ttu-id="50f9a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50f9a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="50f9a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50f9a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="50f9a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="50f9a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="50f9a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50f9a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50f9a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50f9a-114">Not supported.</span></span>                           |
| <span data-ttu-id="50f9a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50f9a-115">Application</span></span>                            | <span data-ttu-id="50f9a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="50f9a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="50f9a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50f9a-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="50f9a-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="50f9a-118">Function parameters</span></span>

<span data-ttu-id="50f9a-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="50f9a-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="50f9a-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="50f9a-120">Parameter</span></span> | <span data-ttu-id="50f9a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="50f9a-121">Type</span></span>   | <span data-ttu-id="50f9a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="50f9a-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="50f9a-123">period</span><span class="sxs-lookup"><span data-stu-id="50f9a-123">period</span></span>    | <span data-ttu-id="50f9a-124">string</span><span class="sxs-lookup"><span data-stu-id="50f9a-124">string</span></span> | <span data-ttu-id="50f9a-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="50f9a-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="50f9a-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="50f9a-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="50f9a-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="50f9a-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="50f9a-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50f9a-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="50f9a-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50f9a-129">Request headers</span></span>

| <span data-ttu-id="50f9a-130">Имя</span><span class="sxs-lookup"><span data-stu-id="50f9a-130">Name</span></span>          | <span data-ttu-id="50f9a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="50f9a-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="50f9a-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50f9a-132">Authorization</span></span> | <span data-ttu-id="50f9a-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50f9a-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="50f9a-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="50f9a-135">If-None-Match</span></span> | <span data-ttu-id="50f9a-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="50f9a-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="50f9a-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="50f9a-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="50f9a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="50f9a-138">Response</span></span>

<span data-ttu-id="50f9a-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="50f9a-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="50f9a-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="50f9a-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="50f9a-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="50f9a-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="50f9a-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="50f9a-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="50f9a-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="50f9a-143">Report Refresh Date</span></span>
- <span data-ttu-id="50f9a-144">Exchange Active (активны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="50f9a-144">Exchange Active</span></span>
- <span data-ttu-id="50f9a-145">Exchange Inactive (неактивны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="50f9a-145">Exchange Inactive</span></span>
- <span data-ttu-id="50f9a-146">OneDrive Active (активны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="50f9a-146">OneDrive Active</span></span>
- <span data-ttu-id="50f9a-147">OneDrive Inactive (неактивны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="50f9a-147">OneDrive Inactive</span></span>
- <span data-ttu-id="50f9a-148">SharePoint Active (активны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="50f9a-148">SharePoint Active</span></span>
- <span data-ttu-id="50f9a-149">SharePoint Inactive (неактивны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="50f9a-149">SharePoint Inactive</span></span>
- <span data-ttu-id="50f9a-150">Skype For Business Active (активны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="50f9a-150">Skype For Business Active</span></span>
- <span data-ttu-id="50f9a-151">Skype For Business Inactive (неактивны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="50f9a-151">Skype For Business Inactive</span></span>
- <span data-ttu-id="50f9a-152">Yammer Active (активны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="50f9a-152">Yammer Active</span></span>
- <span data-ttu-id="50f9a-153">Yammer Inactive (неактивны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="50f9a-153">Yammer Inactive</span></span>
- <span data-ttu-id="50f9a-154">Teams Active (активны в Teams)</span><span class="sxs-lookup"><span data-stu-id="50f9a-154">Teams Active</span></span>
- <span data-ttu-id="50f9a-155">Teams Inactive (неактивны в Teams)</span><span class="sxs-lookup"><span data-stu-id="50f9a-155">Teams Inactive</span></span>
- <span data-ttu-id="50f9a-156">Office 365 активен</span><span class="sxs-lookup"><span data-stu-id="50f9a-156">Office 365 Active</span></span>
- <span data-ttu-id="50f9a-157">Office 365 неактивен</span><span class="sxs-lookup"><span data-stu-id="50f9a-157">Office 365 Inactive</span></span>
- <span data-ttu-id="50f9a-158">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="50f9a-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="50f9a-159">Пример</span><span class="sxs-lookup"><span data-stu-id="50f9a-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="50f9a-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="50f9a-160">Request</span></span>

<span data-ttu-id="50f9a-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50f9a-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="50f9a-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="50f9a-162">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="50f9a-163">C#</span><span class="sxs-lookup"><span data-stu-id="50f9a-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50f9a-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50f9a-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="50f9a-165">Цель — C</span><span class="sxs-lookup"><span data-stu-id="50f9a-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="50f9a-166">Java</span><span class="sxs-lookup"><span data-stu-id="50f9a-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365servicesusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="50f9a-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="50f9a-167">Response</span></span>

<span data-ttu-id="50f9a-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="50f9a-168">The following is an example of the response.</span></span>

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

<span data-ttu-id="50f9a-169">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="50f9a-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Office 365 Active,Office 365 Inactive,Report Period
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
