---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Получение количества активных пользователей за каждый день отчетного периода по продукту.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 7d348aeaf72a1ad558b736d55e9e78393733c11b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982042"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="be078-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="be078-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="be078-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be078-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="be078-105">Получение количества активных пользователей за каждый день отчетного периода по продукту.</span><span class="sxs-lookup"><span data-stu-id="be078-105">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="be078-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — Активные Пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="be078-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="be078-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be078-107">Permissions</span></span>

<span data-ttu-id="be078-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be078-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be078-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be078-110">Permission type</span></span>                        | <span data-ttu-id="be078-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be078-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="be078-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be078-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="be078-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="be078-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="be078-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be078-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be078-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be078-115">Not supported.</span></span>                           |
| <span data-ttu-id="be078-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be078-116">Application</span></span>                            | <span data-ttu-id="be078-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="be078-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="be078-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="be078-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="be078-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="be078-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="be078-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be078-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="be078-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="be078-121">Function parameters</span></span>

<span data-ttu-id="be078-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="be078-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="be078-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="be078-123">Parameter</span></span> | <span data-ttu-id="be078-124">Тип</span><span class="sxs-lookup"><span data-stu-id="be078-124">Type</span></span>   | <span data-ttu-id="be078-125">Описание</span><span class="sxs-lookup"><span data-stu-id="be078-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="be078-126">period</span><span class="sxs-lookup"><span data-stu-id="be078-126">period</span></span>    | <span data-ttu-id="be078-127">string</span><span class="sxs-lookup"><span data-stu-id="be078-127">string</span></span> | <span data-ttu-id="be078-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="be078-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="be078-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="be078-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="be078-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="be078-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="be078-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be078-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="be078-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be078-132">Request headers</span></span>

| <span data-ttu-id="be078-133">Имя</span><span class="sxs-lookup"><span data-stu-id="be078-133">Name</span></span>          | <span data-ttu-id="be078-134">Описание</span><span class="sxs-lookup"><span data-stu-id="be078-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="be078-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be078-135">Authorization</span></span> | <span data-ttu-id="be078-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be078-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="be078-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="be078-138">Response</span></span>

<span data-ttu-id="be078-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="be078-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="be078-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="be078-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="be078-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="be078-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="be078-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="be078-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="be078-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="be078-143">Report Refresh Date</span></span>
- <span data-ttu-id="be078-144">Office 365</span><span class="sxs-lookup"><span data-stu-id="be078-144">Office 365</span></span>
- <span data-ttu-id="be078-145">Exchange</span><span class="sxs-lookup"><span data-stu-id="be078-145">Exchange</span></span>
- <span data-ttu-id="be078-146">OneDrive</span><span class="sxs-lookup"><span data-stu-id="be078-146">OneDrive</span></span>
- <span data-ttu-id="be078-147">SharePoint;</span><span class="sxs-lookup"><span data-stu-id="be078-147">SharePoint</span></span>
- <span data-ttu-id="be078-148">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="be078-148">Skype For Business</span></span> 
- <span data-ttu-id="be078-149">Yammer</span><span class="sxs-lookup"><span data-stu-id="be078-149">Yammer</span></span>
- <span data-ttu-id="be078-150">Teams</span><span class="sxs-lookup"><span data-stu-id="be078-150">Teams</span></span>
- <span data-ttu-id="be078-151">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="be078-151">Report Date</span></span>
- <span data-ttu-id="be078-152">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="be078-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="be078-153">Пример</span><span class="sxs-lookup"><span data-stu-id="be078-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="be078-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="be078-154">Request</span></span>

<span data-ttu-id="be078-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be078-155">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="be078-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="be078-156">Response</span></span>

<span data-ttu-id="be078-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="be078-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="be078-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="be078-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
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

