---
title: 'reportRoot: getOffice365GroupsActivityStorage'
description: Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 26da24349d584267f762ea304e6c3256d8164697
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015710"
---
# <a name="reportroot-getoffice365groupsactivitystorage"></a><span data-ttu-id="5f85d-103">reportRoot: getOffice365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="5f85d-103">reportRoot: getOffice365GroupsActivityStorage</span></span>

<span data-ttu-id="5f85d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f85d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f85d-105">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="5f85d-105">Get the total storage used across all group mailboxes and group sites.</span></span>

> <span data-ttu-id="5f85d-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье microsoft 365 Reports — microsoft 365 Groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="5f85d-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="5f85d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f85d-107">Permissions</span></span>

<span data-ttu-id="5f85d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f85d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f85d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f85d-110">Permission type</span></span>                        | <span data-ttu-id="5f85d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f85d-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5f85d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f85d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f85d-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f85d-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5f85d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f85d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f85d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f85d-115">Not supported.</span></span>                           |
| <span data-ttu-id="5f85d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f85d-116">Application</span></span>                            | <span data-ttu-id="5f85d-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f85d-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="5f85d-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5f85d-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5f85d-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5f85d-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5f85d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f85d-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5f85d-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="5f85d-121">Function parameters</span></span>

<span data-ttu-id="5f85d-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="5f85d-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5f85d-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="5f85d-123">Parameter</span></span> | <span data-ttu-id="5f85d-124">Тип</span><span class="sxs-lookup"><span data-stu-id="5f85d-124">Type</span></span>   | <span data-ttu-id="5f85d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="5f85d-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5f85d-126">period</span><span class="sxs-lookup"><span data-stu-id="5f85d-126">period</span></span>    | <span data-ttu-id="5f85d-127">string</span><span class="sxs-lookup"><span data-stu-id="5f85d-127">string</span></span> | <span data-ttu-id="5f85d-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5f85d-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5f85d-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="5f85d-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5f85d-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="5f85d-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5f85d-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f85d-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5f85d-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f85d-132">Request headers</span></span>

| <span data-ttu-id="5f85d-133">Имя</span><span class="sxs-lookup"><span data-stu-id="5f85d-133">Name</span></span>          | <span data-ttu-id="5f85d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5f85d-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5f85d-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f85d-135">Authorization</span></span> | <span data-ttu-id="5f85d-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f85d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5f85d-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5f85d-138">If-None-Match</span></span> | <span data-ttu-id="5f85d-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="5f85d-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5f85d-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5f85d-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5f85d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f85d-141">Response</span></span>

<span data-ttu-id="5f85d-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="5f85d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5f85d-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="5f85d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5f85d-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5f85d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5f85d-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="5f85d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5f85d-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="5f85d-146">Report Refresh Date</span></span>
- <span data-ttu-id="5f85d-147">Mailbox Storage Used (Byte) [занято почтовыми ящиками (байт)]</span><span class="sxs-lookup"><span data-stu-id="5f85d-147">Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="5f85d-148">Site Storage Used (Byte) [занято сайтами (байт)]</span><span class="sxs-lookup"><span data-stu-id="5f85d-148">Site Storage Used (Byte)</span></span>
- <span data-ttu-id="5f85d-149">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="5f85d-149">Report Date</span></span>
- <span data-ttu-id="5f85d-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="5f85d-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5f85d-151">Пример</span><span class="sxs-lookup"><span data-stu-id="5f85d-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5f85d-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f85d-152">Request</span></span>

<span data-ttu-id="5f85d-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f85d-153">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitystorage"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityStorage(period='D7')
```


#### <a name="response"></a><span data-ttu-id="5f85d-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f85d-154">Response</span></span>

<span data-ttu-id="5f85d-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5f85d-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="5f85d-156">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="5f85d-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mailbox Storage Used (Byte),Site Storage Used (Byte),Report Date,Report Period
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

