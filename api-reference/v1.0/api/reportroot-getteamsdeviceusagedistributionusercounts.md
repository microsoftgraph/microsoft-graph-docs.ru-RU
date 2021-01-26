---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 01dae8db1d6ab014e936395650c4f4291dfdd430
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983115"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="7bfb1-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="7bfb1-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="7bfb1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bfb1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7bfb1-105">Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-105">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bfb1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bfb1-106">Permissions</span></span>

<span data-ttu-id="7bfb1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bfb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7bfb1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bfb1-109">Permission type</span></span>                        | <span data-ttu-id="7bfb1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bfb1-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7bfb1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bfb1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7bfb1-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7bfb1-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7bfb1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bfb1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bfb1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-114">Not supported.</span></span>                           |
| <span data-ttu-id="7bfb1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bfb1-115">Application</span></span>                            | <span data-ttu-id="7bfb1-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7bfb1-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="7bfb1-117">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="7bfb1-118">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="7bfb1-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="7bfb1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bfb1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7bfb1-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="7bfb1-120">Function parameters</span></span>

<span data-ttu-id="7bfb1-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7bfb1-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="7bfb1-122">Parameter</span></span> | <span data-ttu-id="7bfb1-123">Тип</span><span class="sxs-lookup"><span data-stu-id="7bfb1-123">Type</span></span>   | <span data-ttu-id="7bfb1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7bfb1-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7bfb1-125">period</span><span class="sxs-lookup"><span data-stu-id="7bfb1-125">period</span></span>    | <span data-ttu-id="7bfb1-126">string</span><span class="sxs-lookup"><span data-stu-id="7bfb1-126">string</span></span> | <span data-ttu-id="7bfb1-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7bfb1-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7bfb1-129">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-129">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7bfb1-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7bfb1-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bfb1-131">Request headers</span></span>

| <span data-ttu-id="7bfb1-132">Имя</span><span class="sxs-lookup"><span data-stu-id="7bfb1-132">Name</span></span>          | <span data-ttu-id="7bfb1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7bfb1-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7bfb1-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bfb1-134">Authorization</span></span> | <span data-ttu-id="7bfb1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7bfb1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bfb1-137">Response</span></span>

<span data-ttu-id="7bfb1-138">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7bfb1-139">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7bfb1-140">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7bfb1-141">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="7bfb1-141">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="7bfb1-142">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="7bfb1-142">Report Refresh Date</span></span>
- <span data-ttu-id="7bfb1-143">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="7bfb1-143">Web</span></span>
- <span data-ttu-id="7bfb1-144">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="7bfb1-144">Windows Phone</span></span>
- <span data-ttu-id="7bfb1-145">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="7bfb1-145">Android Phone</span></span>
- <span data-ttu-id="7bfb1-146">"iOS";</span><span class="sxs-lookup"><span data-stu-id="7bfb1-146">iOS</span></span>
- <span data-ttu-id="7bfb1-147">"Mac";</span><span class="sxs-lookup"><span data-stu-id="7bfb1-147">Mac</span></span>
- <span data-ttu-id="7bfb1-148">"Windows";</span><span class="sxs-lookup"><span data-stu-id="7bfb1-148">Windows</span></span>
- <span data-ttu-id="7bfb1-149">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="7bfb1-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7bfb1-150">Пример</span><span class="sxs-lookup"><span data-stu-id="7bfb1-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7bfb1-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bfb1-151">Request</span></span>

<span data-ttu-id="7bfb1-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-152">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="7bfb1-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bfb1-153">Response</span></span>

<span data-ttu-id="7bfb1-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="7bfb1-155">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="7bfb1-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
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

