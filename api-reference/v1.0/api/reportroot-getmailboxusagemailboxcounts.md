---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период. Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: ff2e1de3d37f9de1aa0853158cb09e1141016749
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982084"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="4a111-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="4a111-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="4a111-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a111-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4a111-106">Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4a111-106">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="4a111-107">Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.</span><span class="sxs-lookup"><span data-stu-id="4a111-107">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="4a111-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — использование почтовых ящиков](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="4a111-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a111-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a111-109">Permissions</span></span>

<span data-ttu-id="4a111-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a111-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a111-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a111-112">Permission type</span></span>                        | <span data-ttu-id="4a111-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a111-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4a111-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a111-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a111-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a111-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4a111-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a111-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a111-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a111-117">Not supported.</span></span>                           |
| <span data-ttu-id="4a111-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a111-118">Application</span></span>                            | <span data-ttu-id="4a111-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a111-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="4a111-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4a111-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="4a111-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="4a111-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="4a111-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a111-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4a111-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4a111-123">Function parameters</span></span>

<span data-ttu-id="4a111-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4a111-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4a111-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="4a111-125">Parameter</span></span> | <span data-ttu-id="4a111-126">Тип</span><span class="sxs-lookup"><span data-stu-id="4a111-126">Type</span></span>   | <span data-ttu-id="4a111-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4a111-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4a111-128">period</span><span class="sxs-lookup"><span data-stu-id="4a111-128">period</span></span>    | <span data-ttu-id="4a111-129">string</span><span class="sxs-lookup"><span data-stu-id="4a111-129">string</span></span> | <span data-ttu-id="4a111-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4a111-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4a111-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4a111-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4a111-132">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4a111-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4a111-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a111-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4a111-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a111-134">Request headers</span></span>

| <span data-ttu-id="4a111-135">Имя</span><span class="sxs-lookup"><span data-stu-id="4a111-135">Name</span></span>          | <span data-ttu-id="4a111-136">Описание</span><span class="sxs-lookup"><span data-stu-id="4a111-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4a111-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a111-137">Authorization</span></span> | <span data-ttu-id="4a111-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a111-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4a111-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4a111-140">If-None-Match</span></span> | <span data-ttu-id="4a111-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="4a111-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4a111-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4a111-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4a111-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a111-143">Response</span></span>

<span data-ttu-id="4a111-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4a111-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4a111-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4a111-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4a111-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4a111-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4a111-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4a111-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4a111-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4a111-148">Report Refresh Date</span></span>
- <span data-ttu-id="4a111-149">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="4a111-149">Total</span></span>
- <span data-ttu-id="4a111-150">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="4a111-150">Active</span></span>
- <span data-ttu-id="4a111-151">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="4a111-151">Report Date</span></span>
- <span data-ttu-id="4a111-152">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="4a111-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4a111-153">Пример</span><span class="sxs-lookup"><span data-stu-id="4a111-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4a111-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a111-154">Request</span></span>

<span data-ttu-id="4a111-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a111-155">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="4a111-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a111-156">Response</span></span>

<span data-ttu-id="4a111-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a111-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="4a111-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4a111-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

