---
title: 'reportRoot: getMailboxUsageDetail'
description: Получите сведения об использовании почтовых ящиков.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c7b29395486962d8387ffb438465c6f63adf9042
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268798"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="38f70-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="38f70-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="38f70-104">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="38f70-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="38f70-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="38f70-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="38f70-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38f70-106">Permissions</span></span>

<span data-ttu-id="38f70-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38f70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38f70-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38f70-109">Permission type</span></span>                        | <span data-ttu-id="38f70-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38f70-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="38f70-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38f70-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="38f70-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38f70-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="38f70-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38f70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38f70-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38f70-114">Not supported.</span></span>                           |
| <span data-ttu-id="38f70-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38f70-115">Application</span></span>                            | <span data-ttu-id="38f70-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38f70-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="38f70-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38f70-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="38f70-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="38f70-118">Function parameters</span></span>

<span data-ttu-id="38f70-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="38f70-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="38f70-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="38f70-120">Parameter</span></span> | <span data-ttu-id="38f70-121">Тип</span><span class="sxs-lookup"><span data-stu-id="38f70-121">Type</span></span>   | <span data-ttu-id="38f70-122">Описание</span><span class="sxs-lookup"><span data-stu-id="38f70-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="38f70-123">period</span><span class="sxs-lookup"><span data-stu-id="38f70-123">period</span></span>    | <span data-ttu-id="38f70-124">string</span><span class="sxs-lookup"><span data-stu-id="38f70-124">string</span></span> | <span data-ttu-id="38f70-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="38f70-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="38f70-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="38f70-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="38f70-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="38f70-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="38f70-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38f70-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="38f70-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38f70-129">Request headers</span></span>

| <span data-ttu-id="38f70-130">Имя</span><span class="sxs-lookup"><span data-stu-id="38f70-130">Name</span></span>          | <span data-ttu-id="38f70-131">Описание</span><span class="sxs-lookup"><span data-stu-id="38f70-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="38f70-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38f70-132">Authorization</span></span> | <span data-ttu-id="38f70-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38f70-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="38f70-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="38f70-135">If-None-Match</span></span> | <span data-ttu-id="38f70-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="38f70-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="38f70-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="38f70-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="38f70-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="38f70-138">Response</span></span>

<span data-ttu-id="38f70-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="38f70-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="38f70-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="38f70-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="38f70-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="38f70-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="38f70-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="38f70-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="38f70-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="38f70-143">Report Refresh Date</span></span>
- <span data-ttu-id="38f70-144">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="38f70-144">User Principal Name</span></span>
- <span data-ttu-id="38f70-145">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="38f70-145">Display Name</span></span>
- <span data-ttu-id="38f70-146">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="38f70-146">Is Deleted</span></span>
- <span data-ttu-id="38f70-147">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="38f70-147">Deleted Date</span></span>
- <span data-ttu-id="38f70-148">Created Date (дата создания)</span><span class="sxs-lookup"><span data-stu-id="38f70-148">Created Date</span></span>
- <span data-ttu-id="38f70-149">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="38f70-149">Last Activity Date</span></span>
- <span data-ttu-id="38f70-150">Item Count (количество элементов)</span><span class="sxs-lookup"><span data-stu-id="38f70-150">Item Count</span></span>
- <span data-ttu-id="38f70-151">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="38f70-151">Storage Used (Byte)</span></span>
- <span data-ttu-id="38f70-152">Issue Warning Quota (Byte) [объем, при котором выводится предупреждение (байт)]</span><span class="sxs-lookup"><span data-stu-id="38f70-152">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="38f70-153">Prohibit Send Quota (Byte) [объем, при котором блокируется отправка (байт)]</span><span class="sxs-lookup"><span data-stu-id="38f70-153">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="38f70-154">Prohibit Send/Receive Quota (Byte) [объем, при котором блокируются отправка и получение (байт)]</span><span class="sxs-lookup"><span data-stu-id="38f70-154">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="38f70-155">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="38f70-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="38f70-156">Пример</span><span class="sxs-lookup"><span data-stu-id="38f70-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="38f70-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="38f70-157">Request</span></span>

<span data-ttu-id="38f70-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38f70-158">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="38f70-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="38f70-159">Response</span></span>

<span data-ttu-id="38f70-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="38f70-160">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="38f70-161">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="38f70-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="38f70-162">C#</span><span class="sxs-lookup"><span data-stu-id="38f70-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusageuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38f70-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38f70-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusageuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="38f70-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38f70-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusageuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="38f70-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="38f70-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
