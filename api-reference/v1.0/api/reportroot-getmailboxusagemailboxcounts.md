---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период. Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0d7736edaccdf976c8adda3816dcc5c68bb2e74c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728246"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="35274-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="35274-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="35274-105">Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="35274-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="35274-106">Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.</span><span class="sxs-lookup"><span data-stu-id="35274-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="35274-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="35274-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="35274-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35274-108">Permissions</span></span>

<span data-ttu-id="35274-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35274-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35274-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35274-111">Permission type</span></span>                        | <span data-ttu-id="35274-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35274-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="35274-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35274-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="35274-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="35274-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="35274-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35274-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35274-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35274-116">Not supported.</span></span>                           |
| <span data-ttu-id="35274-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35274-117">Application</span></span>                            | <span data-ttu-id="35274-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="35274-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="35274-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35274-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="35274-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="35274-120">Function parameters</span></span>

<span data-ttu-id="35274-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="35274-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="35274-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="35274-122">Parameter</span></span> | <span data-ttu-id="35274-123">Тип</span><span class="sxs-lookup"><span data-stu-id="35274-123">Type</span></span>   | <span data-ttu-id="35274-124">Описание</span><span class="sxs-lookup"><span data-stu-id="35274-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="35274-125">period</span><span class="sxs-lookup"><span data-stu-id="35274-125">period</span></span>    | <span data-ttu-id="35274-126">string</span><span class="sxs-lookup"><span data-stu-id="35274-126">string</span></span> | <span data-ttu-id="35274-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="35274-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="35274-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="35274-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="35274-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="35274-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="35274-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35274-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="35274-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35274-131">Request headers</span></span>

| <span data-ttu-id="35274-132">Имя</span><span class="sxs-lookup"><span data-stu-id="35274-132">Name</span></span>          | <span data-ttu-id="35274-133">Описание</span><span class="sxs-lookup"><span data-stu-id="35274-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="35274-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35274-134">Authorization</span></span> | <span data-ttu-id="35274-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35274-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="35274-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="35274-137">If-None-Match</span></span> | <span data-ttu-id="35274-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="35274-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="35274-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="35274-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="35274-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="35274-140">Response</span></span>

<span data-ttu-id="35274-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="35274-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="35274-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="35274-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="35274-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="35274-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="35274-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="35274-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="35274-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="35274-145">Report Refresh Date</span></span>
- <span data-ttu-id="35274-146">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="35274-146">Total</span></span>
- <span data-ttu-id="35274-147">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="35274-147">Active</span></span>
- <span data-ttu-id="35274-148">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="35274-148">Report Date</span></span>
- <span data-ttu-id="35274-149">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="35274-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="35274-150">Пример</span><span class="sxs-lookup"><span data-stu-id="35274-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="35274-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="35274-151">Request</span></span>

<span data-ttu-id="35274-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35274-152">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="35274-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="35274-153">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="35274-154">C#</span><span class="sxs-lookup"><span data-stu-id="35274-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagemailboxcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35274-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35274-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagemailboxcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="35274-156">Цель — C</span><span class="sxs-lookup"><span data-stu-id="35274-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagemailboxcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="35274-157">Java</span><span class="sxs-lookup"><span data-stu-id="35274-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagemailboxcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="35274-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="35274-158">Response</span></span>

<span data-ttu-id="35274-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="35274-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="35274-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="35274-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
