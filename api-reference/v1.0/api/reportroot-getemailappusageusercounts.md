---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 1fdf65368158ff91dd8cc1db0ffc7d82c452e3ca
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982119"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="d5803-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="d5803-103">reportRoot: getEmailAppUsageUserCounts</span></span>

<span data-ttu-id="d5803-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5803-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5803-105">Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d5803-105">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="d5803-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 об использовании почтовых приложений.](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)</span><span class="sxs-lookup"><span data-stu-id="d5803-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5803-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5803-107">Permissions</span></span>

<span data-ttu-id="d5803-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5803-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5803-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5803-110">Permission type</span></span>                        | <span data-ttu-id="d5803-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5803-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d5803-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5803-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5803-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5803-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d5803-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5803-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5803-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5803-115">Not supported.</span></span>                           |
| <span data-ttu-id="d5803-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5803-116">Application</span></span>                            | <span data-ttu-id="d5803-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5803-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="d5803-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d5803-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d5803-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="d5803-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d5803-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5803-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d5803-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="d5803-121">Function parameters</span></span>

<span data-ttu-id="d5803-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="d5803-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d5803-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="d5803-123">Parameter</span></span> | <span data-ttu-id="d5803-124">Тип</span><span class="sxs-lookup"><span data-stu-id="d5803-124">Type</span></span>   | <span data-ttu-id="d5803-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d5803-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d5803-126">period</span><span class="sxs-lookup"><span data-stu-id="d5803-126">period</span></span>    | <span data-ttu-id="d5803-127">string</span><span class="sxs-lookup"><span data-stu-id="d5803-127">string</span></span> | <span data-ttu-id="d5803-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="d5803-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d5803-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="d5803-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d5803-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="d5803-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d5803-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5803-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d5803-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5803-132">Request headers</span></span>

| <span data-ttu-id="d5803-133">Имя</span><span class="sxs-lookup"><span data-stu-id="d5803-133">Name</span></span>          | <span data-ttu-id="d5803-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d5803-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d5803-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5803-135">Authorization</span></span> | <span data-ttu-id="d5803-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5803-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d5803-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d5803-138">If-None-Match</span></span> | <span data-ttu-id="d5803-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="d5803-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d5803-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d5803-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d5803-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5803-141">Response</span></span>

<span data-ttu-id="d5803-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="d5803-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d5803-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="d5803-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d5803-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d5803-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d5803-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="d5803-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d5803-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="d5803-146">Report Refresh Date</span></span>
- <span data-ttu-id="d5803-147">Mail For Mac (Mail для Mac)</span><span class="sxs-lookup"><span data-stu-id="d5803-147">Mail For Mac</span></span>
- <span data-ttu-id="d5803-148">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="d5803-148">Outlook For Mac</span></span>
- <span data-ttu-id="d5803-149">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="d5803-149">Outlook For Windows</span></span>
- <span data-ttu-id="d5803-150">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="d5803-150">Outlook For Mobile</span></span>
- <span data-ttu-id="d5803-151">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="d5803-151">Other For Mobile</span></span>
- <span data-ttu-id="d5803-152">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="d5803-152">Outlook For Web</span></span>
- <span data-ttu-id="d5803-153">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="d5803-153">POP3 App</span></span>
- <span data-ttu-id="d5803-154">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="d5803-154">IMAP4 App</span></span>
- <span data-ttu-id="d5803-155">SMTP App (Приложение с поддержкой SMTP)</span><span class="sxs-lookup"><span data-stu-id="d5803-155">SMTP App</span></span>
- <span data-ttu-id="d5803-156">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="d5803-156">Report Date</span></span>
- <span data-ttu-id="d5803-157">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="d5803-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d5803-158">Пример</span><span class="sxs-lookup"><span data-stu-id="d5803-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d5803-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5803-159">Request</span></span>

<span data-ttu-id="d5803-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5803-160">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getemailappusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="d5803-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5803-161">Response</span></span>

<span data-ttu-id="d5803-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d5803-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="d5803-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="d5803-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
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

