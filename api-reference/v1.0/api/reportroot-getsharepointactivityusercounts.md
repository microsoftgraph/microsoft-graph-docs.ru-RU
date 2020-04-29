---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Отслеживайте, как меняется количество активных пользователей. Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 6ec42081ba46c9bac6d325dc8b64783f93a3c07a
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591350"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="b250a-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="b250a-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="b250a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b250a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b250a-106">Получение сведений о том, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="b250a-106">Get the trend in the number of active users.</span></span> <span data-ttu-id="b250a-107">Пользователь считается активным, если он сохранил, синхронизировал, изменил или отправил файл или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="b250a-107">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="b250a-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="b250a-108">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="b250a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b250a-109">Permissions</span></span>

<span data-ttu-id="b250a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b250a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b250a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b250a-112">Permission type</span></span>                        | <span data-ttu-id="b250a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b250a-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b250a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b250a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="b250a-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b250a-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b250a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b250a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b250a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b250a-117">Not supported.</span></span>                           |
| <span data-ttu-id="b250a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b250a-118">Application</span></span>                            | <span data-ttu-id="b250a-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b250a-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="b250a-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b250a-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="b250a-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="b250a-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="b250a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b250a-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b250a-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b250a-123">Function parameters</span></span>

<span data-ttu-id="b250a-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="b250a-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b250a-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="b250a-125">Parameter</span></span> | <span data-ttu-id="b250a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="b250a-126">Type</span></span>   | <span data-ttu-id="b250a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b250a-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b250a-128">period</span><span class="sxs-lookup"><span data-stu-id="b250a-128">period</span></span>    | <span data-ttu-id="b250a-129">string</span><span class="sxs-lookup"><span data-stu-id="b250a-129">string</span></span> | <span data-ttu-id="b250a-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="b250a-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b250a-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="b250a-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b250a-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="b250a-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b250a-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b250a-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b250a-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b250a-134">Request headers</span></span>

| <span data-ttu-id="b250a-135">Имя</span><span class="sxs-lookup"><span data-stu-id="b250a-135">Name</span></span>          | <span data-ttu-id="b250a-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b250a-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b250a-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b250a-137">Authorization</span></span> | <span data-ttu-id="b250a-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b250a-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b250a-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b250a-140">If-None-Match</span></span> | <span data-ttu-id="b250a-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="b250a-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b250a-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b250a-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b250a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b250a-143">Response</span></span>

<span data-ttu-id="b250a-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b250a-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b250a-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b250a-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b250a-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b250a-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b250a-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="b250a-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b250a-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="b250a-148">Report Refresh Date</span></span>
- <span data-ttu-id="b250a-149">Visited Page (посетило страницу)</span><span class="sxs-lookup"><span data-stu-id="b250a-149">Visited Page</span></span>
- <span data-ttu-id="b250a-150">Viewed Or Edited (просмотрело или изменило)</span><span class="sxs-lookup"><span data-stu-id="b250a-150">Viewed Or Edited</span></span>
- <span data-ttu-id="b250a-151">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="b250a-151">Synced</span></span>
- <span data-ttu-id="b250a-152">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="b250a-152">Shared Internally</span></span>
- <span data-ttu-id="b250a-153">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="b250a-153">Shared Externally</span></span>
- <span data-ttu-id="b250a-154">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="b250a-154">Report Date</span></span>
- <span data-ttu-id="b250a-155">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="b250a-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b250a-156">Пример</span><span class="sxs-lookup"><span data-stu-id="b250a-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b250a-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="b250a-157">Request</span></span>

<span data-ttu-id="b250a-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b250a-158">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="b250a-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="b250a-159">Response</span></span>

<span data-ttu-id="b250a-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b250a-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="b250a-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b250a-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
