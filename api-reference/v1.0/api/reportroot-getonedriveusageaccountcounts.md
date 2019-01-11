---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса. Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.
localization_priority: Normal
ms.openlocfilehash: 06bedc2da04a10a01cdbcf6960c8548f06aa882c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872116"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="65618-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="65618-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="65618-105">Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="65618-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="65618-106">Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.</span><span class="sxs-lookup"><span data-stu-id="65618-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="65618-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="65618-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="65618-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65618-108">Permissions</span></span>

<span data-ttu-id="65618-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65618-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65618-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65618-111">Permission type</span></span>                        | <span data-ttu-id="65618-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65618-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="65618-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65618-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="65618-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65618-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="65618-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65618-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65618-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65618-116">Not supported.</span></span>                           |
| <span data-ttu-id="65618-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65618-117">Application</span></span>                            | <span data-ttu-id="65618-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65618-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="65618-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65618-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="65618-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="65618-120">Function parameters</span></span>

<span data-ttu-id="65618-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="65618-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="65618-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="65618-122">Parameter</span></span> | <span data-ttu-id="65618-123">Тип</span><span class="sxs-lookup"><span data-stu-id="65618-123">Type</span></span>   | <span data-ttu-id="65618-124">Описание</span><span class="sxs-lookup"><span data-stu-id="65618-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="65618-125">period</span><span class="sxs-lookup"><span data-stu-id="65618-125">period</span></span>    | <span data-ttu-id="65618-126">строка</span><span class="sxs-lookup"><span data-stu-id="65618-126">string</span></span> | <span data-ttu-id="65618-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="65618-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="65618-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="65618-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="65618-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="65618-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="65618-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65618-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="65618-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65618-131">Request headers</span></span>

| <span data-ttu-id="65618-132">Имя</span><span class="sxs-lookup"><span data-stu-id="65618-132">Name</span></span>          | <span data-ttu-id="65618-133">Описание</span><span class="sxs-lookup"><span data-stu-id="65618-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="65618-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65618-134">Authorization</span></span> | <span data-ttu-id="65618-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65618-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="65618-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="65618-137">If-None-Match</span></span> | <span data-ttu-id="65618-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="65618-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="65618-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="65618-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="65618-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="65618-140">Response</span></span>

<span data-ttu-id="65618-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="65618-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="65618-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="65618-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="65618-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="65618-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="65618-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="65618-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="65618-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="65618-145">Report Refresh Date</span></span>
- <span data-ttu-id="65618-146">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="65618-146">Site Type</span></span>
- <span data-ttu-id="65618-147">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="65618-147">Total</span></span>
- <span data-ttu-id="65618-148">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="65618-148">Active</span></span>
- <span data-ttu-id="65618-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="65618-149">Report Date</span></span>
- <span data-ttu-id="65618-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="65618-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="65618-151">Пример</span><span class="sxs-lookup"><span data-stu-id="65618-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="65618-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="65618-152">Request</span></span>

<span data-ttu-id="65618-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65618-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageaccountcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="65618-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="65618-154">Response</span></span>

<span data-ttu-id="65618-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="65618-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="65618-156">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="65618-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
