---
title: 'reportRoot: getSkypeForBusinessActivityCounts'
description: Отслеживайте, как меняется количество организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e4c8e021f292b805f8ffb700679f49e59acc8d5d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510188"
---
# <a name="reportroot-getskypeforbusinessactivitycounts"></a><span data-ttu-id="643dd-104">reportRoot: getSkypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="643dd-104">reportRoot: getSkypeForBusinessActivityCounts</span></span>

<span data-ttu-id="643dd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="643dd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="643dd-106">Отслеживайте, как меняется количество организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="643dd-106">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="643dd-107">Отчет также включает количество одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="643dd-107">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="643dd-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="643dd-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="643dd-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="643dd-109">Permissions</span></span>

<span data-ttu-id="643dd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="643dd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="643dd-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="643dd-112">Permission type</span></span>                        | <span data-ttu-id="643dd-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="643dd-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="643dd-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="643dd-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="643dd-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="643dd-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="643dd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="643dd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="643dd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="643dd-117">Not supported.</span></span>                           |
| <span data-ttu-id="643dd-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="643dd-118">Application</span></span>                            | <span data-ttu-id="643dd-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="643dd-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="643dd-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="643dd-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="643dd-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="643dd-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="643dd-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="643dd-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="643dd-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="643dd-123">Function parameters</span></span>

<span data-ttu-id="643dd-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="643dd-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="643dd-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="643dd-125">Parameter</span></span> | <span data-ttu-id="643dd-126">Тип</span><span class="sxs-lookup"><span data-stu-id="643dd-126">Type</span></span>   | <span data-ttu-id="643dd-127">Описание</span><span class="sxs-lookup"><span data-stu-id="643dd-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="643dd-128">period</span><span class="sxs-lookup"><span data-stu-id="643dd-128">period</span></span>    | <span data-ttu-id="643dd-129">string</span><span class="sxs-lookup"><span data-stu-id="643dd-129">string</span></span> | <span data-ttu-id="643dd-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="643dd-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="643dd-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="643dd-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="643dd-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="643dd-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="643dd-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="643dd-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="643dd-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="643dd-134">Request headers</span></span>

| <span data-ttu-id="643dd-135">Имя</span><span class="sxs-lookup"><span data-stu-id="643dd-135">Name</span></span>          | <span data-ttu-id="643dd-136">Описание</span><span class="sxs-lookup"><span data-stu-id="643dd-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="643dd-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="643dd-137">Authorization</span></span> | <span data-ttu-id="643dd-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="643dd-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="643dd-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="643dd-140">If-None-Match</span></span> | <span data-ttu-id="643dd-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="643dd-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="643dd-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="643dd-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="643dd-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="643dd-143">Response</span></span>

<span data-ttu-id="643dd-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="643dd-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="643dd-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="643dd-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="643dd-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="643dd-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="643dd-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="643dd-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="643dd-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="643dd-148">Report Refresh Date</span></span>
- <span data-ttu-id="643dd-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="643dd-149">Report Date</span></span>
- <span data-ttu-id="643dd-150">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="643dd-150">Report Period</span></span>
- <span data-ttu-id="643dd-151">"Peer-to-peer" (Одноранговый сеанс);</span><span class="sxs-lookup"><span data-stu-id="643dd-151">Peer-to-peer</span></span>
- <span data-ttu-id="643dd-152">"Organized" (Организаторы);</span><span class="sxs-lookup"><span data-stu-id="643dd-152">Organized</span></span>
- <span data-ttu-id="643dd-153">"Participated" (Участники).</span><span class="sxs-lookup"><span data-stu-id="643dd-153">Participated</span></span>

## <a name="example"></a><span data-ttu-id="643dd-154">Пример</span><span class="sxs-lookup"><span data-stu-id="643dd-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="643dd-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="643dd-155">Request</span></span>

<span data-ttu-id="643dd-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="643dd-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="643dd-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="643dd-157">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivitycounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="643dd-158">C#</span><span class="sxs-lookup"><span data-stu-id="643dd-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="643dd-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="643dd-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="643dd-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="643dd-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="643dd-161">Java</span><span class="sxs-lookup"><span data-stu-id="643dd-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="643dd-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="643dd-162">Response</span></span>

<span data-ttu-id="643dd-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="643dd-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="643dd-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="643dd-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
