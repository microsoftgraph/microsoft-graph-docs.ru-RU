---
title: 'reportRoot: getMailboxUsageStorage'
description: Узнайте, сколько места занято в хранилище организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 1df1b2c38c828fae839b2010084f7bab807ed591
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897423"
---
# <a name="reportroot-getmailboxusagestorage"></a><span data-ttu-id="10e07-103">reportRoot: getMailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="10e07-103">reportRoot: getMailboxUsageStorage</span></span>

<span data-ttu-id="10e07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10e07-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10e07-105">Узнайте, сколько места занято в хранилище организации.</span><span class="sxs-lookup"><span data-stu-id="10e07-105">Get the amount of storage used in your organization.</span></span>

> <span data-ttu-id="10e07-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-Mailbox Reporting](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="10e07-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="10e07-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10e07-107">Permissions</span></span>

<span data-ttu-id="10e07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10e07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10e07-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10e07-110">Permission type</span></span>                        | <span data-ttu-id="10e07-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10e07-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="10e07-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10e07-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="10e07-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="10e07-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="10e07-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10e07-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10e07-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10e07-115">Not supported.</span></span>                           |
| <span data-ttu-id="10e07-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10e07-116">Application</span></span>                            | <span data-ttu-id="10e07-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="10e07-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="10e07-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="10e07-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="10e07-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="10e07-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="10e07-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10e07-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="10e07-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="10e07-121">Function parameters</span></span>

<span data-ttu-id="10e07-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="10e07-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="10e07-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="10e07-123">Parameter</span></span> | <span data-ttu-id="10e07-124">Тип</span><span class="sxs-lookup"><span data-stu-id="10e07-124">Type</span></span>   | <span data-ttu-id="10e07-125">Описание</span><span class="sxs-lookup"><span data-stu-id="10e07-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="10e07-126">period</span><span class="sxs-lookup"><span data-stu-id="10e07-126">period</span></span>    | <span data-ttu-id="10e07-127">string</span><span class="sxs-lookup"><span data-stu-id="10e07-127">string</span></span> | <span data-ttu-id="10e07-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="10e07-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="10e07-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="10e07-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="10e07-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="10e07-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="10e07-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10e07-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="10e07-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10e07-132">Request headers</span></span>

| <span data-ttu-id="10e07-133">Имя</span><span class="sxs-lookup"><span data-stu-id="10e07-133">Name</span></span>          | <span data-ttu-id="10e07-134">Описание</span><span class="sxs-lookup"><span data-stu-id="10e07-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="10e07-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10e07-135">Authorization</span></span> | <span data-ttu-id="10e07-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10e07-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="10e07-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="10e07-138">If-None-Match</span></span> | <span data-ttu-id="10e07-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="10e07-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="10e07-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="10e07-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="10e07-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="10e07-141">Response</span></span>

<span data-ttu-id="10e07-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="10e07-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="10e07-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="10e07-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="10e07-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="10e07-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="10e07-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="10e07-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="10e07-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="10e07-146">Report Refresh Date</span></span>
- <span data-ttu-id="10e07-147">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="10e07-147">Storage Used (Byte)</span></span>
- <span data-ttu-id="10e07-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="10e07-148">Report Date</span></span>
- <span data-ttu-id="10e07-149">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="10e07-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="10e07-150">Пример</span><span class="sxs-lookup"><span data-stu-id="10e07-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="10e07-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="10e07-151">Request</span></span>

<span data-ttu-id="10e07-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10e07-152">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getmailboxusagestorage"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageStorage(period='D7')
```


#### <a name="response"></a><span data-ttu-id="10e07-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="10e07-153">Response</span></span>

<span data-ttu-id="10e07-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10e07-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="10e07-155">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="10e07-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Storage Used (Byte),Report Date,Report Period
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
