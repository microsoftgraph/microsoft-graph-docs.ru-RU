---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Отслеживайте, как меняется количество активных пользователей. Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 6ea23bfe190b40394cf3c41efc2bd5d4c758f094
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865393"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="8332c-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8332c-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="8332c-105">Отслеживайте, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="8332c-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="8332c-106">Пользователь считается активным, если он сохранил, синхронизировал, изменил или отправил файл или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="8332c-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="8332c-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="8332c-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="8332c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8332c-108">Permissions</span></span>

<span data-ttu-id="8332c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8332c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8332c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8332c-111">Permission type</span></span>                        | <span data-ttu-id="8332c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8332c-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8332c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8332c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8332c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8332c-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8332c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8332c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8332c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8332c-116">Not supported.</span></span>                           |
| <span data-ttu-id="8332c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8332c-117">Application</span></span>                            | <span data-ttu-id="8332c-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8332c-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="8332c-119">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8332c-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="8332c-120">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="8332c-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="8332c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8332c-121">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8332c-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="8332c-122">Function parameters</span></span>

<span data-ttu-id="8332c-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="8332c-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8332c-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="8332c-124">Parameter</span></span> | <span data-ttu-id="8332c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="8332c-125">Type</span></span>   | <span data-ttu-id="8332c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8332c-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8332c-127">period</span><span class="sxs-lookup"><span data-stu-id="8332c-127">period</span></span>    | <span data-ttu-id="8332c-128">string</span><span class="sxs-lookup"><span data-stu-id="8332c-128">string</span></span> | <span data-ttu-id="8332c-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="8332c-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8332c-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="8332c-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8332c-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="8332c-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8332c-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8332c-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8332c-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8332c-133">Request headers</span></span>

| <span data-ttu-id="8332c-134">Имя</span><span class="sxs-lookup"><span data-stu-id="8332c-134">Name</span></span>          | <span data-ttu-id="8332c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="8332c-135">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8332c-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8332c-136">Authorization</span></span> | <span data-ttu-id="8332c-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8332c-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8332c-139">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8332c-139">If-None-Match</span></span> | <span data-ttu-id="8332c-140">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="8332c-140">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8332c-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="8332c-141">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8332c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8332c-142">Response</span></span>

<span data-ttu-id="8332c-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="8332c-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8332c-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="8332c-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8332c-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8332c-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8332c-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="8332c-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8332c-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="8332c-147">Report Refresh Date</span></span>
- <span data-ttu-id="8332c-148">Visited Page (посетило страницу)</span><span class="sxs-lookup"><span data-stu-id="8332c-148">Visited Page</span></span>
- <span data-ttu-id="8332c-149">Viewed Or Edited (просмотрело или изменило)</span><span class="sxs-lookup"><span data-stu-id="8332c-149">Viewed Or Edited</span></span>
- <span data-ttu-id="8332c-150">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="8332c-150">Synced</span></span>
- <span data-ttu-id="8332c-151">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="8332c-151">Shared Internally</span></span>
- <span data-ttu-id="8332c-152">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="8332c-152">Shared Externally</span></span>
- <span data-ttu-id="8332c-153">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="8332c-153">Report Date</span></span>
- <span data-ttu-id="8332c-154">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="8332c-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="8332c-155">Пример</span><span class="sxs-lookup"><span data-stu-id="8332c-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8332c-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="8332c-156">Request</span></span>

<span data-ttu-id="8332c-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8332c-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8332c-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="8332c-158">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8332c-159">C#</span><span class="sxs-lookup"><span data-stu-id="8332c-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8332c-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8332c-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8332c-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8332c-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8332c-162">Java</span><span class="sxs-lookup"><span data-stu-id="8332c-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8332c-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="8332c-163">Response</span></span>

<span data-ttu-id="8332c-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8332c-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="8332c-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="8332c-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
