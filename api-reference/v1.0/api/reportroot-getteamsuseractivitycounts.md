---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Получение количества действий в Microsoft Teams по каждому типу. К типам действий относятся сообщения в чатах групп, сообщения в приватных чатах, звонки и собрания.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c7b03739d3f9c7d6e4763617e201d6a0598abbe1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510062"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="84713-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="84713-104">reportRoot: getTeamsUserActivityCounts</span></span>

<span data-ttu-id="84713-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84713-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="84713-106">Получение количества действий в Microsoft Teams по каждому типу.</span><span class="sxs-lookup"><span data-stu-id="84713-106">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="84713-107">К типам действий относятся сообщения в чатах групп, сообщения в приватных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="84713-107">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="84713-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84713-108">Permissions</span></span>

<span data-ttu-id="84713-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84713-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84713-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84713-111">Permission type</span></span>                        | <span data-ttu-id="84713-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84713-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="84713-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84713-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="84713-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="84713-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="84713-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84713-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84713-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84713-116">Not supported.</span></span>                           |
| <span data-ttu-id="84713-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84713-117">Application</span></span>                            | <span data-ttu-id="84713-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="84713-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="84713-119">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84713-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="84713-120">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="84713-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="84713-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84713-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="84713-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="84713-122">Function parameters</span></span>

<span data-ttu-id="84713-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="84713-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="84713-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="84713-124">Parameter</span></span> | <span data-ttu-id="84713-125">Тип</span><span class="sxs-lookup"><span data-stu-id="84713-125">Type</span></span>   | <span data-ttu-id="84713-126">Описание</span><span class="sxs-lookup"><span data-stu-id="84713-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="84713-127">period</span><span class="sxs-lookup"><span data-stu-id="84713-127">period</span></span>    | <span data-ttu-id="84713-128">string</span><span class="sxs-lookup"><span data-stu-id="84713-128">string</span></span> | <span data-ttu-id="84713-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="84713-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="84713-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="84713-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="84713-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="84713-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="84713-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84713-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="84713-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84713-133">Request headers</span></span>

| <span data-ttu-id="84713-134">Имя</span><span class="sxs-lookup"><span data-stu-id="84713-134">Name</span></span>          | <span data-ttu-id="84713-135">Описание</span><span class="sxs-lookup"><span data-stu-id="84713-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="84713-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84713-136">Authorization</span></span> | <span data-ttu-id="84713-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84713-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="84713-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="84713-139">Response</span></span>

<span data-ttu-id="84713-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="84713-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="84713-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="84713-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="84713-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="84713-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="84713-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="84713-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="84713-144">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="84713-144">Report Refresh Date</span></span>
- <span data-ttu-id="84713-145">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="84713-145">Report Date</span></span>
- <span data-ttu-id="84713-146">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="84713-146">Team Chat Messages</span></span>
- <span data-ttu-id="84713-147">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="84713-147">Private Chat Messages</span></span>
- <span data-ttu-id="84713-148">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="84713-148">Calls</span></span>
- <span data-ttu-id="84713-149">Meetings (собрания);</span><span class="sxs-lookup"><span data-stu-id="84713-149">Meetings</span></span>
- <span data-ttu-id="84713-150">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="84713-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="84713-151">Пример</span><span class="sxs-lookup"><span data-stu-id="84713-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="84713-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="84713-152">Request</span></span>

<span data-ttu-id="84713-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84713-153">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="84713-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="84713-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="84713-155">C#</span><span class="sxs-lookup"><span data-stu-id="84713-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84713-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84713-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84713-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84713-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84713-158">Java</span><span class="sxs-lookup"><span data-stu-id="84713-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="84713-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="84713-159">Response</span></span>

<span data-ttu-id="84713-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="84713-160">The following is an example of the response.</span></span>

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
<span data-ttu-id="84713-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="84713-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
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
