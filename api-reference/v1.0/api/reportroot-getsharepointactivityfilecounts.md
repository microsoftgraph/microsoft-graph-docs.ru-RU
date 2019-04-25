---
title: 'reportRoot: getSharePointActivityFileCounts'
description: Узнайте, сколько уникальных пользователей с лицензиями работали с хранящимися на сайтах SharePoint файлами.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3e9f577bd4847def41803083c49efa2679c65369
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550574"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="32266-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="32266-103">reportRoot: getSharePointActivityFileCounts</span></span>

<span data-ttu-id="32266-104">Узнайте, сколько уникальных пользователей с лицензиями работали с хранящимися на сайтах SharePoint файлами.</span><span class="sxs-lookup"><span data-stu-id="32266-104">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="32266-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="32266-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="32266-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32266-106">Permissions</span></span>

<span data-ttu-id="32266-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32266-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32266-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32266-109">Permission type</span></span>                        | <span data-ttu-id="32266-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32266-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="32266-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32266-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="32266-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="32266-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="32266-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32266-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32266-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32266-114">Not supported.</span></span>                           |
| <span data-ttu-id="32266-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32266-115">Application</span></span>                            | <span data-ttu-id="32266-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="32266-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="32266-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32266-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="32266-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="32266-118">Function parameters</span></span>

<span data-ttu-id="32266-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="32266-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="32266-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="32266-120">Parameter</span></span> | <span data-ttu-id="32266-121">Тип</span><span class="sxs-lookup"><span data-stu-id="32266-121">Type</span></span>   | <span data-ttu-id="32266-122">Описание</span><span class="sxs-lookup"><span data-stu-id="32266-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="32266-123">period</span><span class="sxs-lookup"><span data-stu-id="32266-123">period</span></span>    | <span data-ttu-id="32266-124">string</span><span class="sxs-lookup"><span data-stu-id="32266-124">string</span></span> | <span data-ttu-id="32266-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="32266-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="32266-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="32266-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="32266-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="32266-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="32266-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32266-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="32266-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32266-129">Request headers</span></span>

| <span data-ttu-id="32266-130">Имя</span><span class="sxs-lookup"><span data-stu-id="32266-130">Name</span></span>          | <span data-ttu-id="32266-131">Описание</span><span class="sxs-lookup"><span data-stu-id="32266-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="32266-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32266-132">Authorization</span></span> | <span data-ttu-id="32266-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32266-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="32266-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="32266-135">If-None-Match</span></span> | <span data-ttu-id="32266-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="32266-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="32266-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="32266-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="32266-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="32266-138">Response</span></span>

<span data-ttu-id="32266-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="32266-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="32266-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="32266-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="32266-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="32266-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="32266-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="32266-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="32266-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="32266-143">Report Refresh Date</span></span>
- <span data-ttu-id="32266-144">"Viewed Or Edited" (Просмотрены или изменены);</span><span class="sxs-lookup"><span data-stu-id="32266-144">Viewed Or Edited</span></span>
- <span data-ttu-id="32266-145">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="32266-145">Synced</span></span>
- <span data-ttu-id="32266-146">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="32266-146">Shared Internally</span></span>
- <span data-ttu-id="32266-147">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="32266-147">Shared Externally</span></span>
- <span data-ttu-id="32266-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="32266-148">Report Date</span></span>
- <span data-ttu-id="32266-149">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="32266-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="32266-150">Пример</span><span class="sxs-lookup"><span data-stu-id="32266-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="32266-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="32266-151">Request</span></span>

<span data-ttu-id="32266-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32266-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityfilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="32266-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="32266-153">Response</span></span>

<span data-ttu-id="32266-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="32266-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="32266-155">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="32266-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```
