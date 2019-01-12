---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: Узнайте, сколько почтовых ящиков пользователей в каждой категории квоты.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d440dc4e7c3077424eb657ac49071eff7791e388
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977978"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="601ba-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="601ba-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

<span data-ttu-id="601ba-104">Узнайте, сколько почтовых ящиков пользователей в каждой категории квоты.</span><span class="sxs-lookup"><span data-stu-id="601ba-104">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="601ba-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="601ba-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="601ba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="601ba-106">Permissions</span></span>

<span data-ttu-id="601ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="601ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="601ba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="601ba-109">Permission type</span></span>                        | <span data-ttu-id="601ba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="601ba-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="601ba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="601ba-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="601ba-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="601ba-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="601ba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="601ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="601ba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="601ba-114">Not supported.</span></span>                           |
| <span data-ttu-id="601ba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="601ba-115">Application</span></span>                            | <span data-ttu-id="601ba-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="601ba-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="601ba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="601ba-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="601ba-118">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="601ba-118">Function parameters</span></span>

<span data-ttu-id="601ba-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="601ba-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="601ba-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="601ba-120">Parameter</span></span> | <span data-ttu-id="601ba-121">Тип</span><span class="sxs-lookup"><span data-stu-id="601ba-121">Type</span></span>   | <span data-ttu-id="601ba-122">Описание</span><span class="sxs-lookup"><span data-stu-id="601ba-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="601ba-123">period</span><span class="sxs-lookup"><span data-stu-id="601ba-123">period</span></span>    | <span data-ttu-id="601ba-124">строка</span><span class="sxs-lookup"><span data-stu-id="601ba-124">string</span></span> | <span data-ttu-id="601ba-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="601ba-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="601ba-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="601ba-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="601ba-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="601ba-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="601ba-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="601ba-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="601ba-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="601ba-129">Request headers</span></span>

| <span data-ttu-id="601ba-130">Имя</span><span class="sxs-lookup"><span data-stu-id="601ba-130">Name</span></span>          | <span data-ttu-id="601ba-131">Описание</span><span class="sxs-lookup"><span data-stu-id="601ba-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="601ba-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="601ba-132">Authorization</span></span> | <span data-ttu-id="601ba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="601ba-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="601ba-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="601ba-135">If-None-Match</span></span> | <span data-ttu-id="601ba-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="601ba-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="601ba-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="601ba-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="601ba-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="601ba-138">Response</span></span>

<span data-ttu-id="601ba-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="601ba-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="601ba-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="601ba-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="601ba-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="601ba-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="601ba-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="601ba-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="601ba-143">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="601ba-143">Report Refresh Date</span></span>
- <span data-ttu-id="601ba-144">Under Limit (ограничение не превышено)</span><span class="sxs-lookup"><span data-stu-id="601ba-144">Under Limit</span></span>
- <span data-ttu-id="601ba-145">Warning Issued (выведено предупреждение)</span><span class="sxs-lookup"><span data-stu-id="601ba-145">Warning Issued</span></span>
- <span data-ttu-id="601ba-146">Send Prohibited (отправка запрещена)</span><span class="sxs-lookup"><span data-stu-id="601ba-146">Send Prohibited</span></span>
- <span data-ttu-id="601ba-147">Send/Receive Prohibited (отправка и получение запрещены)</span><span class="sxs-lookup"><span data-stu-id="601ba-147">Send/Receive Prohibited</span></span>
- <span data-ttu-id="601ba-148">Indeterminate (не определено)</span><span class="sxs-lookup"><span data-stu-id="601ba-148">Indeterminate</span></span>
- <span data-ttu-id="601ba-149">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="601ba-149">Report Date</span></span>
- <span data-ttu-id="601ba-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="601ba-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="601ba-151">Пример</span><span class="sxs-lookup"><span data-stu-id="601ba-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="601ba-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="601ba-152">Request</span></span>

<span data-ttu-id="601ba-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="601ba-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="601ba-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="601ba-154">Response</span></span>

<span data-ttu-id="601ba-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="601ba-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="601ba-156">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="601ba-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Under Limit,Warning Issued,Send Prohibited,Send/Receive Prohibited,Indeterminate,Report Date,Report Period
```
