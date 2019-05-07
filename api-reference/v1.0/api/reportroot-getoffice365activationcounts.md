---
title: 'reportRoot: getOffice365ActivationCounts'
description: Получите количество активаций Office 365 на компьютерах и мобильных устройствах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1180ed5730475801821d43379789c1d688919bba
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33606720"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="ecbae-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="ecbae-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="ecbae-104">Получите количество активаций Office 365 на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="ecbae-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="ecbae-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="ecbae-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="ecbae-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ecbae-106">Permissions</span></span>

<span data-ttu-id="ecbae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecbae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ecbae-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecbae-109">Permission type</span></span>                        | <span data-ttu-id="ecbae-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecbae-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ecbae-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecbae-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ecbae-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecbae-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ecbae-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecbae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecbae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecbae-114">Not supported.</span></span>                           |
| <span data-ttu-id="ecbae-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecbae-115">Application</span></span>                            | <span data-ttu-id="ecbae-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecbae-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ecbae-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecbae-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="ecbae-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecbae-118">Request headers</span></span>

| <span data-ttu-id="ecbae-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ecbae-119">Name</span></span>          | <span data-ttu-id="ecbae-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ecbae-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ecbae-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecbae-121">Authorization</span></span> | <span data-ttu-id="ecbae-p102">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecbae-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ecbae-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ecbae-124">If-None-Match</span></span> | <span data-ttu-id="ecbae-125">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="ecbae-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ecbae-126">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ecbae-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ecbae-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecbae-127">Response</span></span>

<span data-ttu-id="ecbae-128">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ecbae-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ecbae-129">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ecbae-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ecbae-130">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ecbae-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ecbae-131">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ecbae-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ecbae-132">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ecbae-132">Report Refresh Date</span></span>
- <span data-ttu-id="ecbae-133">Product Type (Тип продукта)</span><span class="sxs-lookup"><span data-stu-id="ecbae-133">Product Type</span></span>
- <span data-ttu-id="ecbae-134">Windows</span><span class="sxs-lookup"><span data-stu-id="ecbae-134">Windows</span></span>
- <span data-ttu-id="ecbae-135">Mac</span><span class="sxs-lookup"><span data-stu-id="ecbae-135">Mac</span></span>
- <span data-ttu-id="ecbae-136">Android</span><span class="sxs-lookup"><span data-stu-id="ecbae-136">Android</span></span>
- <span data-ttu-id="ecbae-137">iOS</span><span class="sxs-lookup"><span data-stu-id="ecbae-137">iOS</span></span>
- <span data-ttu-id="ecbae-138">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="ecbae-138">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="ecbae-139">Пример</span><span class="sxs-lookup"><span data-stu-id="ecbae-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ecbae-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecbae-140">Request</span></span>

<span data-ttu-id="ecbae-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecbae-141">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```

#### <a name="response"></a><span data-ttu-id="ecbae-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="ecbae-142">Response</span></span>

<span data-ttu-id="ecbae-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ecbae-143">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ecbae-144">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="ecbae-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ecbae-145">Языках</span><span class="sxs-lookup"><span data-stu-id="ecbae-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ecbae-146">Язык</span><span class="sxs-lookup"><span data-stu-id="ecbae-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="ecbae-147">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ecbae-147">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
