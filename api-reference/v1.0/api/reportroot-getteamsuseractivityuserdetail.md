---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Получение сведений о действиях отдельных пользователей Microsoft Teams.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 6de0af2b1ec30e21658dc8fa2f4ab6bbb56379db
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369430"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="645ab-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="645ab-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="645ab-104">Получение сведений о действиях отдельных пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="645ab-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="645ab-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="645ab-105">Permissions</span></span>

<span data-ttu-id="645ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="645ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="645ab-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="645ab-108">Permission type</span></span>                        | <span data-ttu-id="645ab-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="645ab-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="645ab-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="645ab-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="645ab-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="645ab-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="645ab-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="645ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="645ab-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="645ab-113">Not supported.</span></span>                           |
| <span data-ttu-id="645ab-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="645ab-114">Application</span></span>                            | <span data-ttu-id="645ab-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="645ab-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="645ab-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="645ab-116">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="645ab-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="645ab-117">Function parameters</span></span>

<span data-ttu-id="645ab-118">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="645ab-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="645ab-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="645ab-119">Parameter</span></span> | <span data-ttu-id="645ab-120">Тип</span><span class="sxs-lookup"><span data-stu-id="645ab-120">Type</span></span>   | <span data-ttu-id="645ab-121">Описание</span><span class="sxs-lookup"><span data-stu-id="645ab-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="645ab-122">period</span><span class="sxs-lookup"><span data-stu-id="645ab-122">period</span></span>    | <span data-ttu-id="645ab-123">string</span><span class="sxs-lookup"><span data-stu-id="645ab-123">string</span></span> | <span data-ttu-id="645ab-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="645ab-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="645ab-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="645ab-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="645ab-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="645ab-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="645ab-127">date</span><span class="sxs-lookup"><span data-stu-id="645ab-127">date</span></span>      | <span data-ttu-id="645ab-128">Date</span><span class="sxs-lookup"><span data-stu-id="645ab-128">Date</span></span>   | <span data-ttu-id="645ab-129">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="645ab-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="645ab-130">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="645ab-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="645ab-131">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="645ab-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="645ab-132">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="645ab-132">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="645ab-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="645ab-133">Request headers</span></span>

| <span data-ttu-id="645ab-134">Имя</span><span class="sxs-lookup"><span data-stu-id="645ab-134">Name</span></span>          | <span data-ttu-id="645ab-135">Описание</span><span class="sxs-lookup"><span data-stu-id="645ab-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="645ab-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="645ab-136">Authorization</span></span> | <span data-ttu-id="645ab-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="645ab-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="645ab-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="645ab-139">Response</span></span>

<span data-ttu-id="645ab-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="645ab-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="645ab-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="645ab-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="645ab-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="645ab-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="645ab-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="645ab-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="645ab-144">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="645ab-144">Report Refresh Date</span></span>
- <span data-ttu-id="645ab-145">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="645ab-145">User Principal Name</span></span>
- <span data-ttu-id="645ab-146">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="645ab-146">Last Activity Date</span></span>
- <span data-ttu-id="645ab-147">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="645ab-147">Is Deleted</span></span>
- <span data-ttu-id="645ab-148">Deleted Date (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="645ab-148">Deleted Date</span></span>
- <span data-ttu-id="645ab-149">Assigned Products (Назначенные продукты);</span><span class="sxs-lookup"><span data-stu-id="645ab-149">Assigned Products</span></span>
- <span data-ttu-id="645ab-150">Team Chat Messages Count (Количество сообщений в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="645ab-150">Team Chat Message Count</span></span>
- <span data-ttu-id="645ab-151">Private Chat Message Count (Количество сообщений в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="645ab-151">Private Chat Message Count</span></span>
- <span data-ttu-id="645ab-152">Call Count (Количество звонков);</span><span class="sxs-lookup"><span data-stu-id="645ab-152">Call Count</span></span>
- <span data-ttu-id="645ab-153">Meeting Count (Количество собраний);</span><span class="sxs-lookup"><span data-stu-id="645ab-153">Meeting Count</span></span>
- <span data-ttu-id="645ab-154">Has Other Action (Есть другое действие);</span><span class="sxs-lookup"><span data-stu-id="645ab-154">Has Other Action</span></span>
- <span data-ttu-id="645ab-155">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="645ab-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="645ab-156">Пример</span><span class="sxs-lookup"><span data-stu-id="645ab-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="645ab-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="645ab-157">Request</span></span>

<span data-ttu-id="645ab-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="645ab-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="645ab-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="645ab-159">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="645ab-160">C#</span><span class="sxs-lookup"><span data-stu-id="645ab-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="645ab-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="645ab-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="645ab-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="645ab-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="645ab-163">Java</span><span class="sxs-lookup"><span data-stu-id="645ab-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="645ab-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="645ab-164">Response</span></span>

<span data-ttu-id="645ab-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="645ab-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="645ab-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="645ab-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
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
