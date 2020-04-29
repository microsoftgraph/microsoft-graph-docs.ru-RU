---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 360761aaa7320a1bb31c153f03c61ac6d4a4c252
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591161"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="238d3-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="238d3-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="238d3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="238d3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="238d3-106">Узнайте, сколько всего файлов на всех сайтах и сколько из них активны.</span><span class="sxs-lookup"><span data-stu-id="238d3-106">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="238d3-107">Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="238d3-107">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="238d3-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="238d3-108">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="238d3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="238d3-109">Permissions</span></span>

<span data-ttu-id="238d3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="238d3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="238d3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="238d3-112">Permission type</span></span>                        | <span data-ttu-id="238d3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="238d3-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="238d3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="238d3-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="238d3-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="238d3-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="238d3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="238d3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="238d3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="238d3-117">Not supported.</span></span>                           |
| <span data-ttu-id="238d3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="238d3-118">Application</span></span>                            | <span data-ttu-id="238d3-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="238d3-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="238d3-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="238d3-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="238d3-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="238d3-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="238d3-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="238d3-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="238d3-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="238d3-123">Function parameters</span></span>

<span data-ttu-id="238d3-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="238d3-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="238d3-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="238d3-125">Parameter</span></span> | <span data-ttu-id="238d3-126">Тип</span><span class="sxs-lookup"><span data-stu-id="238d3-126">Type</span></span>   | <span data-ttu-id="238d3-127">Описание</span><span class="sxs-lookup"><span data-stu-id="238d3-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="238d3-128">period</span><span class="sxs-lookup"><span data-stu-id="238d3-128">period</span></span>    | <span data-ttu-id="238d3-129">string</span><span class="sxs-lookup"><span data-stu-id="238d3-129">string</span></span> | <span data-ttu-id="238d3-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="238d3-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="238d3-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="238d3-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="238d3-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="238d3-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="238d3-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="238d3-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="238d3-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="238d3-134">Request headers</span></span>

| <span data-ttu-id="238d3-135">Имя</span><span class="sxs-lookup"><span data-stu-id="238d3-135">Name</span></span>          | <span data-ttu-id="238d3-136">Описание</span><span class="sxs-lookup"><span data-stu-id="238d3-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="238d3-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="238d3-137">Authorization</span></span> | <span data-ttu-id="238d3-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="238d3-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="238d3-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="238d3-140">If-None-Match</span></span> | <span data-ttu-id="238d3-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="238d3-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="238d3-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="238d3-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="238d3-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="238d3-143">Response</span></span>

<span data-ttu-id="238d3-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="238d3-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="238d3-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="238d3-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="238d3-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="238d3-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="238d3-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="238d3-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="238d3-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="238d3-148">Report Refresh Date</span></span>
- <span data-ttu-id="238d3-149">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="238d3-149">Site Type</span></span>
- <span data-ttu-id="238d3-150">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="238d3-150">Total</span></span>
- <span data-ttu-id="238d3-151">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="238d3-151">Active</span></span>
- <span data-ttu-id="238d3-152">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="238d3-152">Report Date</span></span>
- <span data-ttu-id="238d3-153">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="238d3-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="238d3-154">Пример</span><span class="sxs-lookup"><span data-stu-id="238d3-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="238d3-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="238d3-155">Request</span></span>

<span data-ttu-id="238d3-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="238d3-156">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="238d3-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="238d3-157">Response</span></span>

<span data-ttu-id="238d3-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="238d3-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="238d3-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="238d3-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
