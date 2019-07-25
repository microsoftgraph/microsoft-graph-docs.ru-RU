---
title: 'reportRoot: getMailboxUsageDetail'
description: Получите сведения об использовании почтовых ящиков.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 451be57666719f011ba89992089b54ad16d88f29
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894438"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="fd5c9-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="fd5c9-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="fd5c9-104">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="fd5c9-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="fd5c9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="fd5c9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd5c9-106">Permissions</span></span>

<span data-ttu-id="fd5c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd5c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fd5c9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd5c9-109">Permission type</span></span>                        | <span data-ttu-id="fd5c9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd5c9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fd5c9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd5c9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fd5c9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd5c9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fd5c9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd5c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd5c9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-114">Not supported.</span></span>                           |
| <span data-ttu-id="fd5c9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd5c9-115">Application</span></span>                            | <span data-ttu-id="fd5c9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd5c9-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fd5c9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd5c9-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fd5c9-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd5c9-118">--Http</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fd5c9-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="fd5c9-119">Function parameters</span></span>

<span data-ttu-id="fd5c9-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fd5c9-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="fd5c9-121">Parameter</span></span> | <span data-ttu-id="fd5c9-122">Тип</span><span class="sxs-lookup"><span data-stu-id="fd5c9-122">Type</span></span>   | <span data-ttu-id="fd5c9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fd5c9-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fd5c9-124">period</span><span class="sxs-lookup"><span data-stu-id="fd5c9-124">period</span></span>    | <span data-ttu-id="fd5c9-125">string</span><span class="sxs-lookup"><span data-stu-id="fd5c9-125">string</span></span> | <span data-ttu-id="fd5c9-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fd5c9-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fd5c9-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fd5c9-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="fd5c9-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd5c9-130">Request headers</span></span>

| <span data-ttu-id="fd5c9-131">Имя</span><span class="sxs-lookup"><span data-stu-id="fd5c9-131">Name</span></span>          | <span data-ttu-id="fd5c9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fd5c9-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="fd5c9-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd5c9-133">Authorization</span></span> | <span data-ttu-id="fd5c9-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="fd5c9-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="fd5c9-136">If-None-Match</span></span> | <span data-ttu-id="fd5c9-137">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="fd5c9-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fd5c9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd5c9-139">Response</span></span>

<span data-ttu-id="fd5c9-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fd5c9-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fd5c9-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fd5c9-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="fd5c9-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fd5c9-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="fd5c9-144">Report Refresh Date</span></span>
- <span data-ttu-id="fd5c9-145">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="fd5c9-145">User Principal Name</span></span>
- <span data-ttu-id="fd5c9-146">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="fd5c9-146">Display Name</span></span>
- <span data-ttu-id="fd5c9-147">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="fd5c9-147">Is Deleted</span></span>
- <span data-ttu-id="fd5c9-148">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="fd5c9-148">Deleted Date</span></span>
- <span data-ttu-id="fd5c9-149">Created Date (дата создания)</span><span class="sxs-lookup"><span data-stu-id="fd5c9-149">Created Date</span></span>
- <span data-ttu-id="fd5c9-150">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="fd5c9-150">Last Activity Date</span></span>
- <span data-ttu-id="fd5c9-151">Item Count (количество элементов)</span><span class="sxs-lookup"><span data-stu-id="fd5c9-151">Item Count</span></span>
- <span data-ttu-id="fd5c9-152">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="fd5c9-152">Storage Used (Byte)</span></span>
- <span data-ttu-id="fd5c9-153">Issue Warning Quota (Byte) [объем, при котором выводится предупреждение (байт)]</span><span class="sxs-lookup"><span data-stu-id="fd5c9-153">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="fd5c9-154">Prohibit Send Quota (Byte) [объем, при котором блокируется отправка (байт)]</span><span class="sxs-lookup"><span data-stu-id="fd5c9-154">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="fd5c9-155">Prohibit Send/Receive Quota (Byte) [объем, при котором блокируются отправка и получение (байт)]</span><span class="sxs-lookup"><span data-stu-id="fd5c9-155">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="fd5c9-156">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="fd5c9-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fd5c9-157">Пример</span><span class="sxs-lookup"><span data-stu-id="fd5c9-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fd5c9-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd5c9-158">Request</span></span>

<span data-ttu-id="fd5c9-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fd5c9-160">C#</span><span class="sxs-lookup"><span data-stu-id="fd5c9-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd5c9-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd5c9-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fd5c9-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd5c9-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fd5c9-163">Java</span><span class="sxs-lookup"><span data-stu-id="fd5c9-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fd5c9-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd5c9-164">Response</span></span>

<span data-ttu-id="fd5c9-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="fd5c9-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="fd5c9-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
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
