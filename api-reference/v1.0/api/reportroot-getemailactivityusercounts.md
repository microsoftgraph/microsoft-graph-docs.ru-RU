---
title: 'reportRoot: getEmailActivityUserCounts'
description: Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: df1e3f67862a39d15363eadd76779ab0aff0da0c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864532"
---
# <a name="reportroot-getemailactivityusercounts"></a><span data-ttu-id="a657d-103">reportRoot: getEmailActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="a657d-103">reportRoot: getEmailActivityUserCounts</span></span>

<span data-ttu-id="a657d-104">Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.</span><span class="sxs-lookup"><span data-stu-id="a657d-104">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span>

> <span data-ttu-id="a657d-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="a657d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="a657d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a657d-106">Permissions</span></span>

<span data-ttu-id="a657d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a657d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a657d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a657d-109">Permission type</span></span>                        | <span data-ttu-id="a657d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a657d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a657d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a657d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a657d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a657d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a657d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a657d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a657d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a657d-114">Not supported.</span></span>                           |
| <span data-ttu-id="a657d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a657d-115">Application</span></span>                            | <span data-ttu-id="a657d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a657d-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="a657d-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a657d-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a657d-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a657d-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a657d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a657d-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a657d-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="a657d-120">Function parameters</span></span>

<span data-ttu-id="a657d-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="a657d-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a657d-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="a657d-122">Parameter</span></span> | <span data-ttu-id="a657d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="a657d-123">Type</span></span>   | <span data-ttu-id="a657d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a657d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a657d-125">period</span><span class="sxs-lookup"><span data-stu-id="a657d-125">period</span></span>    | <span data-ttu-id="a657d-126">string</span><span class="sxs-lookup"><span data-stu-id="a657d-126">string</span></span> | <span data-ttu-id="a657d-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="a657d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a657d-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="a657d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a657d-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="a657d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a657d-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a657d-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a657d-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a657d-131">Request headers</span></span>

| <span data-ttu-id="a657d-132">Имя</span><span class="sxs-lookup"><span data-stu-id="a657d-132">Name</span></span>          | <span data-ttu-id="a657d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a657d-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a657d-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a657d-134">Authorization</span></span> | <span data-ttu-id="a657d-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a657d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a657d-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a657d-137">If-None-Match</span></span> | <span data-ttu-id="a657d-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="a657d-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a657d-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a657d-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a657d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a657d-140">Response</span></span>

<span data-ttu-id="a657d-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="a657d-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a657d-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="a657d-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a657d-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a657d-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a657d-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="a657d-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a657d-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="a657d-145">Report Refresh Date</span></span>
- <span data-ttu-id="a657d-146">Send (отправлено)</span><span class="sxs-lookup"><span data-stu-id="a657d-146">Send</span></span>
- <span data-ttu-id="a657d-147">Receive (получено)</span><span class="sxs-lookup"><span data-stu-id="a657d-147">Receive</span></span>
- <span data-ttu-id="a657d-148">Read (прочитано)</span><span class="sxs-lookup"><span data-stu-id="a657d-148">Read</span></span>
- <span data-ttu-id="a657d-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="a657d-149">Report Date</span></span>
- <span data-ttu-id="a657d-150">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="a657d-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a657d-151">Пример</span><span class="sxs-lookup"><span data-stu-id="a657d-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a657d-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="a657d-152">Request</span></span>

<span data-ttu-id="a657d-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a657d-153">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a657d-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="a657d-154">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a657d-155">C#</span><span class="sxs-lookup"><span data-stu-id="a657d-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a657d-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a657d-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a657d-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a657d-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a657d-158">Java</span><span class="sxs-lookup"><span data-stu-id="a657d-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a657d-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="a657d-159">Response</span></span>

<span data-ttu-id="a657d-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a657d-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="a657d-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="a657d-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
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
