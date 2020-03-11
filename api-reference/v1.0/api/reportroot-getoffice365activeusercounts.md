---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Получение количества активных пользователей за каждый день отчетного периода по продукту.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 05a2bef267a20d8566ac96baf4f0eee222e9d577
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591301"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="c3b29-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="c3b29-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="c3b29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3b29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3b29-105">Получение количества активных пользователей за каждый день отчетного периода по продукту.</span><span class="sxs-lookup"><span data-stu-id="c3b29-105">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="c3b29-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="c3b29-106">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="c3b29-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3b29-107">Permissions</span></span>

<span data-ttu-id="c3b29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3b29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c3b29-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3b29-110">Permission type</span></span>                        | <span data-ttu-id="c3b29-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3b29-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c3b29-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3b29-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c3b29-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3b29-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c3b29-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3b29-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3b29-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3b29-115">Not supported.</span></span>                           |
| <span data-ttu-id="c3b29-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3b29-116">Application</span></span>                            | <span data-ttu-id="c3b29-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3b29-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="c3b29-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c3b29-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="c3b29-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="c3b29-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="c3b29-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3b29-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c3b29-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c3b29-121">Function parameters</span></span>

<span data-ttu-id="c3b29-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c3b29-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c3b29-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="c3b29-123">Parameter</span></span> | <span data-ttu-id="c3b29-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c3b29-124">Type</span></span>   | <span data-ttu-id="c3b29-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c3b29-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c3b29-126">period</span><span class="sxs-lookup"><span data-stu-id="c3b29-126">period</span></span>    | <span data-ttu-id="c3b29-127">string</span><span class="sxs-lookup"><span data-stu-id="c3b29-127">string</span></span> | <span data-ttu-id="c3b29-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c3b29-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c3b29-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c3b29-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c3b29-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c3b29-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c3b29-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3b29-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c3b29-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3b29-132">Request headers</span></span>

| <span data-ttu-id="c3b29-133">Имя</span><span class="sxs-lookup"><span data-stu-id="c3b29-133">Name</span></span>          | <span data-ttu-id="c3b29-134">Описание</span><span class="sxs-lookup"><span data-stu-id="c3b29-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c3b29-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3b29-135">Authorization</span></span> | <span data-ttu-id="c3b29-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3b29-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c3b29-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3b29-138">Response</span></span>

<span data-ttu-id="c3b29-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c3b29-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c3b29-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c3b29-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c3b29-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c3b29-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c3b29-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c3b29-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c3b29-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c3b29-143">Report Refresh Date</span></span>
- <span data-ttu-id="c3b29-144">Office 365</span><span class="sxs-lookup"><span data-stu-id="c3b29-144">Office 365</span></span>
- <span data-ttu-id="c3b29-145">Exchange</span><span class="sxs-lookup"><span data-stu-id="c3b29-145">Exchange</span></span>
- <span data-ttu-id="c3b29-146">OneDrive;</span><span class="sxs-lookup"><span data-stu-id="c3b29-146">OneDrive</span></span>
- <span data-ttu-id="c3b29-147">SharePoint;</span><span class="sxs-lookup"><span data-stu-id="c3b29-147">SharePoint</span></span>
- <span data-ttu-id="c3b29-148">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="c3b29-148">Skype For Business</span></span> 
- <span data-ttu-id="c3b29-149">Yammer</span><span class="sxs-lookup"><span data-stu-id="c3b29-149">Yammer</span></span>
- <span data-ttu-id="c3b29-150">Teams</span><span class="sxs-lookup"><span data-stu-id="c3b29-150">Teams</span></span>
- <span data-ttu-id="c3b29-151">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="c3b29-151">Report Date</span></span>
- <span data-ttu-id="c3b29-152">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="c3b29-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c3b29-153">Пример</span><span class="sxs-lookup"><span data-stu-id="c3b29-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c3b29-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3b29-154">Request</span></span>

<span data-ttu-id="c3b29-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3b29-155">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="c3b29-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3b29-156">Response</span></span>

<span data-ttu-id="c3b29-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c3b29-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="c3b29-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c3b29-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
