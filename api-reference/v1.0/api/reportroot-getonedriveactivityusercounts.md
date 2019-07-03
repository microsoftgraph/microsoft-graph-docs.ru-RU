---
title: 'reportRoot: getOneDriveActivityUserCounts'
description: Отслеживайте, как меняется количество активных пользователей OneDrive.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3e9a6ba9b8774cbc07a1a0a56be075a5f22f6d9e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444402"
---
# <a name="reportroot-getonedriveactivityusercounts"></a><span data-ttu-id="90c74-103">reportRoot: getOneDriveActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="90c74-103">reportRoot: getOneDriveActivityUserCounts</span></span>

<span data-ttu-id="90c74-104">Отслеживайте, как меняется количество активных пользователей OneDrive.</span><span class="sxs-lookup"><span data-stu-id="90c74-104">Get the trend in the number of active OneDrive users.</span></span>

> <span data-ttu-id="90c74-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="90c74-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="90c74-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90c74-106">Permissions</span></span>

<span data-ttu-id="90c74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90c74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90c74-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90c74-109">Permission type</span></span>                        | <span data-ttu-id="90c74-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90c74-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="90c74-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90c74-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="90c74-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="90c74-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="90c74-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90c74-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90c74-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90c74-114">Not supported.</span></span>                           |
| <span data-ttu-id="90c74-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90c74-115">Application</span></span>                            | <span data-ttu-id="90c74-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="90c74-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="90c74-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90c74-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="90c74-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="90c74-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="90c74-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="90c74-119">Function parameters</span></span>

<span data-ttu-id="90c74-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="90c74-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="90c74-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="90c74-121">Parameter</span></span> | <span data-ttu-id="90c74-122">Тип</span><span class="sxs-lookup"><span data-stu-id="90c74-122">Type</span></span>   | <span data-ttu-id="90c74-123">Описание</span><span class="sxs-lookup"><span data-stu-id="90c74-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="90c74-124">period</span><span class="sxs-lookup"><span data-stu-id="90c74-124">period</span></span>    | <span data-ttu-id="90c74-125">string</span><span class="sxs-lookup"><span data-stu-id="90c74-125">string</span></span> | <span data-ttu-id="90c74-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="90c74-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="90c74-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="90c74-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="90c74-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="90c74-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="90c74-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90c74-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="90c74-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90c74-130">Request headers</span></span>

| <span data-ttu-id="90c74-131">Имя</span><span class="sxs-lookup"><span data-stu-id="90c74-131">Name</span></span>          | <span data-ttu-id="90c74-132">Описание</span><span class="sxs-lookup"><span data-stu-id="90c74-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="90c74-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90c74-133">Authorization</span></span> | <span data-ttu-id="90c74-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90c74-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="90c74-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="90c74-136">If-None-Match</span></span> | <span data-ttu-id="90c74-137">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="90c74-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="90c74-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="90c74-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="90c74-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="90c74-139">Response</span></span>

<span data-ttu-id="90c74-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="90c74-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="90c74-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="90c74-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="90c74-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="90c74-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="90c74-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="90c74-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="90c74-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="90c74-144">Report Refresh Date</span></span>
- <span data-ttu-id="90c74-145">"Viewed Or Edited" (Просмотрены или изменены);</span><span class="sxs-lookup"><span data-stu-id="90c74-145">Viewed Or Edited</span></span>
- <span data-ttu-id="90c74-146">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="90c74-146">Synced</span></span>
- <span data-ttu-id="90c74-147">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="90c74-147">Shared Internally</span></span>
- <span data-ttu-id="90c74-148">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="90c74-148">Shared Externally</span></span>
- <span data-ttu-id="90c74-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="90c74-149">Report Date</span></span>
- <span data-ttu-id="90c74-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="90c74-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="90c74-151">Пример</span><span class="sxs-lookup"><span data-stu-id="90c74-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="90c74-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="90c74-152">Request</span></span>

<span data-ttu-id="90c74-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90c74-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="90c74-154">C#</span><span class="sxs-lookup"><span data-stu-id="90c74-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90c74-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="90c74-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="90c74-156">Цель — C</span><span class="sxs-lookup"><span data-stu-id="90c74-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="90c74-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="90c74-157">Response</span></span>

<span data-ttu-id="90c74-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90c74-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="90c74-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="90c74-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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
