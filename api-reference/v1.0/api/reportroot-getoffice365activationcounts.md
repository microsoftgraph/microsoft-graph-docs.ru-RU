---
title: 'reportRoot: getOffice365ActivationCounts'
description: Получите количество активаций Office 365 на компьютерах и мобильных устройствах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 43df5c8bc681fae23493c8a578b95e894fed107d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327194"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="48ffd-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="48ffd-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="48ffd-104">Получите количество активаций Office 365 на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="48ffd-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="48ffd-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="48ffd-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="48ffd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48ffd-106">Permissions</span></span>

<span data-ttu-id="48ffd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48ffd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48ffd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48ffd-109">Permission type</span></span>                        | <span data-ttu-id="48ffd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48ffd-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="48ffd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48ffd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="48ffd-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="48ffd-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="48ffd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48ffd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48ffd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48ffd-114">Not supported.</span></span>                           |
| <span data-ttu-id="48ffd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48ffd-115">Application</span></span>                            | <span data-ttu-id="48ffd-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="48ffd-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="48ffd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48ffd-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="48ffd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48ffd-118">Request headers</span></span>

| <span data-ttu-id="48ffd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="48ffd-119">Name</span></span>          | <span data-ttu-id="48ffd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="48ffd-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="48ffd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48ffd-121">Authorization</span></span> | <span data-ttu-id="48ffd-p102">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48ffd-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="48ffd-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="48ffd-124">If-None-Match</span></span> | <span data-ttu-id="48ffd-125">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="48ffd-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="48ffd-126">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="48ffd-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="48ffd-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="48ffd-127">Response</span></span>

<span data-ttu-id="48ffd-128">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="48ffd-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="48ffd-129">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="48ffd-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="48ffd-130">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="48ffd-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="48ffd-131">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="48ffd-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="48ffd-132">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="48ffd-132">Report Refresh Date</span></span>
- <span data-ttu-id="48ffd-133">Product Type (Тип продукта)</span><span class="sxs-lookup"><span data-stu-id="48ffd-133">Product Type</span></span>
- <span data-ttu-id="48ffd-134">Windows</span><span class="sxs-lookup"><span data-stu-id="48ffd-134">Windows</span></span>
- <span data-ttu-id="48ffd-135">Mac</span><span class="sxs-lookup"><span data-stu-id="48ffd-135">Mac</span></span>
- <span data-ttu-id="48ffd-136">Android</span><span class="sxs-lookup"><span data-stu-id="48ffd-136">Android</span></span>
- <span data-ttu-id="48ffd-137">iOS</span><span class="sxs-lookup"><span data-stu-id="48ffd-137">iOS</span></span>
- <span data-ttu-id="48ffd-138">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="48ffd-138">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="48ffd-139">Пример</span><span class="sxs-lookup"><span data-stu-id="48ffd-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="48ffd-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="48ffd-140">Request</span></span>

<span data-ttu-id="48ffd-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48ffd-141">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="48ffd-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="48ffd-142">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48ffd-143">C#</span><span class="sxs-lookup"><span data-stu-id="48ffd-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48ffd-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48ffd-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48ffd-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="48ffd-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="48ffd-146">Java</span><span class="sxs-lookup"><span data-stu-id="48ffd-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="48ffd-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="48ffd-147">Response</span></span>

<span data-ttu-id="48ffd-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="48ffd-148">The following is an example of the response.</span></span>

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

<span data-ttu-id="48ffd-149">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="48ffd-149">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
