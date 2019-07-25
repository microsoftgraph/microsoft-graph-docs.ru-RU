---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Получите сведения о пользователях, которые активировали Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9df409f6dbe3943a2adda64953e9be10e43bc4e1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881062"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="cbfc2-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="cbfc2-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="cbfc2-104">Получите сведения о пользователях, которые активировали Office 365.</span><span class="sxs-lookup"><span data-stu-id="cbfc2-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="cbfc2-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="cbfc2-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="cbfc2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cbfc2-106">Permissions</span></span>

<span data-ttu-id="cbfc2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbfc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cbfc2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbfc2-109">Permission type</span></span>                        | <span data-ttu-id="cbfc2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbfc2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cbfc2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbfc2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cbfc2-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbfc2-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cbfc2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbfc2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbfc2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbfc2-114">Not supported.</span></span>                           |
| <span data-ttu-id="cbfc2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbfc2-115">Application</span></span>                            | <span data-ttu-id="cbfc2-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbfc2-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cbfc2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbfc2-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cbfc2-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbfc2-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="cbfc2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbfc2-119">Request headers</span></span>

| <span data-ttu-id="cbfc2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="cbfc2-120">Name</span></span>          | <span data-ttu-id="cbfc2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cbfc2-121">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="cbfc2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cbfc2-122">Authorization</span></span> | <span data-ttu-id="cbfc2-p102">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbfc2-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="cbfc2-125">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="cbfc2-125">If-None-Match</span></span> | <span data-ttu-id="cbfc2-126">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="cbfc2-126">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="cbfc2-127">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cbfc2-127">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="cbfc2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbfc2-128">Response</span></span>

<span data-ttu-id="cbfc2-129">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="cbfc2-129">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cbfc2-130">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="cbfc2-130">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cbfc2-131">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cbfc2-131">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cbfc2-132">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="cbfc2-132">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cbfc2-133">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="cbfc2-133">Report Refresh Date</span></span>
- <span data-ttu-id="cbfc2-134">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="cbfc2-134">User Principal Name</span></span>
- <span data-ttu-id="cbfc2-135">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="cbfc2-135">Display Name</span></span>
- <span data-ttu-id="cbfc2-136">Product Type (тип продукта)</span><span class="sxs-lookup"><span data-stu-id="cbfc2-136">Product Type</span></span>
- <span data-ttu-id="cbfc2-137">Last Activated Date (дата последней активации)</span><span class="sxs-lookup"><span data-stu-id="cbfc2-137">Last Activated Date</span></span>
- <span data-ttu-id="cbfc2-138">Windows</span><span class="sxs-lookup"><span data-stu-id="cbfc2-138">Windows</span></span>
- <span data-ttu-id="cbfc2-139">Mac</span><span class="sxs-lookup"><span data-stu-id="cbfc2-139">Mac</span></span>
- <span data-ttu-id="cbfc2-140">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="cbfc2-140">Windows 10 Mobile</span></span>
- <span data-ttu-id="cbfc2-141">iOS</span><span class="sxs-lookup"><span data-stu-id="cbfc2-141">iOS</span></span>
- <span data-ttu-id="cbfc2-142">Android</span><span class="sxs-lookup"><span data-stu-id="cbfc2-142">Android</span></span>
- <span data-ttu-id="cbfc2-143">Активирован на общем компьютере</span><span class="sxs-lookup"><span data-stu-id="cbfc2-143">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="cbfc2-144">Пример</span><span class="sxs-lookup"><span data-stu-id="cbfc2-144">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cbfc2-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbfc2-145">Request</span></span>

<span data-ttu-id="cbfc2-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbfc2-146">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cbfc2-147">C#</span><span class="sxs-lookup"><span data-stu-id="cbfc2-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cbfc2-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="cbfc2-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cbfc2-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cbfc2-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cbfc2-150">Java</span><span class="sxs-lookup"><span data-stu-id="cbfc2-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cbfc2-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="cbfc2-151">Response</span></span>

<span data-ttu-id="cbfc2-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cbfc2-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="cbfc2-153">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="cbfc2-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
