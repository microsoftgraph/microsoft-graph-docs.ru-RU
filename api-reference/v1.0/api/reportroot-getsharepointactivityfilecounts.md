---
title: 'reportRoot: getSharePointActivityFileCounts'
description: Узнайте, сколько уникальных пользователей с лицензиями работали с хранящимися на сайтах SharePoint файлами.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 8da5e12ec4bf620f0101d81aaeadf5ab61c90d18
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954829"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="26de8-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="26de8-103">reportRoot: getSharePointActivityFileCounts</span></span>

<span data-ttu-id="26de8-104">Узнайте, сколько уникальных пользователей с лицензиями работали с хранящимися на сайтах SharePoint файлами.</span><span class="sxs-lookup"><span data-stu-id="26de8-104">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="26de8-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="26de8-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="26de8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26de8-106">Permissions</span></span>

<span data-ttu-id="26de8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26de8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26de8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26de8-109">Permission type</span></span>                        | <span data-ttu-id="26de8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26de8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="26de8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26de8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="26de8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="26de8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="26de8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26de8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26de8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26de8-114">Not supported.</span></span>                           |
| <span data-ttu-id="26de8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26de8-115">Application</span></span>                            | <span data-ttu-id="26de8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="26de8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="26de8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26de8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="26de8-118">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="26de8-118">Function parameters</span></span>

<span data-ttu-id="26de8-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="26de8-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="26de8-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="26de8-120">Parameter</span></span> | <span data-ttu-id="26de8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="26de8-121">Type</span></span>   | <span data-ttu-id="26de8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="26de8-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="26de8-123">period</span><span class="sxs-lookup"><span data-stu-id="26de8-123">period</span></span>    | <span data-ttu-id="26de8-124">строка</span><span class="sxs-lookup"><span data-stu-id="26de8-124">string</span></span> | <span data-ttu-id="26de8-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="26de8-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="26de8-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="26de8-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="26de8-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="26de8-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="26de8-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26de8-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="26de8-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26de8-129">Request headers</span></span>

| <span data-ttu-id="26de8-130">Имя</span><span class="sxs-lookup"><span data-stu-id="26de8-130">Name</span></span>          | <span data-ttu-id="26de8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="26de8-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="26de8-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26de8-132">Authorization</span></span> | <span data-ttu-id="26de8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26de8-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="26de8-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="26de8-135">If-None-Match</span></span> | <span data-ttu-id="26de8-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="26de8-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="26de8-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="26de8-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="26de8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="26de8-138">Response</span></span>

<span data-ttu-id="26de8-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="26de8-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="26de8-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="26de8-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="26de8-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="26de8-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="26de8-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="26de8-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="26de8-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="26de8-143">Report Refresh Date</span></span>
- <span data-ttu-id="26de8-144">"Viewed Or Edited" (Просмотрены или изменены);</span><span class="sxs-lookup"><span data-stu-id="26de8-144">Viewed Or Edited</span></span>
- <span data-ttu-id="26de8-145">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="26de8-145">Synced</span></span>
- <span data-ttu-id="26de8-146">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="26de8-146">Shared Internally</span></span>
- <span data-ttu-id="26de8-147">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="26de8-147">Shared Externally</span></span>
- <span data-ttu-id="26de8-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="26de8-148">Report Date</span></span>
- <span data-ttu-id="26de8-149">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="26de8-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="26de8-150">Пример</span><span class="sxs-lookup"><span data-stu-id="26de8-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="26de8-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="26de8-151">Request</span></span>

<span data-ttu-id="26de8-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26de8-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityfilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="26de8-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="26de8-153">Response</span></span>

<span data-ttu-id="26de8-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="26de8-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="26de8-155">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="26de8-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```
