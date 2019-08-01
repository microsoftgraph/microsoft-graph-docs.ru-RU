---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций (аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 6af4d5560067e30b058633e2158b9c86ef4fb781
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021741"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="e9150-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="e9150-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

<span data-ttu-id="e9150-105">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций</span><span class="sxs-lookup"><span data-stu-id="e9150-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="e9150-106">(аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="e9150-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="e9150-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="e9150-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9150-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9150-108">Permissions</span></span>

<span data-ttu-id="e9150-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9150-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9150-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9150-111">Permission type</span></span>                        | <span data-ttu-id="e9150-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9150-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e9150-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9150-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9150-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9150-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e9150-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9150-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9150-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9150-116">Not supported.</span></span>                           |
| <span data-ttu-id="e9150-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9150-117">Application</span></span>                            | <span data-ttu-id="e9150-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9150-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e9150-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9150-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e9150-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9150-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e9150-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="e9150-121">Function parameters</span></span>

<span data-ttu-id="e9150-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="e9150-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e9150-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="e9150-123">Parameter</span></span> | <span data-ttu-id="e9150-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e9150-124">Type</span></span>   | <span data-ttu-id="e9150-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e9150-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e9150-126">period</span><span class="sxs-lookup"><span data-stu-id="e9150-126">period</span></span>    | <span data-ttu-id="e9150-127">string</span><span class="sxs-lookup"><span data-stu-id="e9150-127">string</span></span> | <span data-ttu-id="e9150-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="e9150-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e9150-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="e9150-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e9150-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="e9150-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e9150-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9150-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e9150-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9150-132">Request headers</span></span>

| <span data-ttu-id="e9150-133">Имя</span><span class="sxs-lookup"><span data-stu-id="e9150-133">Name</span></span>          | <span data-ttu-id="e9150-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e9150-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e9150-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9150-135">Authorization</span></span> | <span data-ttu-id="e9150-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9150-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e9150-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e9150-138">If-None-Match</span></span> | <span data-ttu-id="e9150-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="e9150-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e9150-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e9150-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e9150-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9150-141">Response</span></span>

<span data-ttu-id="e9150-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="e9150-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e9150-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="e9150-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e9150-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e9150-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e9150-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="e9150-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e9150-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="e9150-146">Report Refresh Date</span></span>
- <span data-ttu-id="e9150-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="e9150-147">Report Date</span></span>
- <span data-ttu-id="e9150-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="e9150-148">Report Period</span></span>
- <span data-ttu-id="e9150-149">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="e9150-149">Audio/Video</span></span>
- <span data-ttu-id="e9150-150">Dial-in Microsoft (с телефонным подключением через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9150-150">Dial-in Microsoft</span></span>
- <span data-ttu-id="e9150-151">Dial-out Microsoft (с присоединением обратным звонком через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9150-151">Dial-out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="e9150-152">Пример</span><span class="sxs-lookup"><span data-stu-id="e9150-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e9150-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9150-153">Request</span></span>

<span data-ttu-id="e9150-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9150-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e9150-155">C#</span><span class="sxs-lookup"><span data-stu-id="e9150-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityminutecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9150-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="e9150-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityminutecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e9150-157">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e9150-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityminutecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e9150-158">Java</span><span class="sxs-lookup"><span data-stu-id="e9150-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivityminutecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9150-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9150-159">Response</span></span>

<span data-ttu-id="e9150-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9150-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="e9150-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="e9150-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
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
