---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций (аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f02f1eb78f7452f62378742f192c7023f4f037fd
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729499"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="eae86-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="eae86-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

<span data-ttu-id="eae86-105">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций</span><span class="sxs-lookup"><span data-stu-id="eae86-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="eae86-106">(аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="eae86-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="eae86-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="eae86-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="eae86-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eae86-108">Permissions</span></span>

<span data-ttu-id="eae86-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eae86-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eae86-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eae86-111">Permission type</span></span>                        | <span data-ttu-id="eae86-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eae86-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="eae86-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eae86-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="eae86-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eae86-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="eae86-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eae86-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eae86-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eae86-116">Not supported.</span></span>                           |
| <span data-ttu-id="eae86-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eae86-117">Application</span></span>                            | <span data-ttu-id="eae86-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eae86-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="eae86-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eae86-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="eae86-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="eae86-120">Function parameters</span></span>

<span data-ttu-id="eae86-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="eae86-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="eae86-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="eae86-122">Parameter</span></span> | <span data-ttu-id="eae86-123">Тип</span><span class="sxs-lookup"><span data-stu-id="eae86-123">Type</span></span>   | <span data-ttu-id="eae86-124">Описание</span><span class="sxs-lookup"><span data-stu-id="eae86-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="eae86-125">period</span><span class="sxs-lookup"><span data-stu-id="eae86-125">period</span></span>    | <span data-ttu-id="eae86-126">string</span><span class="sxs-lookup"><span data-stu-id="eae86-126">string</span></span> | <span data-ttu-id="eae86-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="eae86-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="eae86-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="eae86-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="eae86-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="eae86-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="eae86-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eae86-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="eae86-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eae86-131">Request headers</span></span>

| <span data-ttu-id="eae86-132">Имя</span><span class="sxs-lookup"><span data-stu-id="eae86-132">Name</span></span>          | <span data-ttu-id="eae86-133">Описание</span><span class="sxs-lookup"><span data-stu-id="eae86-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="eae86-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eae86-134">Authorization</span></span> | <span data-ttu-id="eae86-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eae86-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="eae86-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="eae86-137">If-None-Match</span></span> | <span data-ttu-id="eae86-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="eae86-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="eae86-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="eae86-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="eae86-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="eae86-140">Response</span></span>

<span data-ttu-id="eae86-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="eae86-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="eae86-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="eae86-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="eae86-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="eae86-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="eae86-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="eae86-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="eae86-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="eae86-145">Report Refresh Date</span></span>
- <span data-ttu-id="eae86-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="eae86-146">Report Date</span></span>
- <span data-ttu-id="eae86-147">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="eae86-147">Report Period</span></span>
- <span data-ttu-id="eae86-148">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="eae86-148">Audio/Video</span></span>
- <span data-ttu-id="eae86-149">Dial-in Microsoft (с телефонным подключением через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eae86-149">Dial-in Microsoft</span></span>
- <span data-ttu-id="eae86-150">Dial-out Microsoft (с присоединением обратным звонком через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eae86-150">Dial-out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="eae86-151">Пример</span><span class="sxs-lookup"><span data-stu-id="eae86-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="eae86-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="eae86-152">Request</span></span>

<span data-ttu-id="eae86-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eae86-153">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="eae86-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="eae86-154">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eae86-155">C#</span><span class="sxs-lookup"><span data-stu-id="eae86-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityminutecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eae86-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eae86-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityminutecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eae86-157">Цель — C</span><span class="sxs-lookup"><span data-stu-id="eae86-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityminutecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eae86-158">Java</span><span class="sxs-lookup"><span data-stu-id="eae86-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivityminutecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eae86-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="eae86-159">Response</span></span>

<span data-ttu-id="eae86-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eae86-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="eae86-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="eae86-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
