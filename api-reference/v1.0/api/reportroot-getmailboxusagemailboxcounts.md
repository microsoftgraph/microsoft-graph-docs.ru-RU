---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период. Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 621c3897b7e97043d93852f14909713309164a58
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968871"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="e2606-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="e2606-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="e2606-105">Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="e2606-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="e2606-106">Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.</span><span class="sxs-lookup"><span data-stu-id="e2606-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="e2606-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="e2606-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="e2606-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2606-108">Permissions</span></span>

<span data-ttu-id="e2606-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2606-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e2606-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2606-111">Permission type</span></span>                        | <span data-ttu-id="e2606-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2606-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e2606-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2606-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2606-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2606-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e2606-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2606-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2606-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2606-116">Not supported.</span></span>                           |
| <span data-ttu-id="e2606-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2606-117">Application</span></span>                            | <span data-ttu-id="e2606-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2606-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e2606-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2606-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e2606-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="e2606-120">Function parameters</span></span>

<span data-ttu-id="e2606-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="e2606-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e2606-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="e2606-122">Parameter</span></span> | <span data-ttu-id="e2606-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e2606-123">Type</span></span>   | <span data-ttu-id="e2606-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e2606-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e2606-125">period</span><span class="sxs-lookup"><span data-stu-id="e2606-125">period</span></span>    | <span data-ttu-id="e2606-126">строка</span><span class="sxs-lookup"><span data-stu-id="e2606-126">string</span></span> | <span data-ttu-id="e2606-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="e2606-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e2606-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="e2606-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e2606-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="e2606-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e2606-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2606-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e2606-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2606-131">Request headers</span></span>

| <span data-ttu-id="e2606-132">Имя</span><span class="sxs-lookup"><span data-stu-id="e2606-132">Name</span></span>          | <span data-ttu-id="e2606-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e2606-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e2606-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2606-134">Authorization</span></span> | <span data-ttu-id="e2606-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2606-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e2606-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e2606-137">If-None-Match</span></span> | <span data-ttu-id="e2606-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="e2606-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e2606-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e2606-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e2606-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2606-140">Response</span></span>

<span data-ttu-id="e2606-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="e2606-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e2606-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="e2606-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e2606-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e2606-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e2606-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="e2606-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e2606-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="e2606-145">Report Refresh Date</span></span>
- <span data-ttu-id="e2606-146">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="e2606-146">Total</span></span>
- <span data-ttu-id="e2606-147">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="e2606-147">Active</span></span>
- <span data-ttu-id="e2606-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="e2606-148">Report Date</span></span>
- <span data-ttu-id="e2606-149">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="e2606-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e2606-150">Пример</span><span class="sxs-lookup"><span data-stu-id="e2606-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e2606-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2606-151">Request</span></span>

<span data-ttu-id="e2606-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2606-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="e2606-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2606-153">Response</span></span>

<span data-ttu-id="e2606-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e2606-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="e2606-155">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="e2606-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```
