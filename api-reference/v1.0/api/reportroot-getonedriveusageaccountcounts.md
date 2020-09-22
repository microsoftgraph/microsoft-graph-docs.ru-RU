---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса. Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7f524fd58c10788308562c8deff136ef15484402
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015654"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="fbcc8-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="fbcc8-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="fbcc8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbcc8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fbcc8-106">Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-106">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="fbcc8-107">Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-107">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="fbcc8-108">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports: использование OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="fbcc8-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="fbcc8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbcc8-109">Permissions</span></span>

<span data-ttu-id="fbcc8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbcc8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fbcc8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbcc8-112">Permission type</span></span>                        | <span data-ttu-id="fbcc8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbcc8-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fbcc8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbcc8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="fbcc8-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbcc8-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fbcc8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbcc8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbcc8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-117">Not supported.</span></span>                           |
| <span data-ttu-id="fbcc8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbcc8-118">Application</span></span>                            | <span data-ttu-id="fbcc8-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbcc8-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="fbcc8-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="fbcc8-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="fbcc8-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="fbcc8-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbcc8-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fbcc8-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="fbcc8-123">Function parameters</span></span>

<span data-ttu-id="fbcc8-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fbcc8-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="fbcc8-125">Parameter</span></span> | <span data-ttu-id="fbcc8-126">Тип</span><span class="sxs-lookup"><span data-stu-id="fbcc8-126">Type</span></span>   | <span data-ttu-id="fbcc8-127">Описание</span><span class="sxs-lookup"><span data-stu-id="fbcc8-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fbcc8-128">period</span><span class="sxs-lookup"><span data-stu-id="fbcc8-128">period</span></span>    | <span data-ttu-id="fbcc8-129">string</span><span class="sxs-lookup"><span data-stu-id="fbcc8-129">string</span></span> | <span data-ttu-id="fbcc8-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fbcc8-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fbcc8-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fbcc8-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="fbcc8-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbcc8-134">Request headers</span></span>

| <span data-ttu-id="fbcc8-135">Имя</span><span class="sxs-lookup"><span data-stu-id="fbcc8-135">Name</span></span>          | <span data-ttu-id="fbcc8-136">Описание</span><span class="sxs-lookup"><span data-stu-id="fbcc8-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="fbcc8-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbcc8-137">Authorization</span></span> | <span data-ttu-id="fbcc8-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="fbcc8-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="fbcc8-140">If-None-Match</span></span> | <span data-ttu-id="fbcc8-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="fbcc8-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fbcc8-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbcc8-143">Response</span></span>

<span data-ttu-id="fbcc8-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fbcc8-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fbcc8-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fbcc8-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="fbcc8-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fbcc8-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="fbcc8-148">Report Refresh Date</span></span>
- <span data-ttu-id="fbcc8-149">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="fbcc8-149">Site Type</span></span>
- <span data-ttu-id="fbcc8-150">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="fbcc8-150">Total</span></span>
- <span data-ttu-id="fbcc8-151">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="fbcc8-151">Active</span></span>
- <span data-ttu-id="fbcc8-152">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="fbcc8-152">Report Date</span></span>
- <span data-ttu-id="fbcc8-153">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="fbcc8-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fbcc8-154">Пример</span><span class="sxs-lookup"><span data-stu-id="fbcc8-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fbcc8-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbcc8-155">Request</span></span>

<span data-ttu-id="fbcc8-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-156">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getonedriveusageaccountcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="fbcc8-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbcc8-157">Response</span></span>

<span data-ttu-id="fbcc8-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="fbcc8-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="fbcc8-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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

