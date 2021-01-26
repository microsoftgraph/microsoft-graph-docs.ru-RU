---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Узнайте, сколько различных действий было в группах.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: f91f1822ae4423855e7928dcf232c6230898eb09
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982014"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="5f04f-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="5f04f-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

<span data-ttu-id="5f04f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f04f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f04f-105">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="5f04f-105">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="5f04f-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 — группы Microsoft 365.](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)</span><span class="sxs-lookup"><span data-stu-id="5f04f-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="5f04f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f04f-107">Permissions</span></span>

<span data-ttu-id="5f04f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f04f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f04f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f04f-110">Permission type</span></span>                        | <span data-ttu-id="5f04f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f04f-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5f04f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f04f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f04f-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f04f-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5f04f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f04f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f04f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f04f-115">Not supported.</span></span>                           |
| <span data-ttu-id="5f04f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f04f-116">Application</span></span>                            | <span data-ttu-id="5f04f-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f04f-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="5f04f-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5f04f-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5f04f-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5f04f-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5f04f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f04f-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5f04f-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="5f04f-121">Function parameters</span></span>

<span data-ttu-id="5f04f-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="5f04f-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5f04f-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="5f04f-123">Parameter</span></span> | <span data-ttu-id="5f04f-124">Тип</span><span class="sxs-lookup"><span data-stu-id="5f04f-124">Type</span></span>   | <span data-ttu-id="5f04f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="5f04f-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5f04f-126">period</span><span class="sxs-lookup"><span data-stu-id="5f04f-126">period</span></span>    | <span data-ttu-id="5f04f-127">string</span><span class="sxs-lookup"><span data-stu-id="5f04f-127">string</span></span> | <span data-ttu-id="5f04f-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5f04f-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5f04f-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="5f04f-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5f04f-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="5f04f-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5f04f-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f04f-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5f04f-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f04f-132">Request headers</span></span>

| <span data-ttu-id="5f04f-133">Имя</span><span class="sxs-lookup"><span data-stu-id="5f04f-133">Name</span></span>          | <span data-ttu-id="5f04f-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5f04f-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5f04f-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f04f-135">Authorization</span></span> | <span data-ttu-id="5f04f-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f04f-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5f04f-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5f04f-138">If-None-Match</span></span> | <span data-ttu-id="5f04f-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="5f04f-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5f04f-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5f04f-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5f04f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f04f-141">Response</span></span>

<span data-ttu-id="5f04f-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="5f04f-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5f04f-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="5f04f-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5f04f-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5f04f-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5f04f-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="5f04f-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5f04f-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="5f04f-146">Report Refresh Date</span></span>
- <span data-ttu-id="5f04f-147">Exchange Emails Received (получено писем Exchange)</span><span class="sxs-lookup"><span data-stu-id="5f04f-147">Exchange Emails Received</span></span>
- <span data-ttu-id="5f04f-148">Yammer Messages Posted (опубликовано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="5f04f-148">Yammer Messages Posted</span></span>
- <span data-ttu-id="5f04f-149">Yammer Messages Read (прочитано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="5f04f-149">Yammer Messages Read</span></span>
- <span data-ttu-id="5f04f-150">Yammer Messages Liked (понравилось сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="5f04f-150">Yammer Messages Liked</span></span>
- <span data-ttu-id="5f04f-151">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="5f04f-151">Report Date</span></span>
- <span data-ttu-id="5f04f-152">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="5f04f-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5f04f-153">Пример</span><span class="sxs-lookup"><span data-stu-id="5f04f-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5f04f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f04f-154">Request</span></span>

<span data-ttu-id="5f04f-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f04f-155">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitycounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="5f04f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f04f-156">Response</span></span>

<span data-ttu-id="5f04f-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5f04f-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="5f04f-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="5f04f-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
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

