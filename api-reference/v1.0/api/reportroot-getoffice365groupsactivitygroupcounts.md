---
title: 'reportRoot: getOffice365GroupsActivityGroupCounts'
description: Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7cfb356f10dc82a189a492fe24005dda6d2b7594
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897451"
---
# <a name="reportroot-getoffice365groupsactivitygroupcounts"></a><span data-ttu-id="451be-103">reportRoot: getOffice365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="451be-103">reportRoot: getOffice365GroupsActivityGroupCounts</span></span>

<span data-ttu-id="451be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="451be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="451be-105">Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день.</span><span class="sxs-lookup"><span data-stu-id="451be-105">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span>

> <span data-ttu-id="451be-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье microsoft 365 Reports — microsoft 365 Groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="451be-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="451be-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="451be-107">Permissions</span></span>

<span data-ttu-id="451be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="451be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="451be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="451be-110">Permission type</span></span>                        | <span data-ttu-id="451be-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="451be-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="451be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="451be-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="451be-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="451be-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="451be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="451be-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="451be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="451be-115">Not supported.</span></span>                           |
| <span data-ttu-id="451be-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="451be-116">Application</span></span>                            | <span data-ttu-id="451be-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="451be-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="451be-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="451be-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="451be-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="451be-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="451be-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="451be-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="451be-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="451be-121">Function parameters</span></span>

<span data-ttu-id="451be-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="451be-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="451be-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="451be-123">Parameter</span></span> | <span data-ttu-id="451be-124">Тип</span><span class="sxs-lookup"><span data-stu-id="451be-124">Type</span></span>   | <span data-ttu-id="451be-125">Описание</span><span class="sxs-lookup"><span data-stu-id="451be-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="451be-126">period</span><span class="sxs-lookup"><span data-stu-id="451be-126">period</span></span>    | <span data-ttu-id="451be-127">string</span><span class="sxs-lookup"><span data-stu-id="451be-127">string</span></span> | <span data-ttu-id="451be-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="451be-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="451be-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="451be-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="451be-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="451be-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="451be-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="451be-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="451be-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="451be-132">Request headers</span></span>

| <span data-ttu-id="451be-133">Имя</span><span class="sxs-lookup"><span data-stu-id="451be-133">Name</span></span>          | <span data-ttu-id="451be-134">Описание</span><span class="sxs-lookup"><span data-stu-id="451be-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="451be-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="451be-135">Authorization</span></span> | <span data-ttu-id="451be-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="451be-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="451be-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="451be-138">If-None-Match</span></span> | <span data-ttu-id="451be-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="451be-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="451be-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="451be-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="451be-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="451be-141">Response</span></span>

<span data-ttu-id="451be-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="451be-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="451be-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="451be-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="451be-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="451be-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="451be-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="451be-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="451be-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="451be-146">Report Refresh Date</span></span>
- <span data-ttu-id="451be-147">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="451be-147">Total</span></span>
- <span data-ttu-id="451be-148">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="451be-148">Active</span></span>
- <span data-ttu-id="451be-149">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="451be-149">Report Date</span></span>
- <span data-ttu-id="451be-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="451be-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="451be-151">Пример</span><span class="sxs-lookup"><span data-stu-id="451be-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="451be-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="451be-152">Request</span></span>

<span data-ttu-id="451be-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="451be-153">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitygroupcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityGroupCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="451be-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="451be-154">Response</span></span>

<span data-ttu-id="451be-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="451be-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="451be-156">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="451be-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
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
