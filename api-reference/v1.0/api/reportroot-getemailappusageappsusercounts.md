---
title: 'reportRoot: getEmailAppUsageAppsUserCounts'
description: Узнайте, сколько уникальных пользователей у каждого почтового приложения.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 071dde5c18a6b30cda502c121cde65a5dd69e0a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582313"
---
# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="d634c-103">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="d634c-103">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

<span data-ttu-id="d634c-104">Узнайте, сколько уникальных пользователей у каждого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="d634c-104">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="d634c-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="d634c-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="d634c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d634c-106">Permissions</span></span>

<span data-ttu-id="d634c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d634c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d634c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d634c-109">Permission type</span></span>                        | <span data-ttu-id="d634c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d634c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d634c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d634c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d634c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d634c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d634c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d634c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d634c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d634c-114">Not supported.</span></span>                           |
| <span data-ttu-id="d634c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d634c-115">Application</span></span>                            | <span data-ttu-id="d634c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d634c-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d634c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d634c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d634c-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="d634c-118">Function parameters</span></span>

<span data-ttu-id="d634c-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="d634c-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d634c-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="d634c-120">Parameter</span></span> | <span data-ttu-id="d634c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d634c-121">Type</span></span>   | <span data-ttu-id="d634c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d634c-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d634c-123">period</span><span class="sxs-lookup"><span data-stu-id="d634c-123">period</span></span>    | <span data-ttu-id="d634c-124">string</span><span class="sxs-lookup"><span data-stu-id="d634c-124">string</span></span> | <span data-ttu-id="d634c-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="d634c-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d634c-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="d634c-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d634c-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="d634c-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d634c-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d634c-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d634c-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d634c-129">Request headers</span></span>

| <span data-ttu-id="d634c-130">Имя</span><span class="sxs-lookup"><span data-stu-id="d634c-130">Name</span></span>          | <span data-ttu-id="d634c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d634c-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d634c-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d634c-132">Authorization</span></span> | <span data-ttu-id="d634c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d634c-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d634c-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d634c-135">If-None-Match</span></span> | <span data-ttu-id="d634c-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="d634c-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d634c-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d634c-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d634c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d634c-138">Response</span></span>

<span data-ttu-id="d634c-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="d634c-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d634c-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="d634c-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d634c-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d634c-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d634c-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="d634c-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d634c-143">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="d634c-143">Report Refresh Date</span></span>
- <span data-ttu-id="d634c-144">Mail For Mac (Mail для Mac)</span><span class="sxs-lookup"><span data-stu-id="d634c-144">Mail For Mac</span></span>
- <span data-ttu-id="d634c-145">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="d634c-145">Outlook For Mac</span></span>
- <span data-ttu-id="d634c-146">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="d634c-146">Outlook For Windows</span></span>
- <span data-ttu-id="d634c-147">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="d634c-147">Outlook For Mobile</span></span>
- <span data-ttu-id="d634c-148">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="d634c-148">Other For Mobile</span></span>
- <span data-ttu-id="d634c-149">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="d634c-149">Outlook For Web</span></span>
- <span data-ttu-id="d634c-150">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="d634c-150">POP3 App</span></span>
- <span data-ttu-id="d634c-151">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="d634c-151">IMAP4 App</span></span>
- <span data-ttu-id="d634c-152">"SMTP App" (Приложение с поддержкой SMTP);</span><span class="sxs-lookup"><span data-stu-id="d634c-152">SMTP App</span></span>
- <span data-ttu-id="d634c-153">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="d634c-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d634c-154">Пример</span><span class="sxs-lookup"><span data-stu-id="d634c-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d634c-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="d634c-155">Request</span></span>

<span data-ttu-id="d634c-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d634c-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageappsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageAppsUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="d634c-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="d634c-157">Response</span></span>

<span data-ttu-id="d634c-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d634c-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="d634c-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="d634c-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```
