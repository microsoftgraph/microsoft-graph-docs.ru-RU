---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций (аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b96f6484ae6f4a0a6ad0cdcf54356b520298d8ca
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33604315"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="5676d-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="5676d-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

<span data-ttu-id="5676d-105">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций</span><span class="sxs-lookup"><span data-stu-id="5676d-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="5676d-106">(аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="5676d-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="5676d-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="5676d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="5676d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5676d-108">Permissions</span></span>

<span data-ttu-id="5676d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5676d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5676d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5676d-111">Permission type</span></span>                        | <span data-ttu-id="5676d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5676d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5676d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5676d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5676d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5676d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5676d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5676d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5676d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5676d-116">Not supported.</span></span>                           |
| <span data-ttu-id="5676d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5676d-117">Application</span></span>                            | <span data-ttu-id="5676d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5676d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5676d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5676d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5676d-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="5676d-120">Function parameters</span></span>

<span data-ttu-id="5676d-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="5676d-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5676d-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="5676d-122">Parameter</span></span> | <span data-ttu-id="5676d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5676d-123">Type</span></span>   | <span data-ttu-id="5676d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5676d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5676d-125">period</span><span class="sxs-lookup"><span data-stu-id="5676d-125">period</span></span>    | <span data-ttu-id="5676d-126">string</span><span class="sxs-lookup"><span data-stu-id="5676d-126">string</span></span> | <span data-ttu-id="5676d-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5676d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5676d-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="5676d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5676d-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="5676d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5676d-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5676d-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5676d-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5676d-131">Request headers</span></span>

| <span data-ttu-id="5676d-132">Имя</span><span class="sxs-lookup"><span data-stu-id="5676d-132">Name</span></span>          | <span data-ttu-id="5676d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="5676d-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5676d-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5676d-134">Authorization</span></span> | <span data-ttu-id="5676d-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5676d-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5676d-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5676d-137">If-None-Match</span></span> | <span data-ttu-id="5676d-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="5676d-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5676d-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5676d-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5676d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5676d-140">Response</span></span>

<span data-ttu-id="5676d-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="5676d-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5676d-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="5676d-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5676d-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5676d-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5676d-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="5676d-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5676d-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="5676d-145">Report Refresh Date</span></span>
- <span data-ttu-id="5676d-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="5676d-146">Report Date</span></span>
- <span data-ttu-id="5676d-147">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="5676d-147">Report Period</span></span>
- <span data-ttu-id="5676d-148">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="5676d-148">Audio/Video</span></span>
- <span data-ttu-id="5676d-149">Dial-in Microsoft (с телефонным подключением через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5676d-149">Dial-in Microsoft</span></span>
- <span data-ttu-id="5676d-150">Dial-out Microsoft (с присоединением обратным звонком через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5676d-150">Dial-out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="5676d-151">Пример</span><span class="sxs-lookup"><span data-stu-id="5676d-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5676d-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="5676d-152">Request</span></span>

<span data-ttu-id="5676d-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5676d-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="5676d-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="5676d-154">Response</span></span>

<span data-ttu-id="5676d-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5676d-155">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5676d-156">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="5676d-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5676d-157">Языках</span><span class="sxs-lookup"><span data-stu-id="5676d-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5676d-158">Язык</span><span class="sxs-lookup"><span data-stu-id="5676d-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="5676d-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="5676d-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
