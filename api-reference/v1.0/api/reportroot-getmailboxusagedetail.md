---
title: 'reportRoot: getMailboxUsageDetail'
description: Получите сведения об использовании почтовых ящиков.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1cadda862e0d271f7ef435be018971ad68fa1de8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607141"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="f41c8-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="f41c8-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="f41c8-104">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="f41c8-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="f41c8-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="f41c8-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="f41c8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f41c8-106">Permissions</span></span>

<span data-ttu-id="f41c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f41c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f41c8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f41c8-109">Permission type</span></span>                        | <span data-ttu-id="f41c8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f41c8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f41c8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f41c8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f41c8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f41c8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f41c8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f41c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f41c8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f41c8-114">Not supported.</span></span>                           |
| <span data-ttu-id="f41c8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f41c8-115">Application</span></span>                            | <span data-ttu-id="f41c8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f41c8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f41c8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f41c8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f41c8-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="f41c8-118">Function parameters</span></span>

<span data-ttu-id="f41c8-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="f41c8-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f41c8-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="f41c8-120">Parameter</span></span> | <span data-ttu-id="f41c8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f41c8-121">Type</span></span>   | <span data-ttu-id="f41c8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f41c8-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f41c8-123">period</span><span class="sxs-lookup"><span data-stu-id="f41c8-123">period</span></span>    | <span data-ttu-id="f41c8-124">string</span><span class="sxs-lookup"><span data-stu-id="f41c8-124">string</span></span> | <span data-ttu-id="f41c8-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f41c8-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f41c8-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="f41c8-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f41c8-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="f41c8-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f41c8-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f41c8-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f41c8-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f41c8-129">Request headers</span></span>

| <span data-ttu-id="f41c8-130">Имя</span><span class="sxs-lookup"><span data-stu-id="f41c8-130">Name</span></span>          | <span data-ttu-id="f41c8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f41c8-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f41c8-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f41c8-132">Authorization</span></span> | <span data-ttu-id="f41c8-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f41c8-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f41c8-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f41c8-135">If-None-Match</span></span> | <span data-ttu-id="f41c8-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="f41c8-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f41c8-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f41c8-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f41c8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f41c8-138">Response</span></span>

<span data-ttu-id="f41c8-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="f41c8-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f41c8-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="f41c8-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f41c8-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f41c8-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f41c8-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="f41c8-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f41c8-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="f41c8-143">Report Refresh Date</span></span>
- <span data-ttu-id="f41c8-144">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="f41c8-144">User Principal Name</span></span>
- <span data-ttu-id="f41c8-145">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="f41c8-145">Display Name</span></span>
- <span data-ttu-id="f41c8-146">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="f41c8-146">Is Deleted</span></span>
- <span data-ttu-id="f41c8-147">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="f41c8-147">Deleted Date</span></span>
- <span data-ttu-id="f41c8-148">Created Date (дата создания)</span><span class="sxs-lookup"><span data-stu-id="f41c8-148">Created Date</span></span>
- <span data-ttu-id="f41c8-149">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="f41c8-149">Last Activity Date</span></span>
- <span data-ttu-id="f41c8-150">Item Count (количество элементов)</span><span class="sxs-lookup"><span data-stu-id="f41c8-150">Item Count</span></span>
- <span data-ttu-id="f41c8-151">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="f41c8-151">Storage Used (Byte)</span></span>
- <span data-ttu-id="f41c8-152">Issue Warning Quota (Byte) [объем, при котором выводится предупреждение (байт)]</span><span class="sxs-lookup"><span data-stu-id="f41c8-152">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="f41c8-153">Prohibit Send Quota (Byte) [объем, при котором блокируется отправка (байт)]</span><span class="sxs-lookup"><span data-stu-id="f41c8-153">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="f41c8-154">Prohibit Send/Receive Quota (Byte) [объем, при котором блокируются отправка и получение (байт)]</span><span class="sxs-lookup"><span data-stu-id="f41c8-154">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="f41c8-155">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="f41c8-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f41c8-156">Пример</span><span class="sxs-lookup"><span data-stu-id="f41c8-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f41c8-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="f41c8-157">Request</span></span>

<span data-ttu-id="f41c8-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f41c8-158">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="f41c8-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="f41c8-159">Response</span></span>

<span data-ttu-id="f41c8-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f41c8-160">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f41c8-161">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="f41c8-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f41c8-162">C#</span><span class="sxs-lookup"><span data-stu-id="f41c8-162">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusageuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f41c8-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f41c8-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusageuserdetail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="f41c8-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="f41c8-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
