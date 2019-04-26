---
title: 'reportRoot: getOffice365ActivationCounts'
description: Получите количество активаций Office 365 на компьютерах и мобильных устройствах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 31aed10d7a2b70c32f0654df67dfa86385d5fd17
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582341"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="4e520-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="4e520-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="4e520-104">Получите количество активаций Office 365 на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="4e520-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="4e520-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="4e520-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="4e520-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e520-106">Permissions</span></span>

<span data-ttu-id="4e520-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4e520-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e520-109">Permission type</span></span>                        | <span data-ttu-id="4e520-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e520-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4e520-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e520-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e520-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e520-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4e520-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e520-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e520-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e520-114">Not supported.</span></span>                           |
| <span data-ttu-id="4e520-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e520-115">Application</span></span>                            | <span data-ttu-id="4e520-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e520-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4e520-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e520-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="4e520-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e520-118">Request headers</span></span>

| <span data-ttu-id="4e520-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4e520-119">Name</span></span>          | <span data-ttu-id="4e520-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4e520-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4e520-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e520-121">Authorization</span></span> | <span data-ttu-id="4e520-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e520-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4e520-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4e520-124">If-None-Match</span></span> | <span data-ttu-id="4e520-125">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="4e520-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4e520-126">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4e520-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4e520-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e520-127">Response</span></span>

<span data-ttu-id="4e520-128">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4e520-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4e520-129">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4e520-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4e520-130">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4e520-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4e520-131">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4e520-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4e520-132">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4e520-132">Report Refresh Date</span></span>
- <span data-ttu-id="4e520-133">Product Type (Тип продукта)</span><span class="sxs-lookup"><span data-stu-id="4e520-133">Product Type</span></span>
- <span data-ttu-id="4e520-134">Windows</span><span class="sxs-lookup"><span data-stu-id="4e520-134">Windows</span></span>
- <span data-ttu-id="4e520-135">Mac</span><span class="sxs-lookup"><span data-stu-id="4e520-135">Mac</span></span>
- <span data-ttu-id="4e520-136">Android</span><span class="sxs-lookup"><span data-stu-id="4e520-136">Android</span></span>
- <span data-ttu-id="4e520-137">iOS</span><span class="sxs-lookup"><span data-stu-id="4e520-137">iOS</span></span>
- <span data-ttu-id="4e520-138">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="4e520-138">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="4e520-139">Пример</span><span class="sxs-lookup"><span data-stu-id="4e520-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4e520-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e520-140">Request</span></span>

<span data-ttu-id="4e520-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e520-141">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```

#### <a name="response"></a><span data-ttu-id="4e520-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e520-142">Response</span></span>

<span data-ttu-id="4e520-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4e520-143">The following is an example of the response.</span></span>

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

<span data-ttu-id="4e520-144">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4e520-144">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```
