---
title: 'reportRoot: getSkypeForBusinessActivityUserCounts'
description: Отслеживайте, как меняется количество уникальных организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 20bf04fd3213959c69a54a15db3a93ae97546755
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349270"
---
# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="38b6b-104">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="38b6b-104">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

<span data-ttu-id="38b6b-105">Отслеживайте, как меняется количество уникальных организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="38b6b-105">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="38b6b-106">Отчет также включает количество одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="38b6b-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="38b6b-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="38b6b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="38b6b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38b6b-108">Permissions</span></span>

<span data-ttu-id="38b6b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38b6b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38b6b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38b6b-111">Permission type</span></span>                        | <span data-ttu-id="38b6b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38b6b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="38b6b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38b6b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="38b6b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38b6b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="38b6b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38b6b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38b6b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38b6b-116">Not supported.</span></span>                           |
| <span data-ttu-id="38b6b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38b6b-117">Application</span></span>                            | <span data-ttu-id="38b6b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38b6b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="38b6b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38b6b-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="38b6b-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="38b6b-120">Function parameters</span></span>

<span data-ttu-id="38b6b-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="38b6b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="38b6b-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="38b6b-122">Parameter</span></span> | <span data-ttu-id="38b6b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="38b6b-123">Type</span></span>   | <span data-ttu-id="38b6b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="38b6b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="38b6b-125">period</span><span class="sxs-lookup"><span data-stu-id="38b6b-125">period</span></span>    | <span data-ttu-id="38b6b-126">string</span><span class="sxs-lookup"><span data-stu-id="38b6b-126">string</span></span> | <span data-ttu-id="38b6b-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="38b6b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="38b6b-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="38b6b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="38b6b-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="38b6b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="38b6b-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38b6b-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="38b6b-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38b6b-131">Request headers</span></span>

| <span data-ttu-id="38b6b-132">Имя</span><span class="sxs-lookup"><span data-stu-id="38b6b-132">Name</span></span>          | <span data-ttu-id="38b6b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="38b6b-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="38b6b-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38b6b-134">Authorization</span></span> | <span data-ttu-id="38b6b-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38b6b-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="38b6b-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="38b6b-137">If-None-Match</span></span> | <span data-ttu-id="38b6b-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="38b6b-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="38b6b-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="38b6b-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="38b6b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="38b6b-140">Response</span></span>

<span data-ttu-id="38b6b-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="38b6b-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="38b6b-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="38b6b-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="38b6b-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="38b6b-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="38b6b-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="38b6b-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="38b6b-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="38b6b-145">Report Refresh Date</span></span>
- <span data-ttu-id="38b6b-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="38b6b-146">Report Date</span></span>
- <span data-ttu-id="38b6b-147">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="38b6b-147">Report Period</span></span>
- <span data-ttu-id="38b6b-148">"Peer-to-peer" (Одноранговый сеанс);</span><span class="sxs-lookup"><span data-stu-id="38b6b-148">Peer-to-peer</span></span>
- <span data-ttu-id="38b6b-149">"Organized" (Организаторы);</span><span class="sxs-lookup"><span data-stu-id="38b6b-149">Organized</span></span>
- <span data-ttu-id="38b6b-150">"Participated" (Участники).</span><span class="sxs-lookup"><span data-stu-id="38b6b-150">Participated</span></span>

## <a name="example"></a><span data-ttu-id="38b6b-151">Пример</span><span class="sxs-lookup"><span data-stu-id="38b6b-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="38b6b-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="38b6b-152">Request</span></span>

<span data-ttu-id="38b6b-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38b6b-153">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="38b6b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="38b6b-154">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="38b6b-155">C#</span><span class="sxs-lookup"><span data-stu-id="38b6b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38b6b-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38b6b-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="38b6b-157">Цель — C</span><span class="sxs-lookup"><span data-stu-id="38b6b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="38b6b-158">Java</span><span class="sxs-lookup"><span data-stu-id="38b6b-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="38b6b-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="38b6b-159">Response</span></span>

<span data-ttu-id="38b6b-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="38b6b-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="38b6b-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="38b6b-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
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
