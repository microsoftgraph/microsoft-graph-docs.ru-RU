---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 637826d9eb5b26646436fc6ffd77b4c1b272c837
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729436"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="32581-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="32581-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="32581-104">Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.</span><span class="sxs-lookup"><span data-stu-id="32581-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="32581-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32581-105">Permissions</span></span>

<span data-ttu-id="32581-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32581-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32581-108">Permission type</span></span>                        | <span data-ttu-id="32581-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32581-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="32581-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32581-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="32581-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="32581-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="32581-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32581-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32581-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32581-113">Not supported.</span></span>                           |
| <span data-ttu-id="32581-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32581-114">Application</span></span>                            | <span data-ttu-id="32581-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="32581-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="32581-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32581-116">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='{period_value}')
GET /reports/getTeamsDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="32581-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="32581-117">Function parameters</span></span>

<span data-ttu-id="32581-118">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="32581-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="32581-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="32581-119">Parameter</span></span> | <span data-ttu-id="32581-120">Тип</span><span class="sxs-lookup"><span data-stu-id="32581-120">Type</span></span>   | <span data-ttu-id="32581-121">Описание</span><span class="sxs-lookup"><span data-stu-id="32581-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="32581-122">period</span><span class="sxs-lookup"><span data-stu-id="32581-122">period</span></span>    | <span data-ttu-id="32581-123">string</span><span class="sxs-lookup"><span data-stu-id="32581-123">string</span></span> | <span data-ttu-id="32581-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="32581-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="32581-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="32581-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="32581-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="32581-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="32581-127">date</span><span class="sxs-lookup"><span data-stu-id="32581-127">date</span></span>      | <span data-ttu-id="32581-128">Date</span><span class="sxs-lookup"><span data-stu-id="32581-128">Date</span></span>   | <span data-ttu-id="32581-129">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="32581-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="32581-130">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="32581-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="32581-131">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="32581-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="32581-132">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="32581-132">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32581-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32581-133">Request headers</span></span>

| <span data-ttu-id="32581-134">Имя</span><span class="sxs-lookup"><span data-stu-id="32581-134">Name</span></span>          | <span data-ttu-id="32581-135">Описание</span><span class="sxs-lookup"><span data-stu-id="32581-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="32581-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32581-136">Authorization</span></span> | <span data-ttu-id="32581-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32581-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="32581-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="32581-139">Response</span></span>

<span data-ttu-id="32581-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="32581-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="32581-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="32581-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="32581-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="32581-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="32581-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="32581-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="32581-144">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="32581-144">Report Refresh Date</span></span>
- <span data-ttu-id="32581-145">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="32581-145">User Principal Name</span></span>
- <span data-ttu-id="32581-146">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="32581-146">Last Activity Date</span></span>
- <span data-ttu-id="32581-147">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="32581-147">Is Deleted</span></span>
- <span data-ttu-id="32581-148">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="32581-148">Deleted Date</span></span>
- <span data-ttu-id="32581-149">Used Web (использовал браузер);</span><span class="sxs-lookup"><span data-stu-id="32581-149">Used Web</span></span>
- <span data-ttu-id="32581-150">Used Windows Phone (использовал телефон с Windows);</span><span class="sxs-lookup"><span data-stu-id="32581-150">Used Windows Phone</span></span>
- <span data-ttu-id="32581-151">Used iOS (использовал iOS);</span><span class="sxs-lookup"><span data-stu-id="32581-151">Used iOS</span></span>
- <span data-ttu-id="32581-152">Used Mac (использовал Mac);</span><span class="sxs-lookup"><span data-stu-id="32581-152">Used Mac</span></span>
- <span data-ttu-id="32581-153">Used Android Phone (использовал телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="32581-153">Used Android Phone</span></span>
- <span data-ttu-id="32581-154">Used Windows (использовал Windows);</span><span class="sxs-lookup"><span data-stu-id="32581-154">Used Windows</span></span>
- <span data-ttu-id="32581-155">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="32581-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="32581-156">Пример</span><span class="sxs-lookup"><span data-stu-id="32581-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="32581-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="32581-157">Request</span></span>

<span data-ttu-id="32581-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32581-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="32581-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="32581-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="32581-160">C#</span><span class="sxs-lookup"><span data-stu-id="32581-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32581-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32581-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="32581-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="32581-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="32581-163">Java</span><span class="sxs-lookup"><span data-stu-id="32581-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="32581-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="32581-164">Response</span></span>

<span data-ttu-id="32581-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="32581-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="32581-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="32581-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
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
