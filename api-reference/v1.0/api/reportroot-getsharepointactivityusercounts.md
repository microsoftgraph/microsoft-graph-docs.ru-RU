---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Отслеживайте, как меняется количество активных пользователей. Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 7a3cb1ef2e0fff5cfa61df6a3dd63f2baf6769b8
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980656"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="05856-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="05856-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="05856-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05856-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05856-106">Получение сведений о том, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="05856-106">Get the trend in the number of active users.</span></span> <span data-ttu-id="05856-107">Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="05856-107">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="05856-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 : действия в SharePoint.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)</span><span class="sxs-lookup"><span data-stu-id="05856-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="05856-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05856-109">Permissions</span></span>

<span data-ttu-id="05856-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05856-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05856-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05856-112">Permission type</span></span>                        | <span data-ttu-id="05856-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05856-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="05856-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05856-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="05856-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="05856-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="05856-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05856-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05856-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05856-117">Not supported.</span></span>                           |
| <span data-ttu-id="05856-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05856-118">Application</span></span>                            | <span data-ttu-id="05856-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="05856-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="05856-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="05856-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="05856-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="05856-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="05856-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05856-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="05856-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="05856-123">Function parameters</span></span>

<span data-ttu-id="05856-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="05856-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="05856-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="05856-125">Parameter</span></span> | <span data-ttu-id="05856-126">Тип</span><span class="sxs-lookup"><span data-stu-id="05856-126">Type</span></span>   | <span data-ttu-id="05856-127">Описание</span><span class="sxs-lookup"><span data-stu-id="05856-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="05856-128">period</span><span class="sxs-lookup"><span data-stu-id="05856-128">period</span></span>    | <span data-ttu-id="05856-129">string</span><span class="sxs-lookup"><span data-stu-id="05856-129">string</span></span> | <span data-ttu-id="05856-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="05856-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="05856-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="05856-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="05856-132">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="05856-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="05856-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05856-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="05856-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05856-134">Request headers</span></span>

| <span data-ttu-id="05856-135">Имя</span><span class="sxs-lookup"><span data-stu-id="05856-135">Name</span></span>          | <span data-ttu-id="05856-136">Описание</span><span class="sxs-lookup"><span data-stu-id="05856-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="05856-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05856-137">Authorization</span></span> | <span data-ttu-id="05856-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05856-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="05856-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="05856-140">If-None-Match</span></span> | <span data-ttu-id="05856-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="05856-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="05856-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="05856-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="05856-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="05856-143">Response</span></span>

<span data-ttu-id="05856-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="05856-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="05856-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="05856-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="05856-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="05856-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="05856-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="05856-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="05856-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="05856-148">Report Refresh Date</span></span>
- <span data-ttu-id="05856-149">Visited Page (посетило страницу)</span><span class="sxs-lookup"><span data-stu-id="05856-149">Visited Page</span></span>
- <span data-ttu-id="05856-150">Viewed Or Edited (просмотрело или изменило)</span><span class="sxs-lookup"><span data-stu-id="05856-150">Viewed Or Edited</span></span>
- <span data-ttu-id="05856-151">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="05856-151">Synced</span></span>
- <span data-ttu-id="05856-152">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="05856-152">Shared Internally</span></span>
- <span data-ttu-id="05856-153">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="05856-153">Shared Externally</span></span>
- <span data-ttu-id="05856-154">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="05856-154">Report Date</span></span>
- <span data-ttu-id="05856-155">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="05856-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="05856-156">Пример</span><span class="sxs-lookup"><span data-stu-id="05856-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="05856-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="05856-157">Request</span></span>

<span data-ttu-id="05856-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05856-158">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="05856-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="05856-159">Response</span></span>

<span data-ttu-id="05856-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="05856-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="05856-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="05856-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

