---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Отслеживайте, как меняется количество активных пользователей. Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: ff4fcd543c87e1915a7a8ba1a3ce6abda045b40a
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895904"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="d8794-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="d8794-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="d8794-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8794-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8794-106">Получение сведений о том, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="d8794-106">Get the trend in the number of active users.</span></span> <span data-ttu-id="d8794-107">Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="d8794-107">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="d8794-108">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-SharePoint Activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="d8794-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="d8794-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8794-109">Permissions</span></span>

<span data-ttu-id="d8794-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d8794-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d8794-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8794-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d8794-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8794-112">Permission type</span></span>                        | <span data-ttu-id="d8794-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8794-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d8794-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8794-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8794-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8794-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d8794-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8794-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8794-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8794-117">Not supported.</span></span>                           |
| <span data-ttu-id="d8794-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8794-118">Application</span></span>                            | <span data-ttu-id="d8794-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8794-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="d8794-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d8794-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d8794-121">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="d8794-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d8794-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8794-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d8794-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="d8794-123">Function parameters</span></span>

<span data-ttu-id="d8794-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="d8794-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d8794-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="d8794-125">Parameter</span></span> | <span data-ttu-id="d8794-126">Тип</span><span class="sxs-lookup"><span data-stu-id="d8794-126">Type</span></span>   | <span data-ttu-id="d8794-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d8794-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d8794-128">period</span><span class="sxs-lookup"><span data-stu-id="d8794-128">period</span></span>    | <span data-ttu-id="d8794-129">string</span><span class="sxs-lookup"><span data-stu-id="d8794-129">string</span></span> | <span data-ttu-id="d8794-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="d8794-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d8794-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="d8794-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d8794-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="d8794-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d8794-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8794-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d8794-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8794-134">Request headers</span></span>

| <span data-ttu-id="d8794-135">Имя</span><span class="sxs-lookup"><span data-stu-id="d8794-135">Name</span></span>          | <span data-ttu-id="d8794-136">Описание</span><span class="sxs-lookup"><span data-stu-id="d8794-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d8794-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8794-137">Authorization</span></span> | <span data-ttu-id="d8794-138">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="d8794-138">Bearer {token}.</span></span> <span data-ttu-id="d8794-139">Required.</span><span class="sxs-lookup"><span data-stu-id="d8794-139">Required.</span></span>                |
| <span data-ttu-id="d8794-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d8794-140">If-None-Match</span></span> | <span data-ttu-id="d8794-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="d8794-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d8794-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d8794-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d8794-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8794-143">Response</span></span>

<span data-ttu-id="d8794-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="d8794-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d8794-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="d8794-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d8794-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d8794-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d8794-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="d8794-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d8794-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="d8794-148">Report Refresh Date</span></span>
- <span data-ttu-id="d8794-149">Visited Page (посетило страницу)</span><span class="sxs-lookup"><span data-stu-id="d8794-149">Visited Page</span></span>
- <span data-ttu-id="d8794-150">Viewed Or Edited (просмотрело или изменило)</span><span class="sxs-lookup"><span data-stu-id="d8794-150">Viewed Or Edited</span></span>
- <span data-ttu-id="d8794-151">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="d8794-151">Synced</span></span>
- <span data-ttu-id="d8794-152">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="d8794-152">Shared Internally</span></span>
- <span data-ttu-id="d8794-153">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="d8794-153">Shared Externally</span></span>
- <span data-ttu-id="d8794-154">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="d8794-154">Report Date</span></span>
- <span data-ttu-id="d8794-155">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="d8794-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d8794-156">Пример</span><span class="sxs-lookup"><span data-stu-id="d8794-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d8794-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8794-157">Request</span></span>

<span data-ttu-id="d8794-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8794-158">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="d8794-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8794-159">Response</span></span>

<span data-ttu-id="d8794-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d8794-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="d8794-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="d8794-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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
