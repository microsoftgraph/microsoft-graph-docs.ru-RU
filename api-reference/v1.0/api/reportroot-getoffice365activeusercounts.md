---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Получение количества активных пользователей за каждый день отчетного периода по продукту.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d84596fc283b09c0cbf30c8855424c7e76f4e45e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022005"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="1a63b-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="1a63b-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="1a63b-104">Получение количества активных пользователей за каждый день отчетного периода по продукту.</span><span class="sxs-lookup"><span data-stu-id="1a63b-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="1a63b-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="1a63b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a63b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a63b-106">Permissions</span></span>

<span data-ttu-id="1a63b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a63b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a63b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a63b-109">Permission type</span></span>                        | <span data-ttu-id="1a63b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a63b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1a63b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a63b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a63b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a63b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1a63b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a63b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a63b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a63b-114">Not supported.</span></span>                           |
| <span data-ttu-id="1a63b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a63b-115">Application</span></span>                            | <span data-ttu-id="1a63b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a63b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1a63b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a63b-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1a63b-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a63b-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1a63b-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="1a63b-119">Function parameters</span></span>

<span data-ttu-id="1a63b-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="1a63b-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1a63b-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="1a63b-121">Parameter</span></span> | <span data-ttu-id="1a63b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1a63b-122">Type</span></span>   | <span data-ttu-id="1a63b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1a63b-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1a63b-124">period</span><span class="sxs-lookup"><span data-stu-id="1a63b-124">period</span></span>    | <span data-ttu-id="1a63b-125">string</span><span class="sxs-lookup"><span data-stu-id="1a63b-125">string</span></span> | <span data-ttu-id="1a63b-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="1a63b-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1a63b-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="1a63b-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1a63b-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="1a63b-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1a63b-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a63b-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1a63b-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a63b-130">Request headers</span></span>

| <span data-ttu-id="1a63b-131">Имя</span><span class="sxs-lookup"><span data-stu-id="1a63b-131">Name</span></span>          | <span data-ttu-id="1a63b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1a63b-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1a63b-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a63b-133">Authorization</span></span> | <span data-ttu-id="1a63b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a63b-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1a63b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a63b-136">Response</span></span>

<span data-ttu-id="1a63b-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="1a63b-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1a63b-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="1a63b-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1a63b-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1a63b-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1a63b-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="1a63b-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1a63b-141">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="1a63b-141">Report Refresh Date</span></span>
- <span data-ttu-id="1a63b-142">Office 365</span><span class="sxs-lookup"><span data-stu-id="1a63b-142">Office 365</span></span>
- <span data-ttu-id="1a63b-143">Exchange</span><span class="sxs-lookup"><span data-stu-id="1a63b-143">Exchange</span></span>
- <span data-ttu-id="1a63b-144">OneDrive;</span><span class="sxs-lookup"><span data-stu-id="1a63b-144">OneDrive</span></span>
- <span data-ttu-id="1a63b-145">SharePoint;</span><span class="sxs-lookup"><span data-stu-id="1a63b-145">SharePoint</span></span>
- <span data-ttu-id="1a63b-146">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="1a63b-146">Skype For Business</span></span> 
- <span data-ttu-id="1a63b-147">Yammer</span><span class="sxs-lookup"><span data-stu-id="1a63b-147">Yammer</span></span>
- <span data-ttu-id="1a63b-148">Teams</span><span class="sxs-lookup"><span data-stu-id="1a63b-148">Teams</span></span>
- <span data-ttu-id="1a63b-149">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="1a63b-149">Report Date</span></span>
- <span data-ttu-id="1a63b-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="1a63b-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="1a63b-151">Пример</span><span class="sxs-lookup"><span data-stu-id="1a63b-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1a63b-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a63b-152">Request</span></span>

<span data-ttu-id="1a63b-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a63b-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a63b-154">C#</span><span class="sxs-lookup"><span data-stu-id="1a63b-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a63b-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a63b-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a63b-156">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1a63b-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1a63b-157">Java</span><span class="sxs-lookup"><span data-stu-id="1a63b-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activeusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1a63b-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a63b-158">Response</span></span>

<span data-ttu-id="1a63b-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1a63b-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="1a63b-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="1a63b-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
