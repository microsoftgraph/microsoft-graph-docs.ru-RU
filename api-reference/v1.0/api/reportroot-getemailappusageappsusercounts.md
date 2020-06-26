---
title: 'reportRoot: getEmailAppUsageAppsUserCounts'
description: Узнайте, сколько уникальных пользователей у каждого почтового приложения.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a7aeb6faa93d4d6ddc654a08daa7bf2095b35846
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898228"
---
# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="33497-103">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="33497-103">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

<span data-ttu-id="33497-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33497-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33497-105">Узнайте, сколько уникальных пользователей у каждого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="33497-105">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="33497-106">**Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="33497-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="33497-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33497-107">Permissions</span></span>

<span data-ttu-id="33497-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="33497-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="33497-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33497-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="33497-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33497-110">Permission type</span></span>                        | <span data-ttu-id="33497-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33497-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="33497-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33497-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="33497-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="33497-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="33497-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33497-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33497-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33497-115">Not supported.</span></span>                           |
| <span data-ttu-id="33497-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33497-116">Application</span></span>                            | <span data-ttu-id="33497-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="33497-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="33497-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="33497-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="33497-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="33497-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="33497-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33497-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="33497-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="33497-121">Function parameters</span></span>

<span data-ttu-id="33497-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="33497-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="33497-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="33497-123">Parameter</span></span> | <span data-ttu-id="33497-124">Тип</span><span class="sxs-lookup"><span data-stu-id="33497-124">Type</span></span>   | <span data-ttu-id="33497-125">Описание</span><span class="sxs-lookup"><span data-stu-id="33497-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="33497-126">period</span><span class="sxs-lookup"><span data-stu-id="33497-126">period</span></span>    | <span data-ttu-id="33497-127">string</span><span class="sxs-lookup"><span data-stu-id="33497-127">string</span></span> | <span data-ttu-id="33497-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="33497-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="33497-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="33497-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="33497-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="33497-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="33497-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33497-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="33497-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33497-132">Request headers</span></span>

| <span data-ttu-id="33497-133">Имя</span><span class="sxs-lookup"><span data-stu-id="33497-133">Name</span></span>          | <span data-ttu-id="33497-134">Описание</span><span class="sxs-lookup"><span data-stu-id="33497-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="33497-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33497-135">Authorization</span></span> | <span data-ttu-id="33497-136">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="33497-136">Bearer {token}.</span></span> <span data-ttu-id="33497-137">Required.</span><span class="sxs-lookup"><span data-stu-id="33497-137">Required.</span></span>                |
| <span data-ttu-id="33497-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="33497-138">If-None-Match</span></span> | <span data-ttu-id="33497-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="33497-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="33497-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="33497-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="33497-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="33497-141">Response</span></span>

<span data-ttu-id="33497-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="33497-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="33497-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="33497-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="33497-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="33497-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="33497-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="33497-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="33497-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="33497-146">Report Refresh Date</span></span>
- <span data-ttu-id="33497-147">Mail For Mac (Mail для Mac)</span><span class="sxs-lookup"><span data-stu-id="33497-147">Mail For Mac</span></span>
- <span data-ttu-id="33497-148">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="33497-148">Outlook For Mac</span></span>
- <span data-ttu-id="33497-149">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="33497-149">Outlook For Windows</span></span>
- <span data-ttu-id="33497-150">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="33497-150">Outlook For Mobile</span></span>
- <span data-ttu-id="33497-151">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="33497-151">Other For Mobile</span></span>
- <span data-ttu-id="33497-152">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="33497-152">Outlook For Web</span></span>
- <span data-ttu-id="33497-153">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="33497-153">POP3 App</span></span>
- <span data-ttu-id="33497-154">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="33497-154">IMAP4 App</span></span>
- <span data-ttu-id="33497-155">"SMTP App" (Приложение с поддержкой SMTP);</span><span class="sxs-lookup"><span data-stu-id="33497-155">SMTP App</span></span>
- <span data-ttu-id="33497-156">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="33497-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="33497-157">Пример</span><span class="sxs-lookup"><span data-stu-id="33497-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="33497-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="33497-158">Request</span></span>

<span data-ttu-id="33497-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33497-159">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getemailappusageappsusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageAppsUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="33497-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="33497-160">Response</span></span>

<span data-ttu-id="33497-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="33497-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="33497-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="33497-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
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
