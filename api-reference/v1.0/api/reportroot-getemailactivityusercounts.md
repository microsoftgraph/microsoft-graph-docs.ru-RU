---
title: 'reportRoot: getEmailActivityUserCounts'
description: Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c0f51f755b4e8882d5e6f5443637ed67db73369b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092155"
---
# <a name="reportroot-getemailactivityusercounts"></a><span data-ttu-id="a039b-103">reportRoot: getEmailActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="a039b-103">reportRoot: getEmailActivityUserCounts</span></span>

<span data-ttu-id="a039b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a039b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a039b-105">Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.</span><span class="sxs-lookup"><span data-stu-id="a039b-105">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span>

> <span data-ttu-id="a039b-106">**Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-Activity email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="a039b-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="a039b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a039b-107">Permissions</span></span>

<span data-ttu-id="a039b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a039b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a039b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a039b-110">Permission type</span></span>                        | <span data-ttu-id="a039b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a039b-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a039b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a039b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a039b-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a039b-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a039b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a039b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a039b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a039b-115">Not supported.</span></span>                           |
| <span data-ttu-id="a039b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a039b-116">Application</span></span>                            | <span data-ttu-id="a039b-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a039b-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="a039b-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a039b-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a039b-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a039b-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a039b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a039b-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a039b-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="a039b-121">Function parameters</span></span>

<span data-ttu-id="a039b-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="a039b-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a039b-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="a039b-123">Parameter</span></span> | <span data-ttu-id="a039b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a039b-124">Type</span></span>   | <span data-ttu-id="a039b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a039b-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a039b-126">period</span><span class="sxs-lookup"><span data-stu-id="a039b-126">period</span></span>    | <span data-ttu-id="a039b-127">string</span><span class="sxs-lookup"><span data-stu-id="a039b-127">string</span></span> | <span data-ttu-id="a039b-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="a039b-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a039b-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="a039b-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a039b-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="a039b-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a039b-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a039b-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a039b-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a039b-132">Request headers</span></span>

| <span data-ttu-id="a039b-133">Имя</span><span class="sxs-lookup"><span data-stu-id="a039b-133">Name</span></span>          | <span data-ttu-id="a039b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a039b-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a039b-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a039b-135">Authorization</span></span> | <span data-ttu-id="a039b-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a039b-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a039b-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a039b-138">If-None-Match</span></span> | <span data-ttu-id="a039b-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="a039b-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a039b-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a039b-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a039b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a039b-141">Response</span></span>

<span data-ttu-id="a039b-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="a039b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a039b-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="a039b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a039b-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a039b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a039b-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="a039b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a039b-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="a039b-146">Report Refresh Date</span></span>
- <span data-ttu-id="a039b-147">Send (отправлено)</span><span class="sxs-lookup"><span data-stu-id="a039b-147">Send</span></span>
- <span data-ttu-id="a039b-148">Receive (получено)</span><span class="sxs-lookup"><span data-stu-id="a039b-148">Receive</span></span>
- <span data-ttu-id="a039b-149">Read (прочитано)</span><span class="sxs-lookup"><span data-stu-id="a039b-149">Read</span></span>
- <span data-ttu-id="a039b-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="a039b-150">Report Date</span></span>
- <span data-ttu-id="a039b-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="a039b-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a039b-152">Пример</span><span class="sxs-lookup"><span data-stu-id="a039b-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a039b-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="a039b-153">Request</span></span>

<span data-ttu-id="a039b-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a039b-154">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getemailactivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="a039b-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="a039b-155">Response</span></span>

<span data-ttu-id="a039b-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a039b-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="a039b-157">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="a039b-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
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

