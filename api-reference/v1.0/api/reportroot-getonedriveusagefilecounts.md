---
title: 'reportRoot: getOneDriveUsageFileCounts'
description: Получение общего количества файлов на всех сайтах и количества активных файлов. Файл считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.
ms.openlocfilehash: 4691ebf1981c4a775fb86d51e0b92eea15ca597e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025707"
---
# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="342a2-104">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="342a2-104">reportRoot: getOneDriveUsageFileCounts</span></span>

<span data-ttu-id="342a2-105">Получение общего количества файлов на всех сайтах и количества активных файлов.</span><span class="sxs-lookup"><span data-stu-id="342a2-105">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="342a2-106">Файл считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="342a2-106">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="342a2-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="342a2-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="342a2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="342a2-108">Permissions</span></span>

<span data-ttu-id="342a2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="342a2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="342a2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="342a2-111">Permission type</span></span>                        | <span data-ttu-id="342a2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="342a2-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="342a2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="342a2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="342a2-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="342a2-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="342a2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="342a2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="342a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="342a2-116">Not supported.</span></span>                           |
| <span data-ttu-id="342a2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="342a2-117">Application</span></span>                            | <span data-ttu-id="342a2-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="342a2-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="342a2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="342a2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="342a2-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="342a2-120">Function parameters</span></span>

<span data-ttu-id="342a2-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="342a2-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="342a2-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="342a2-122">Parameter</span></span> | <span data-ttu-id="342a2-123">Тип</span><span class="sxs-lookup"><span data-stu-id="342a2-123">Type</span></span>   | <span data-ttu-id="342a2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="342a2-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="342a2-125">period</span><span class="sxs-lookup"><span data-stu-id="342a2-125">period</span></span>    | <span data-ttu-id="342a2-126">строка</span><span class="sxs-lookup"><span data-stu-id="342a2-126">string</span></span> | <span data-ttu-id="342a2-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="342a2-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="342a2-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="342a2-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="342a2-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="342a2-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="342a2-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="342a2-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="342a2-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="342a2-131">Request headers</span></span>

| <span data-ttu-id="342a2-132">Имя</span><span class="sxs-lookup"><span data-stu-id="342a2-132">Name</span></span>          | <span data-ttu-id="342a2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="342a2-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="342a2-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="342a2-134">Authorization</span></span> | <span data-ttu-id="342a2-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="342a2-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="342a2-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="342a2-137">If-None-Match</span></span> | <span data-ttu-id="342a2-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="342a2-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="342a2-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="342a2-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="342a2-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="342a2-140">Response</span></span>

<span data-ttu-id="342a2-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="342a2-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="342a2-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="342a2-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="342a2-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="342a2-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="342a2-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="342a2-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="342a2-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="342a2-145">Report Refresh Date</span></span>
- <span data-ttu-id="342a2-146">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="342a2-146">Site Type</span></span>
- <span data-ttu-id="342a2-147">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="342a2-147">Total</span></span>
- <span data-ttu-id="342a2-148">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="342a2-148">Active</span></span>
- <span data-ttu-id="342a2-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="342a2-149">Report Date</span></span>
- <span data-ttu-id="342a2-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="342a2-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="342a2-151">Пример</span><span class="sxs-lookup"><span data-stu-id="342a2-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="342a2-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="342a2-152">Request</span></span>

<span data-ttu-id="342a2-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="342a2-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusagefilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="342a2-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="342a2-154">Response</span></span>

<span data-ttu-id="342a2-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="342a2-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="342a2-156">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="342a2-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
