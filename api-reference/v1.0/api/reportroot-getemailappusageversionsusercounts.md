---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 5dd67fe78d0c61ddaeb30a580f034799b8b846b2
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413305"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="4f6e0-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="4f6e0-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

<span data-ttu-id="4f6e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f6e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4f6e0-105">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-105">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="4f6e0-106">**Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="4f6e0-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="4f6e0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f6e0-107">Permissions</span></span>

<span data-ttu-id="4f6e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f6e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f6e0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f6e0-110">Permission type</span></span>                        | <span data-ttu-id="4f6e0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f6e0-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4f6e0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f6e0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f6e0-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f6e0-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4f6e0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f6e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f6e0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-115">Not supported.</span></span>                           |
| <span data-ttu-id="4f6e0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f6e0-116">Application</span></span>                            | <span data-ttu-id="4f6e0-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f6e0-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="4f6e0-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="4f6e0-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="4f6e0-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="4f6e0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f6e0-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4f6e0-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4f6e0-121">Function parameters</span></span>

<span data-ttu-id="4f6e0-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4f6e0-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="4f6e0-123">Parameter</span></span> | <span data-ttu-id="4f6e0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="4f6e0-124">Type</span></span>   | <span data-ttu-id="4f6e0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4f6e0-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4f6e0-126">period</span><span class="sxs-lookup"><span data-stu-id="4f6e0-126">period</span></span>    | <span data-ttu-id="4f6e0-127">string</span><span class="sxs-lookup"><span data-stu-id="4f6e0-127">string</span></span> | <span data-ttu-id="4f6e0-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4f6e0-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4f6e0-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4f6e0-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4f6e0-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f6e0-132">Request headers</span></span>

| <span data-ttu-id="4f6e0-133">Имя</span><span class="sxs-lookup"><span data-stu-id="4f6e0-133">Name</span></span>          | <span data-ttu-id="4f6e0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4f6e0-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4f6e0-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f6e0-135">Authorization</span></span> | <span data-ttu-id="4f6e0-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4f6e0-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4f6e0-138">If-None-Match</span></span> | <span data-ttu-id="4f6e0-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4f6e0-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4f6e0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6e0-141">Response</span></span>

<span data-ttu-id="4f6e0-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4f6e0-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4f6e0-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4f6e0-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4f6e0-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4f6e0-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4f6e0-146">Report Refresh Date</span></span>
- <span data-ttu-id="4f6e0-147">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="4f6e0-147">Outlook 2016</span></span>
- <span data-ttu-id="4f6e0-148">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="4f6e0-148">Outlook 2013</span></span>
- <span data-ttu-id="4f6e0-149">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="4f6e0-149">Outlook 2010</span></span>
- <span data-ttu-id="4f6e0-150">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="4f6e0-150">Outlook 2007</span></span>
- <span data-ttu-id="4f6e0-151">Undetermined (не определено)</span><span class="sxs-lookup"><span data-stu-id="4f6e0-151">Undetermined</span></span>
- <span data-ttu-id="4f6e0-152">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="4f6e0-152">Report Period</span></span>
- <span data-ttu-id="4f6e0-153">Outlook M365</span><span class="sxs-lookup"><span data-stu-id="4f6e0-153">Outlook M365</span></span>
- <span data-ttu-id="4f6e0-154">Outlook 2019</span><span class="sxs-lookup"><span data-stu-id="4f6e0-154">Outlook 2019</span></span>

## <a name="example"></a><span data-ttu-id="4f6e0-155">Пример</span><span class="sxs-lookup"><span data-stu-id="4f6e0-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4f6e0-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6e0-156">Request</span></span>

<span data-ttu-id="4f6e0-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-157">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getemailappusageversionsusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageVersionsUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="4f6e0-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6e0-158">Response</span></span>

<span data-ttu-id="4f6e0-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="4f6e0-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4f6e0-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period,Outlook M365,Outlook 2019
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
