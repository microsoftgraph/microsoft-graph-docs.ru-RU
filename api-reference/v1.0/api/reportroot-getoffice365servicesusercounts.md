---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Узнайте, сколько пользователей были активны и неактивны в каждой службе.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 45ba2e17024a4635f5d0eb8d3b01050bbf5f6867
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983484"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="330be-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="330be-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="330be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="330be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="330be-105">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="330be-105">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="330be-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — Активные Пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="330be-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="330be-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="330be-107">Permissions</span></span>

<span data-ttu-id="330be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="330be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="330be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="330be-110">Permission type</span></span>                        | <span data-ttu-id="330be-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="330be-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="330be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="330be-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="330be-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="330be-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="330be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="330be-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="330be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="330be-115">Not supported.</span></span>                           |
| <span data-ttu-id="330be-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="330be-116">Application</span></span>                            | <span data-ttu-id="330be-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="330be-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="330be-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="330be-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="330be-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="330be-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="330be-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="330be-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="330be-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="330be-121">Function parameters</span></span>

<span data-ttu-id="330be-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="330be-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="330be-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="330be-123">Parameter</span></span> | <span data-ttu-id="330be-124">Тип</span><span class="sxs-lookup"><span data-stu-id="330be-124">Type</span></span>   | <span data-ttu-id="330be-125">Описание</span><span class="sxs-lookup"><span data-stu-id="330be-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="330be-126">period</span><span class="sxs-lookup"><span data-stu-id="330be-126">period</span></span>    | <span data-ttu-id="330be-127">string</span><span class="sxs-lookup"><span data-stu-id="330be-127">string</span></span> | <span data-ttu-id="330be-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="330be-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="330be-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="330be-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="330be-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="330be-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="330be-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="330be-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="330be-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="330be-132">Request headers</span></span>

| <span data-ttu-id="330be-133">Имя</span><span class="sxs-lookup"><span data-stu-id="330be-133">Name</span></span>          | <span data-ttu-id="330be-134">Описание</span><span class="sxs-lookup"><span data-stu-id="330be-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="330be-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="330be-135">Authorization</span></span> | <span data-ttu-id="330be-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="330be-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="330be-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="330be-138">If-None-Match</span></span> | <span data-ttu-id="330be-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="330be-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="330be-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="330be-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="330be-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="330be-141">Response</span></span>

<span data-ttu-id="330be-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="330be-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="330be-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="330be-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="330be-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="330be-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="330be-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="330be-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="330be-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="330be-146">Report Refresh Date</span></span>
- <span data-ttu-id="330be-147">Exchange Active (активны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="330be-147">Exchange Active</span></span>
- <span data-ttu-id="330be-148">Exchange Inactive (неактивны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="330be-148">Exchange Inactive</span></span>
- <span data-ttu-id="330be-149">OneDrive Active (активны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="330be-149">OneDrive Active</span></span>
- <span data-ttu-id="330be-150">OneDrive Inactive (неактивны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="330be-150">OneDrive Inactive</span></span>
- <span data-ttu-id="330be-151">SharePoint Active (активны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="330be-151">SharePoint Active</span></span>
- <span data-ttu-id="330be-152">SharePoint Inactive (неактивны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="330be-152">SharePoint Inactive</span></span>
- <span data-ttu-id="330be-153">Skype For Business Active (активны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="330be-153">Skype For Business Active</span></span>
- <span data-ttu-id="330be-154">Skype For Business Inactive (неактивны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="330be-154">Skype For Business Inactive</span></span>
- <span data-ttu-id="330be-155">Yammer Active (активны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="330be-155">Yammer Active</span></span>
- <span data-ttu-id="330be-156">Yammer Inactive (неактивны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="330be-156">Yammer Inactive</span></span>
- <span data-ttu-id="330be-157">Teams Active (активны в Teams)</span><span class="sxs-lookup"><span data-stu-id="330be-157">Teams Active</span></span>
- <span data-ttu-id="330be-158">Teams Inactive (неактивны в Teams)</span><span class="sxs-lookup"><span data-stu-id="330be-158">Teams Inactive</span></span>
- <span data-ttu-id="330be-159">Office 365 Active</span><span class="sxs-lookup"><span data-stu-id="330be-159">Office 365 Active</span></span>
- <span data-ttu-id="330be-160">Неактивный Office 365</span><span class="sxs-lookup"><span data-stu-id="330be-160">Office 365 Inactive</span></span>
- <span data-ttu-id="330be-161">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="330be-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="330be-162">Пример</span><span class="sxs-lookup"><span data-stu-id="330be-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="330be-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="330be-163">Request</span></span>

<span data-ttu-id="330be-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="330be-164">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="330be-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="330be-165">Response</span></span>

<span data-ttu-id="330be-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="330be-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="330be-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="330be-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Office 365 Active,Office 365 Inactive,Report Period
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

