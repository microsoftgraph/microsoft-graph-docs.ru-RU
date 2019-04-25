---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 242a7256bab59fa8fa010a1e1966e262c81797c2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582327"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="743b7-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="743b7-103">reportRoot: getEmailAppUsageUserCounts</span></span>

<span data-ttu-id="743b7-104">Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="743b7-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="743b7-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Центре администрирования Office 365 — использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="743b7-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="743b7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="743b7-106">Permissions</span></span>

<span data-ttu-id="743b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="743b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="743b7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="743b7-109">Permission type</span></span>                        | <span data-ttu-id="743b7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="743b7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="743b7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="743b7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="743b7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="743b7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="743b7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="743b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="743b7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="743b7-114">Not supported.</span></span>                           |
| <span data-ttu-id="743b7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="743b7-115">Application</span></span>                            | <span data-ttu-id="743b7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="743b7-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="743b7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="743b7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="743b7-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="743b7-118">Function parameters</span></span>

<span data-ttu-id="743b7-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="743b7-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="743b7-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="743b7-120">Parameter</span></span> | <span data-ttu-id="743b7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="743b7-121">Type</span></span>   | <span data-ttu-id="743b7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="743b7-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="743b7-123">period</span><span class="sxs-lookup"><span data-stu-id="743b7-123">period</span></span>    | <span data-ttu-id="743b7-124">string</span><span class="sxs-lookup"><span data-stu-id="743b7-124">string</span></span> | <span data-ttu-id="743b7-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="743b7-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="743b7-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="743b7-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="743b7-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="743b7-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="743b7-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="743b7-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="743b7-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="743b7-129">Request headers</span></span>

| <span data-ttu-id="743b7-130">Имя</span><span class="sxs-lookup"><span data-stu-id="743b7-130">Name</span></span>          | <span data-ttu-id="743b7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="743b7-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="743b7-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="743b7-132">Authorization</span></span> | <span data-ttu-id="743b7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="743b7-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="743b7-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="743b7-135">If-None-Match</span></span> | <span data-ttu-id="743b7-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="743b7-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="743b7-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="743b7-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="743b7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="743b7-138">Response</span></span>

<span data-ttu-id="743b7-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="743b7-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="743b7-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="743b7-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="743b7-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="743b7-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="743b7-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="743b7-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="743b7-143">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="743b7-143">Report Refresh Date</span></span>
- <span data-ttu-id="743b7-144">Mail For Mac (Mail для Mac)</span><span class="sxs-lookup"><span data-stu-id="743b7-144">Mail For Mac</span></span>
- <span data-ttu-id="743b7-145">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="743b7-145">Outlook For Mac</span></span>
- <span data-ttu-id="743b7-146">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="743b7-146">Outlook For Windows</span></span>
- <span data-ttu-id="743b7-147">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="743b7-147">Outlook For Mobile</span></span>
- <span data-ttu-id="743b7-148">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="743b7-148">Other For Mobile</span></span>
- <span data-ttu-id="743b7-149">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="743b7-149">Outlook For Web</span></span>
- <span data-ttu-id="743b7-150">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="743b7-150">POP3 App</span></span>
- <span data-ttu-id="743b7-151">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="743b7-151">IMAP4 App</span></span>
- <span data-ttu-id="743b7-152">SMTP App (Приложение с поддержкой SMTP)</span><span class="sxs-lookup"><span data-stu-id="743b7-152">SMTP App</span></span>
- <span data-ttu-id="743b7-153">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="743b7-153">Report Date</span></span>
- <span data-ttu-id="743b7-154">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="743b7-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="743b7-155">Пример</span><span class="sxs-lookup"><span data-stu-id="743b7-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="743b7-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="743b7-156">Request</span></span>

<span data-ttu-id="743b7-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="743b7-157">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="743b7-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="743b7-158">Response</span></span>

<span data-ttu-id="743b7-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="743b7-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="743b7-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="743b7-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
```
