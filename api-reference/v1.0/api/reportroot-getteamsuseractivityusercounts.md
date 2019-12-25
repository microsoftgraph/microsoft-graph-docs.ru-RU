---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Получение количества пользователей Microsoft Teams по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 14c32dadff08ba8a9b8e2f2796c9e274dd043438
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864231"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="0e838-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="0e838-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="0e838-105">Получение количества пользователей Microsoft Teams по типу действия.</span><span class="sxs-lookup"><span data-stu-id="0e838-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="0e838-106">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="0e838-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e838-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e838-107">Permissions</span></span>

<span data-ttu-id="0e838-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e838-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e838-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e838-110">Permission type</span></span>                        | <span data-ttu-id="0e838-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e838-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0e838-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e838-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e838-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e838-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0e838-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e838-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e838-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e838-115">Not supported.</span></span>                           |
| <span data-ttu-id="0e838-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e838-116">Application</span></span>                            | <span data-ttu-id="0e838-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e838-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="0e838-118">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0e838-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="0e838-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="0e838-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="0e838-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e838-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0e838-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="0e838-121">Function parameters</span></span>

<span data-ttu-id="0e838-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="0e838-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0e838-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="0e838-123">Parameter</span></span> | <span data-ttu-id="0e838-124">Тип</span><span class="sxs-lookup"><span data-stu-id="0e838-124">Type</span></span>   | <span data-ttu-id="0e838-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0e838-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0e838-126">period</span><span class="sxs-lookup"><span data-stu-id="0e838-126">period</span></span>    | <span data-ttu-id="0e838-127">string</span><span class="sxs-lookup"><span data-stu-id="0e838-127">string</span></span> | <span data-ttu-id="0e838-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="0e838-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0e838-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="0e838-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0e838-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="0e838-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0e838-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e838-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0e838-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e838-132">Request headers</span></span>

| <span data-ttu-id="0e838-133">Имя</span><span class="sxs-lookup"><span data-stu-id="0e838-133">Name</span></span>          | <span data-ttu-id="0e838-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0e838-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0e838-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e838-135">Authorization</span></span> | <span data-ttu-id="0e838-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e838-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0e838-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e838-138">Response</span></span>

<span data-ttu-id="0e838-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="0e838-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0e838-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="0e838-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0e838-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0e838-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0e838-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="0e838-142">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="0e838-143">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="0e838-143">Report Refresh Date</span></span>
- <span data-ttu-id="0e838-144">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="0e838-144">Report Date</span></span>
- <span data-ttu-id="0e838-145">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="0e838-145">Team Chat Messages</span></span>
- <span data-ttu-id="0e838-146">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="0e838-146">Private Chat Messages</span></span>
- <span data-ttu-id="0e838-147">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="0e838-147">Calls</span></span>
- <span data-ttu-id="0e838-148">Meetings (Собрания);</span><span class="sxs-lookup"><span data-stu-id="0e838-148">Meetings</span></span>
- <span data-ttu-id="0e838-149">Other Actions (Другие действия);</span><span class="sxs-lookup"><span data-stu-id="0e838-149">Other Actions</span></span>
- <span data-ttu-id="0e838-150">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="0e838-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0e838-151">Пример</span><span class="sxs-lookup"><span data-stu-id="0e838-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0e838-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e838-152">Request</span></span>

<span data-ttu-id="0e838-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e838-153">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0e838-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e838-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0e838-155">C#</span><span class="sxs-lookup"><span data-stu-id="0e838-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e838-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e838-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0e838-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e838-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0e838-158">Java</span><span class="sxs-lookup"><span data-stu-id="0e838-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0e838-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e838-159">Response</span></span>

<span data-ttu-id="0e838-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0e838-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="0e838-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="0e838-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
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
