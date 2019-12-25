---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Получите сведения о пользователях, которые активировали Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e403643b01315741cc28c19b32c1aed0b2409e6c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865428"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="c8b41-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="c8b41-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="c8b41-104">Получите сведения о пользователях, которые активировали Office 365.</span><span class="sxs-lookup"><span data-stu-id="c8b41-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="c8b41-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="c8b41-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="c8b41-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8b41-106">Permissions</span></span>

<span data-ttu-id="c8b41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8b41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8b41-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8b41-109">Permission type</span></span>                        | <span data-ttu-id="c8b41-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8b41-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c8b41-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8b41-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8b41-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8b41-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c8b41-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8b41-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8b41-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8b41-114">Not supported.</span></span>                           |
| <span data-ttu-id="c8b41-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8b41-115">Application</span></span>                            | <span data-ttu-id="c8b41-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8b41-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="c8b41-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c8b41-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="c8b41-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="c8b41-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="c8b41-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8b41-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="c8b41-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8b41-120">Request headers</span></span>

| <span data-ttu-id="c8b41-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c8b41-121">Name</span></span>          | <span data-ttu-id="c8b41-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c8b41-122">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c8b41-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8b41-123">Authorization</span></span> | <span data-ttu-id="c8b41-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8b41-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c8b41-126">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c8b41-126">If-None-Match</span></span> | <span data-ttu-id="c8b41-127">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="c8b41-127">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c8b41-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c8b41-128">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c8b41-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8b41-129">Response</span></span>

<span data-ttu-id="c8b41-130">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c8b41-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c8b41-131">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c8b41-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c8b41-132">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c8b41-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c8b41-133">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c8b41-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c8b41-134">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c8b41-134">Report Refresh Date</span></span>
- <span data-ttu-id="c8b41-135">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="c8b41-135">User Principal Name</span></span>
- <span data-ttu-id="c8b41-136">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="c8b41-136">Display Name</span></span>
- <span data-ttu-id="c8b41-137">Product Type (тип продукта)</span><span class="sxs-lookup"><span data-stu-id="c8b41-137">Product Type</span></span>
- <span data-ttu-id="c8b41-138">Last Activated Date (дата последней активации)</span><span class="sxs-lookup"><span data-stu-id="c8b41-138">Last Activated Date</span></span>
- <span data-ttu-id="c8b41-139">Windows</span><span class="sxs-lookup"><span data-stu-id="c8b41-139">Windows</span></span>
- <span data-ttu-id="c8b41-140">Mac</span><span class="sxs-lookup"><span data-stu-id="c8b41-140">Mac</span></span>
- <span data-ttu-id="c8b41-141">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="c8b41-141">Windows 10 Mobile</span></span>
- <span data-ttu-id="c8b41-142">iOS</span><span class="sxs-lookup"><span data-stu-id="c8b41-142">iOS</span></span>
- <span data-ttu-id="c8b41-143">Android</span><span class="sxs-lookup"><span data-stu-id="c8b41-143">Android</span></span>
- <span data-ttu-id="c8b41-144">Активирован на общем компьютере</span><span class="sxs-lookup"><span data-stu-id="c8b41-144">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="c8b41-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c8b41-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c8b41-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8b41-146">Request</span></span>

<span data-ttu-id="c8b41-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8b41-147">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c8b41-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8b41-148">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c8b41-149">C#</span><span class="sxs-lookup"><span data-stu-id="c8b41-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8b41-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8b41-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c8b41-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8b41-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c8b41-152">Java</span><span class="sxs-lookup"><span data-stu-id="c8b41-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c8b41-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8b41-153">Response</span></span>

<span data-ttu-id="c8b41-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c8b41-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="c8b41-155">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c8b41-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
