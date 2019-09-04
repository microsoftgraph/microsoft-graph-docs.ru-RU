---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityCounts'
description: Отслеживайте динамику использования по количеству и типу проведенных в организации сеансов (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 47ffd094fd3d653295878d60255c876a44899931
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727945"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="3c53d-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="3c53d-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

<span data-ttu-id="3c53d-105">Отслеживайте динамику использования по количеству и типу проведенных в организации сеансов</span><span class="sxs-lookup"><span data-stu-id="3c53d-105">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="3c53d-106">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов).</span><span class="sxs-lookup"><span data-stu-id="3c53d-106">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="3c53d-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="3c53d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c53d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c53d-108">Permissions</span></span>

<span data-ttu-id="3c53d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c53d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c53d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c53d-111">Permission type</span></span>                        | <span data-ttu-id="3c53d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c53d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3c53d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c53d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c53d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c53d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3c53d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c53d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c53d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c53d-116">Not supported.</span></span>                           |
| <span data-ttu-id="3c53d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c53d-117">Application</span></span>                            | <span data-ttu-id="3c53d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c53d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3c53d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c53d-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3c53d-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3c53d-120">Function parameters</span></span>

<span data-ttu-id="3c53d-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3c53d-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3c53d-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="3c53d-122">Parameter</span></span> | <span data-ttu-id="3c53d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3c53d-123">Type</span></span>   | <span data-ttu-id="3c53d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3c53d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3c53d-125">period</span><span class="sxs-lookup"><span data-stu-id="3c53d-125">period</span></span>    | <span data-ttu-id="3c53d-126">string</span><span class="sxs-lookup"><span data-stu-id="3c53d-126">string</span></span> | <span data-ttu-id="3c53d-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3c53d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3c53d-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3c53d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3c53d-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3c53d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3c53d-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c53d-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3c53d-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c53d-131">Request headers</span></span>

| <span data-ttu-id="3c53d-132">Имя</span><span class="sxs-lookup"><span data-stu-id="3c53d-132">Name</span></span>          | <span data-ttu-id="3c53d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3c53d-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3c53d-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c53d-134">Authorization</span></span> | <span data-ttu-id="3c53d-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c53d-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3c53d-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3c53d-137">If-None-Match</span></span> | <span data-ttu-id="3c53d-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="3c53d-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3c53d-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3c53d-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3c53d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c53d-140">Response</span></span>

<span data-ttu-id="3c53d-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3c53d-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3c53d-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3c53d-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3c53d-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3c53d-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3c53d-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3c53d-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3c53d-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3c53d-145">Report Refresh Date</span></span>
- <span data-ttu-id="3c53d-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="3c53d-146">Report Date</span></span>
- <span data-ttu-id="3c53d-147">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="3c53d-147">Report Period</span></span>
- <span data-ttu-id="3c53d-148">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="3c53d-148">IM</span></span>
- <span data-ttu-id="3c53d-149">"Audio" (Аудио);</span><span class="sxs-lookup"><span data-stu-id="3c53d-149">Audio</span></span>
- <span data-ttu-id="3c53d-150">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="3c53d-150">Video</span></span>
- <span data-ttu-id="3c53d-151">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="3c53d-151">App Sharing</span></span>
- <span data-ttu-id="3c53d-152">"File Transfer" (Передача файлов).</span><span class="sxs-lookup"><span data-stu-id="3c53d-152">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="3c53d-153">Пример</span><span class="sxs-lookup"><span data-stu-id="3c53d-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3c53d-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c53d-154">Request</span></span>

<span data-ttu-id="3c53d-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c53d-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3c53d-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c53d-156">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c53d-157">C#</span><span class="sxs-lookup"><span data-stu-id="3c53d-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c53d-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c53d-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c53d-159">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3c53d-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3c53d-160">Java</span><span class="sxs-lookup"><span data-stu-id="3c53d-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinesspeertopeeractivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3c53d-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c53d-161">Response</span></span>

<span data-ttu-id="3c53d-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3c53d-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="3c53d-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3c53d-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
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
