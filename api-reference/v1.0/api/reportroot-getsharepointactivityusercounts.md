---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Отслеживайте, как меняется количество активных пользователей. Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 09b0b823858d34212aa0580c3c85f645734bf901
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525441"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="f50e4-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="f50e4-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="f50e4-105">Отслеживайте, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f50e4-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="f50e4-106">Пользователь считается активным, если он сохранил, синхронизировал, изменил или отправил файл или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="f50e4-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="f50e4-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="f50e4-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="f50e4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f50e4-108">Permissions</span></span>

<span data-ttu-id="f50e4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f50e4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f50e4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f50e4-111">Permission type</span></span>                        | <span data-ttu-id="f50e4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f50e4-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f50e4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f50e4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f50e4-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f50e4-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f50e4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f50e4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f50e4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f50e4-116">Not supported.</span></span>                           |
| <span data-ttu-id="f50e4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f50e4-117">Application</span></span>                            | <span data-ttu-id="f50e4-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f50e4-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f50e4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f50e4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f50e4-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="f50e4-120">Function parameters</span></span>

<span data-ttu-id="f50e4-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="f50e4-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f50e4-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="f50e4-122">Parameter</span></span> | <span data-ttu-id="f50e4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f50e4-123">Type</span></span>   | <span data-ttu-id="f50e4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f50e4-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f50e4-125">period</span><span class="sxs-lookup"><span data-stu-id="f50e4-125">period</span></span>    | <span data-ttu-id="f50e4-126">string</span><span class="sxs-lookup"><span data-stu-id="f50e4-126">string</span></span> | <span data-ttu-id="f50e4-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f50e4-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f50e4-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="f50e4-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f50e4-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="f50e4-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f50e4-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f50e4-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f50e4-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f50e4-131">Request headers</span></span>

| <span data-ttu-id="f50e4-132">Имя</span><span class="sxs-lookup"><span data-stu-id="f50e4-132">Name</span></span>          | <span data-ttu-id="f50e4-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f50e4-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f50e4-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f50e4-134">Authorization</span></span> | <span data-ttu-id="f50e4-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f50e4-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f50e4-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f50e4-137">If-None-Match</span></span> | <span data-ttu-id="f50e4-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="f50e4-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f50e4-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f50e4-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f50e4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f50e4-140">Response</span></span>

<span data-ttu-id="f50e4-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="f50e4-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f50e4-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="f50e4-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f50e4-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f50e4-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f50e4-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="f50e4-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f50e4-145">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="f50e4-145">Report Refresh Date</span></span>
- <span data-ttu-id="f50e4-146">Visited Page (посетило страницу)</span><span class="sxs-lookup"><span data-stu-id="f50e4-146">Visited Page</span></span>
- <span data-ttu-id="f50e4-147">Viewed Or Edited (просмотрело или изменило)</span><span class="sxs-lookup"><span data-stu-id="f50e4-147">Viewed Or Edited</span></span>
- <span data-ttu-id="f50e4-148">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="f50e4-148">Synced</span></span>
- <span data-ttu-id="f50e4-149">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="f50e4-149">Shared Internally</span></span>
- <span data-ttu-id="f50e4-150">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="f50e4-150">Shared Externally</span></span>
- <span data-ttu-id="f50e4-151">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="f50e4-151">Report Date</span></span>
- <span data-ttu-id="f50e4-152">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="f50e4-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f50e4-153">Пример</span><span class="sxs-lookup"><span data-stu-id="f50e4-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f50e4-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="f50e4-154">Request</span></span>

<span data-ttu-id="f50e4-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f50e4-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="f50e4-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="f50e4-156">Response</span></span>

<span data-ttu-id="f50e4-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f50e4-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="f50e4-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="f50e4-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```
