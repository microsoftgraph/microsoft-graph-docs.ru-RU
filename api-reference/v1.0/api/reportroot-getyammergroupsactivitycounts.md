---
title: 'reportRoot: getYammerGroupsActivityCounts'
description: Узнайте, сколько сообщений Yammer было опубликовано, прочитано и оценено в группах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 05d1788352f52ae4f902088b91b385934fcf1ac7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509999"
---
# <a name="reportroot-getyammergroupsactivitycounts"></a><span data-ttu-id="4890c-103">reportRoot: getYammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4890c-103">reportRoot: getYammerGroupsActivityCounts</span></span>

<span data-ttu-id="4890c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4890c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4890c-105">Узнайте, сколько сообщений Yammer было опубликовано, прочитано и оценено в группах.</span><span class="sxs-lookup"><span data-stu-id="4890c-105">Get the number of Yammer messages posted, read, and liked in groups.</span></span>

> <span data-ttu-id="4890c-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в группах Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="4890c-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="4890c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4890c-107">Permissions</span></span>

<span data-ttu-id="4890c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4890c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4890c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4890c-110">Permission type</span></span>                        | <span data-ttu-id="4890c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4890c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4890c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4890c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4890c-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4890c-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4890c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4890c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4890c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4890c-115">Not supported.</span></span>                           |
| <span data-ttu-id="4890c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4890c-116">Application</span></span>                            | <span data-ttu-id="4890c-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4890c-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="4890c-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4890c-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="4890c-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="4890c-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="4890c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4890c-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4890c-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4890c-121">Function parameters</span></span>

<span data-ttu-id="4890c-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4890c-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4890c-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="4890c-123">Parameter</span></span> | <span data-ttu-id="4890c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="4890c-124">Type</span></span>   | <span data-ttu-id="4890c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4890c-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4890c-126">period</span><span class="sxs-lookup"><span data-stu-id="4890c-126">period</span></span>    | <span data-ttu-id="4890c-127">string</span><span class="sxs-lookup"><span data-stu-id="4890c-127">string</span></span> | <span data-ttu-id="4890c-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4890c-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4890c-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4890c-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4890c-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4890c-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4890c-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4890c-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4890c-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4890c-132">Request headers</span></span>

| <span data-ttu-id="4890c-133">Имя</span><span class="sxs-lookup"><span data-stu-id="4890c-133">Name</span></span>          | <span data-ttu-id="4890c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4890c-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4890c-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4890c-135">Authorization</span></span> | <span data-ttu-id="4890c-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4890c-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4890c-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4890c-138">If-None-Match</span></span> | <span data-ttu-id="4890c-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="4890c-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4890c-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4890c-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4890c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4890c-141">Response</span></span>

<span data-ttu-id="4890c-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4890c-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4890c-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4890c-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4890c-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4890c-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4890c-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4890c-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4890c-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4890c-146">Report Refresh Date</span></span>
- <span data-ttu-id="4890c-147">"Liked" (Понравилось);</span><span class="sxs-lookup"><span data-stu-id="4890c-147">Liked</span></span>
- <span data-ttu-id="4890c-148">"Posted" (Опубликовано);</span><span class="sxs-lookup"><span data-stu-id="4890c-148">Posted</span></span>
- <span data-ttu-id="4890c-149">"Read" (Чтение);</span><span class="sxs-lookup"><span data-stu-id="4890c-149">Read</span></span>
- <span data-ttu-id="4890c-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="4890c-150">Report Date</span></span>
- <span data-ttu-id="4890c-151">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="4890c-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4890c-152">Пример</span><span class="sxs-lookup"><span data-stu-id="4890c-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4890c-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="4890c-153">Request</span></span>

<span data-ttu-id="4890c-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4890c-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4890c-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="4890c-155">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivitycounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="4890c-156">C#</span><span class="sxs-lookup"><span data-stu-id="4890c-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4890c-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4890c-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4890c-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4890c-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4890c-159">Java</span><span class="sxs-lookup"><span data-stu-id="4890c-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammergroupsactivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4890c-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="4890c-160">Response</span></span>

<span data-ttu-id="4890c-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4890c-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="4890c-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4890c-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
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
