---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Получите сведения о пользователях, которые активировали Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4f16e070f2ac39e83b70185192bf19d09eab1038
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460611"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="94513-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="94513-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="94513-104">Получите сведения о пользователях, которые активировали Office 365.</span><span class="sxs-lookup"><span data-stu-id="94513-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="94513-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="94513-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="94513-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94513-106">Permissions</span></span>

<span data-ttu-id="94513-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94513-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94513-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94513-109">Permission type</span></span>                        | <span data-ttu-id="94513-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94513-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="94513-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94513-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="94513-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="94513-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="94513-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94513-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94513-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94513-114">Not supported.</span></span>                           |
| <span data-ttu-id="94513-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94513-115">Application</span></span>                            | <span data-ttu-id="94513-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="94513-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="94513-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94513-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="94513-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="94513-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="94513-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94513-119">Request headers</span></span>

| <span data-ttu-id="94513-120">Имя</span><span class="sxs-lookup"><span data-stu-id="94513-120">Name</span></span>          | <span data-ttu-id="94513-121">Описание</span><span class="sxs-lookup"><span data-stu-id="94513-121">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="94513-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94513-122">Authorization</span></span> | <span data-ttu-id="94513-p102">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94513-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="94513-125">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="94513-125">If-None-Match</span></span> | <span data-ttu-id="94513-126">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="94513-126">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="94513-127">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="94513-127">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="94513-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="94513-128">Response</span></span>

<span data-ttu-id="94513-129">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="94513-129">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="94513-130">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="94513-130">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="94513-131">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="94513-131">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="94513-132">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="94513-132">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="94513-133">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="94513-133">Report Refresh Date</span></span>
- <span data-ttu-id="94513-134">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="94513-134">User Principal Name</span></span>
- <span data-ttu-id="94513-135">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="94513-135">Display Name</span></span>
- <span data-ttu-id="94513-136">Product Type (тип продукта)</span><span class="sxs-lookup"><span data-stu-id="94513-136">Product Type</span></span>
- <span data-ttu-id="94513-137">Last Activated Date (дата последней активации)</span><span class="sxs-lookup"><span data-stu-id="94513-137">Last Activated Date</span></span>
- <span data-ttu-id="94513-138">Windows</span><span class="sxs-lookup"><span data-stu-id="94513-138">Windows</span></span>
- <span data-ttu-id="94513-139">Mac</span><span class="sxs-lookup"><span data-stu-id="94513-139">Mac</span></span>
- <span data-ttu-id="94513-140">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="94513-140">Windows 10 Mobile</span></span>
- <span data-ttu-id="94513-141">iOS</span><span class="sxs-lookup"><span data-stu-id="94513-141">iOS</span></span>
- <span data-ttu-id="94513-142">Android</span><span class="sxs-lookup"><span data-stu-id="94513-142">Android</span></span>
- <span data-ttu-id="94513-143">Активирован на общем компьютере</span><span class="sxs-lookup"><span data-stu-id="94513-143">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="94513-144">Пример</span><span class="sxs-lookup"><span data-stu-id="94513-144">Example</span></span>

#### <a name="request"></a><span data-ttu-id="94513-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="94513-145">Request</span></span>

<span data-ttu-id="94513-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94513-146">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="94513-147">C#</span><span class="sxs-lookup"><span data-stu-id="94513-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94513-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="94513-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94513-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="94513-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94513-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="94513-150">Response</span></span>

<span data-ttu-id="94513-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="94513-151">The following is an example of the response.</span></span>

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

<span data-ttu-id="94513-152">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="94513-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
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
