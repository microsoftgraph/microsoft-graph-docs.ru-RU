---
title: 'reportRoot: getMailboxUsageStorage'
description: Узнайте, сколько места занято в хранилище организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 731c27c1d7ee3944542d1695c8a0d3efc77ff6c1
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573993"
---
# <a name="reportroot-getmailboxusagestorage"></a><span data-ttu-id="48885-103">reportRoot: getMailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="48885-103">reportRoot: getMailboxUsageStorage</span></span>

<span data-ttu-id="48885-104">Узнайте, сколько места занято в хранилище организации.</span><span class="sxs-lookup"><span data-stu-id="48885-104">Get the amount of storage used in your organization.</span></span>

> <span data-ttu-id="48885-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование почтовых ящиков](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="48885-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="48885-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48885-106">Permissions</span></span>

<span data-ttu-id="48885-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48885-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48885-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48885-109">Permission type</span></span>                        | <span data-ttu-id="48885-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48885-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="48885-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48885-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="48885-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="48885-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="48885-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48885-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48885-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48885-114">Not supported.</span></span>                           |
| <span data-ttu-id="48885-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48885-115">Application</span></span>                            | <span data-ttu-id="48885-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="48885-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="48885-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48885-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="48885-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="48885-118">Function parameters</span></span>

<span data-ttu-id="48885-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="48885-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="48885-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="48885-120">Parameter</span></span> | <span data-ttu-id="48885-121">Тип</span><span class="sxs-lookup"><span data-stu-id="48885-121">Type</span></span>   | <span data-ttu-id="48885-122">Описание</span><span class="sxs-lookup"><span data-stu-id="48885-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="48885-123">period</span><span class="sxs-lookup"><span data-stu-id="48885-123">period</span></span>    | <span data-ttu-id="48885-124">строка</span><span class="sxs-lookup"><span data-stu-id="48885-124">string</span></span> | <span data-ttu-id="48885-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="48885-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="48885-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="48885-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="48885-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="48885-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="48885-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48885-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="48885-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48885-129">Request headers</span></span>

| <span data-ttu-id="48885-130">Имя</span><span class="sxs-lookup"><span data-stu-id="48885-130">Name</span></span>          | <span data-ttu-id="48885-131">Описание</span><span class="sxs-lookup"><span data-stu-id="48885-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="48885-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48885-132">Authorization</span></span> | <span data-ttu-id="48885-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48885-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="48885-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="48885-135">If-None-Match</span></span> | <span data-ttu-id="48885-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="48885-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="48885-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="48885-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="48885-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="48885-138">Response</span></span>

<span data-ttu-id="48885-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="48885-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="48885-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="48885-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="48885-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="48885-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="48885-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="48885-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="48885-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="48885-143">Report Refresh Date</span></span>
- <span data-ttu-id="48885-144">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="48885-144">Storage Used (Byte)</span></span>
- <span data-ttu-id="48885-145">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="48885-145">Report Date</span></span>
- <span data-ttu-id="48885-146">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="48885-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="48885-147">Пример</span><span class="sxs-lookup"><span data-stu-id="48885-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="48885-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="48885-148">Request</span></span>

<span data-ttu-id="48885-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48885-149">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagestorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageStorage(period='D7')
```

#### <a name="response"></a><span data-ttu-id="48885-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="48885-150">Response</span></span>

<span data-ttu-id="48885-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="48885-151">The following is an example of the response.</span></span>

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

<span data-ttu-id="48885-152">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="48885-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Storage Used (Byte),Report Date,Report Period
```
