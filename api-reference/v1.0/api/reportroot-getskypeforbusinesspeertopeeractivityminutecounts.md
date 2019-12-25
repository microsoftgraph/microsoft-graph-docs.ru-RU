---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов (аудио и видео).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 59bba2b4b35524670999297677f6d59b4fc55877
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865260"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="e9619-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="e9619-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

<span data-ttu-id="e9619-105">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов</span><span class="sxs-lookup"><span data-stu-id="e9619-105">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="e9619-106">(аудио и видео).</span><span class="sxs-lookup"><span data-stu-id="e9619-106">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="e9619-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="e9619-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9619-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9619-108">Permissions</span></span>

<span data-ttu-id="e9619-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9619-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9619-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9619-111">Permission type</span></span>                        | <span data-ttu-id="e9619-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9619-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e9619-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9619-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9619-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9619-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e9619-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9619-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9619-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9619-116">Not supported.</span></span>                           |
| <span data-ttu-id="e9619-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9619-117">Application</span></span>                            | <span data-ttu-id="e9619-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9619-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="e9619-119">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e9619-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e9619-120">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="e9619-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e9619-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9619-121">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e9619-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="e9619-122">Function parameters</span></span>

<span data-ttu-id="e9619-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="e9619-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e9619-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="e9619-124">Parameter</span></span> | <span data-ttu-id="e9619-125">Тип</span><span class="sxs-lookup"><span data-stu-id="e9619-125">Type</span></span>   | <span data-ttu-id="e9619-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e9619-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e9619-127">period</span><span class="sxs-lookup"><span data-stu-id="e9619-127">period</span></span>    | <span data-ttu-id="e9619-128">string</span><span class="sxs-lookup"><span data-stu-id="e9619-128">string</span></span> | <span data-ttu-id="e9619-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="e9619-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e9619-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="e9619-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e9619-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="e9619-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e9619-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9619-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e9619-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9619-133">Request headers</span></span>

| <span data-ttu-id="e9619-134">Имя</span><span class="sxs-lookup"><span data-stu-id="e9619-134">Name</span></span>          | <span data-ttu-id="e9619-135">Описание</span><span class="sxs-lookup"><span data-stu-id="e9619-135">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e9619-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9619-136">Authorization</span></span> | <span data-ttu-id="e9619-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9619-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e9619-139">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e9619-139">If-None-Match</span></span> | <span data-ttu-id="e9619-140">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="e9619-140">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e9619-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e9619-141">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e9619-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9619-142">Response</span></span>

<span data-ttu-id="e9619-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="e9619-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e9619-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="e9619-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e9619-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e9619-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e9619-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="e9619-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e9619-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="e9619-147">Report Refresh Date</span></span>
- <span data-ttu-id="e9619-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="e9619-148">Report Date</span></span>
- <span data-ttu-id="e9619-149">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="e9619-149">Report Period</span></span>
- <span data-ttu-id="e9619-150">Audio (аудио)</span><span class="sxs-lookup"><span data-stu-id="e9619-150">Audio</span></span>
- <span data-ttu-id="e9619-151">Video (видео)</span><span class="sxs-lookup"><span data-stu-id="e9619-151">Video</span></span>

## <a name="example"></a><span data-ttu-id="e9619-152">Пример</span><span class="sxs-lookup"><span data-stu-id="e9619-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e9619-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9619-153">Request</span></span>

<span data-ttu-id="e9619-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9619-154">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e9619-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9619-155">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e9619-156">C#</span><span class="sxs-lookup"><span data-stu-id="e9619-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9619-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9619-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e9619-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9619-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e9619-159">Java</span><span class="sxs-lookup"><span data-stu-id="e9619-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9619-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9619-160">Response</span></span>

<span data-ttu-id="e9619-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9619-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="e9619-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="e9619-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
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
