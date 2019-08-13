---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Отслеживайте, как меняется количество активных пользователей. Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7eabd3b86f83283005918670981839c04098318b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321848"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="00be0-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="00be0-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="00be0-105">Отслеживайте, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="00be0-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="00be0-106">Пользователь считается активным, если он сохранил, синхронизировал, изменил или отправил файл или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="00be0-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="00be0-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="00be0-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="00be0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00be0-108">Permissions</span></span>

<span data-ttu-id="00be0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00be0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00be0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00be0-111">Permission type</span></span>                        | <span data-ttu-id="00be0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00be0-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="00be0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00be0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="00be0-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="00be0-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="00be0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00be0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00be0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00be0-116">Not supported.</span></span>                           |
| <span data-ttu-id="00be0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00be0-117">Application</span></span>                            | <span data-ttu-id="00be0-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="00be0-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="00be0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00be0-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="00be0-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="00be0-120">Function parameters</span></span>

<span data-ttu-id="00be0-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="00be0-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="00be0-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="00be0-122">Parameter</span></span> | <span data-ttu-id="00be0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="00be0-123">Type</span></span>   | <span data-ttu-id="00be0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="00be0-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="00be0-125">period</span><span class="sxs-lookup"><span data-stu-id="00be0-125">period</span></span>    | <span data-ttu-id="00be0-126">string</span><span class="sxs-lookup"><span data-stu-id="00be0-126">string</span></span> | <span data-ttu-id="00be0-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="00be0-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="00be0-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="00be0-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="00be0-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="00be0-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="00be0-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00be0-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="00be0-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00be0-131">Request headers</span></span>

| <span data-ttu-id="00be0-132">Имя</span><span class="sxs-lookup"><span data-stu-id="00be0-132">Name</span></span>          | <span data-ttu-id="00be0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="00be0-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="00be0-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00be0-134">Authorization</span></span> | <span data-ttu-id="00be0-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00be0-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="00be0-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="00be0-137">If-None-Match</span></span> | <span data-ttu-id="00be0-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="00be0-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="00be0-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="00be0-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="00be0-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="00be0-140">Response</span></span>

<span data-ttu-id="00be0-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="00be0-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="00be0-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="00be0-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="00be0-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="00be0-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="00be0-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="00be0-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="00be0-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="00be0-145">Report Refresh Date</span></span>
- <span data-ttu-id="00be0-146">Visited Page (посетило страницу)</span><span class="sxs-lookup"><span data-stu-id="00be0-146">Visited Page</span></span>
- <span data-ttu-id="00be0-147">Viewed Or Edited (просмотрело или изменило)</span><span class="sxs-lookup"><span data-stu-id="00be0-147">Viewed Or Edited</span></span>
- <span data-ttu-id="00be0-148">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="00be0-148">Synced</span></span>
- <span data-ttu-id="00be0-149">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="00be0-149">Shared Internally</span></span>
- <span data-ttu-id="00be0-150">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="00be0-150">Shared Externally</span></span>
- <span data-ttu-id="00be0-151">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="00be0-151">Report Date</span></span>
- <span data-ttu-id="00be0-152">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="00be0-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="00be0-153">Пример</span><span class="sxs-lookup"><span data-stu-id="00be0-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="00be0-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="00be0-154">Request</span></span>

<span data-ttu-id="00be0-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00be0-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="00be0-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="00be0-156">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="00be0-157">C#</span><span class="sxs-lookup"><span data-stu-id="00be0-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00be0-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00be0-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00be0-159">Цель — C</span><span class="sxs-lookup"><span data-stu-id="00be0-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="00be0-160">Java</span><span class="sxs-lookup"><span data-stu-id="00be0-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="00be0-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="00be0-161">Response</span></span>

<span data-ttu-id="00be0-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00be0-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="00be0-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="00be0-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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
