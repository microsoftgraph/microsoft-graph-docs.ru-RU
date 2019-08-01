---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Получите число включенных пользователей, которые активировали подписку на Office на настольных компьютерах, устройствах или общих компьютерах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0f6f27dcec75cf8a761fa4f8115962e3f444b923
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025094"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="ec795-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="ec795-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="ec795-104">Получите число включенных пользователей, которые активировали подписку на Office на настольных компьютерах, устройствах или общих компьютерах.</span><span class="sxs-lookup"><span data-stu-id="ec795-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="ec795-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="ec795-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="ec795-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec795-106">Permissions</span></span>

<span data-ttu-id="ec795-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec795-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec795-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec795-109">Permission type</span></span>                        | <span data-ttu-id="ec795-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec795-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ec795-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec795-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec795-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec795-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ec795-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec795-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec795-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec795-114">Not supported.</span></span>                           |
| <span data-ttu-id="ec795-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec795-115">Application</span></span>                            | <span data-ttu-id="ec795-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec795-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ec795-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec795-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ec795-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec795-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="ec795-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec795-119">Request headers</span></span>

| <span data-ttu-id="ec795-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ec795-120">Name</span></span>          | <span data-ttu-id="ec795-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ec795-121">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ec795-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec795-122">Authorization</span></span> | <span data-ttu-id="ec795-p102">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec795-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ec795-125">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ec795-125">If-None-Match</span></span> | <span data-ttu-id="ec795-126">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="ec795-126">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ec795-127">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ec795-127">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ec795-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec795-128">Response</span></span>

<span data-ttu-id="ec795-129">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ec795-129">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ec795-130">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ec795-130">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ec795-131">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ec795-131">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ec795-132">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ec795-132">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ec795-133">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ec795-133">Report Refresh Date</span></span>
- <span data-ttu-id="ec795-134">"Product Type" (Тип продукта);</span><span class="sxs-lookup"><span data-stu-id="ec795-134">Product Type</span></span>
- <span data-ttu-id="ec795-135">"Assigned" (Назначенные);</span><span class="sxs-lookup"><span data-stu-id="ec795-135">Assigned</span></span>
- <span data-ttu-id="ec795-136">"Activated" (Активированные).</span><span class="sxs-lookup"><span data-stu-id="ec795-136">Activated</span></span>
- <span data-ttu-id="ec795-137">Активация на общем компьютере</span><span class="sxs-lookup"><span data-stu-id="ec795-137">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="ec795-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ec795-138">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ec795-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec795-139">Request</span></span>

<span data-ttu-id="ec795-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec795-140">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ec795-141">C#</span><span class="sxs-lookup"><span data-stu-id="ec795-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ec795-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="ec795-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ec795-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ec795-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ec795-144">Java</span><span class="sxs-lookup"><span data-stu-id="ec795-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ec795-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec795-145">Response</span></span>

<span data-ttu-id="ec795-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ec795-146">The following is an example of the response.</span></span>

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

<span data-ttu-id="ec795-147">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ec795-147">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
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
