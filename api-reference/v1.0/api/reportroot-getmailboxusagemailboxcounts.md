---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период. Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 856a55f480973d82a7c1b223dedfd17aa8d117f1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864469"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="53dca-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="53dca-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="53dca-105">Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="53dca-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="53dca-106">Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.</span><span class="sxs-lookup"><span data-stu-id="53dca-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="53dca-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="53dca-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="53dca-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53dca-108">Permissions</span></span>

<span data-ttu-id="53dca-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53dca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53dca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53dca-111">Permission type</span></span>                        | <span data-ttu-id="53dca-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53dca-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="53dca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53dca-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="53dca-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="53dca-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="53dca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53dca-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53dca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53dca-116">Not supported.</span></span>                           |
| <span data-ttu-id="53dca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53dca-117">Application</span></span>                            | <span data-ttu-id="53dca-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="53dca-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="53dca-119">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="53dca-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="53dca-120">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="53dca-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="53dca-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53dca-121">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="53dca-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="53dca-122">Function parameters</span></span>

<span data-ttu-id="53dca-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="53dca-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="53dca-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="53dca-124">Parameter</span></span> | <span data-ttu-id="53dca-125">Тип</span><span class="sxs-lookup"><span data-stu-id="53dca-125">Type</span></span>   | <span data-ttu-id="53dca-126">Описание</span><span class="sxs-lookup"><span data-stu-id="53dca-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="53dca-127">period</span><span class="sxs-lookup"><span data-stu-id="53dca-127">period</span></span>    | <span data-ttu-id="53dca-128">string</span><span class="sxs-lookup"><span data-stu-id="53dca-128">string</span></span> | <span data-ttu-id="53dca-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="53dca-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="53dca-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="53dca-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="53dca-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="53dca-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="53dca-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53dca-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="53dca-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53dca-133">Request headers</span></span>

| <span data-ttu-id="53dca-134">Имя</span><span class="sxs-lookup"><span data-stu-id="53dca-134">Name</span></span>          | <span data-ttu-id="53dca-135">Описание</span><span class="sxs-lookup"><span data-stu-id="53dca-135">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="53dca-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53dca-136">Authorization</span></span> | <span data-ttu-id="53dca-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53dca-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="53dca-139">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="53dca-139">If-None-Match</span></span> | <span data-ttu-id="53dca-140">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="53dca-140">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="53dca-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="53dca-141">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="53dca-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="53dca-142">Response</span></span>

<span data-ttu-id="53dca-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="53dca-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="53dca-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="53dca-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="53dca-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="53dca-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="53dca-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="53dca-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="53dca-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="53dca-147">Report Refresh Date</span></span>
- <span data-ttu-id="53dca-148">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="53dca-148">Total</span></span>
- <span data-ttu-id="53dca-149">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="53dca-149">Active</span></span>
- <span data-ttu-id="53dca-150">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="53dca-150">Report Date</span></span>
- <span data-ttu-id="53dca-151">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="53dca-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="53dca-152">Пример</span><span class="sxs-lookup"><span data-stu-id="53dca-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="53dca-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="53dca-153">Request</span></span>

<span data-ttu-id="53dca-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53dca-154">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="53dca-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="53dca-155">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="53dca-156">C#</span><span class="sxs-lookup"><span data-stu-id="53dca-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagemailboxcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53dca-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53dca-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagemailboxcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53dca-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53dca-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagemailboxcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="53dca-159">Java</span><span class="sxs-lookup"><span data-stu-id="53dca-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagemailboxcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="53dca-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="53dca-160">Response</span></span>

<span data-ttu-id="53dca-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53dca-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="53dca-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="53dca-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
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
