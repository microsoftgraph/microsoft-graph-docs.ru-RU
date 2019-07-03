---
title: 'reportRoot: getMailboxUsageDetail'
description: Получите сведения об использовании почтовых ящиков.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0ec06a813d0e7080c9b3b4f2ae8565bca9031e4a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448565"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="6f369-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="6f369-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="6f369-104">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="6f369-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="6f369-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="6f369-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="6f369-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f369-106">Permissions</span></span>

<span data-ttu-id="6f369-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f369-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f369-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f369-109">Permission type</span></span>                        | <span data-ttu-id="6f369-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f369-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6f369-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f369-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f369-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f369-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6f369-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f369-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f369-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f369-114">Not supported.</span></span>                           |
| <span data-ttu-id="6f369-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f369-115">Application</span></span>                            | <span data-ttu-id="6f369-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f369-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6f369-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f369-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6f369-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f369-118">--Http</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6f369-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6f369-119">Function parameters</span></span>

<span data-ttu-id="6f369-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="6f369-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6f369-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="6f369-121">Parameter</span></span> | <span data-ttu-id="6f369-122">Тип</span><span class="sxs-lookup"><span data-stu-id="6f369-122">Type</span></span>   | <span data-ttu-id="6f369-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6f369-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6f369-124">period</span><span class="sxs-lookup"><span data-stu-id="6f369-124">period</span></span>    | <span data-ttu-id="6f369-125">string</span><span class="sxs-lookup"><span data-stu-id="6f369-125">string</span></span> | <span data-ttu-id="6f369-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="6f369-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6f369-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="6f369-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6f369-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="6f369-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6f369-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f369-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6f369-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f369-130">Request headers</span></span>

| <span data-ttu-id="6f369-131">Имя</span><span class="sxs-lookup"><span data-stu-id="6f369-131">Name</span></span>          | <span data-ttu-id="6f369-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6f369-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6f369-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f369-133">Authorization</span></span> | <span data-ttu-id="6f369-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f369-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6f369-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6f369-136">If-None-Match</span></span> | <span data-ttu-id="6f369-137">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="6f369-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6f369-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6f369-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6f369-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f369-139">Response</span></span>

<span data-ttu-id="6f369-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6f369-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6f369-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6f369-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6f369-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6f369-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6f369-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6f369-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6f369-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="6f369-144">Report Refresh Date</span></span>
- <span data-ttu-id="6f369-145">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="6f369-145">User Principal Name</span></span>
- <span data-ttu-id="6f369-146">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="6f369-146">Display Name</span></span>
- <span data-ttu-id="6f369-147">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="6f369-147">Is Deleted</span></span>
- <span data-ttu-id="6f369-148">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="6f369-148">Deleted Date</span></span>
- <span data-ttu-id="6f369-149">Created Date (дата создания)</span><span class="sxs-lookup"><span data-stu-id="6f369-149">Created Date</span></span>
- <span data-ttu-id="6f369-150">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="6f369-150">Last Activity Date</span></span>
- <span data-ttu-id="6f369-151">Item Count (количество элементов)</span><span class="sxs-lookup"><span data-stu-id="6f369-151">Item Count</span></span>
- <span data-ttu-id="6f369-152">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="6f369-152">Storage Used (Byte)</span></span>
- <span data-ttu-id="6f369-153">Issue Warning Quota (Byte) [объем, при котором выводится предупреждение (байт)]</span><span class="sxs-lookup"><span data-stu-id="6f369-153">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="6f369-154">Prohibit Send Quota (Byte) [объем, при котором блокируется отправка (байт)]</span><span class="sxs-lookup"><span data-stu-id="6f369-154">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="6f369-155">Prohibit Send/Receive Quota (Byte) [объем, при котором блокируются отправка и получение (байт)]</span><span class="sxs-lookup"><span data-stu-id="6f369-155">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="6f369-156">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="6f369-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="6f369-157">Пример</span><span class="sxs-lookup"><span data-stu-id="6f369-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6f369-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f369-158">Request</span></span>

<span data-ttu-id="6f369-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f369-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6f369-160">C#</span><span class="sxs-lookup"><span data-stu-id="6f369-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f369-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f369-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6f369-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f369-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f369-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f369-163">Response</span></span>

<span data-ttu-id="6f369-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6f369-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="6f369-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6f369-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
