---
title: 'reportRoot: getOffice365ActivationCounts'
description: Получение числа активаций Microsoft 365 на настольных компьютерах и устройствах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e95b2bd30b34abb7cb9d4dec5920c3ef43725272
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897416"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="0288e-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="0288e-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="0288e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0288e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0288e-105">Получение числа активаций Microsoft 365 на настольных компьютерах и устройствах.</span><span class="sxs-lookup"><span data-stu-id="0288e-105">Get the count of Microsoft 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="0288e-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports — активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="0288e-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="0288e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0288e-107">Permissions</span></span>

<span data-ttu-id="0288e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0288e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0288e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0288e-110">Permission type</span></span>                        | <span data-ttu-id="0288e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0288e-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0288e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0288e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0288e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0288e-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0288e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0288e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0288e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0288e-115">Not supported.</span></span>                           |
| <span data-ttu-id="0288e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0288e-116">Application</span></span>                            | <span data-ttu-id="0288e-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0288e-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="0288e-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0288e-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="0288e-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="0288e-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="0288e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0288e-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="0288e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0288e-121">Request headers</span></span>

| <span data-ttu-id="0288e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0288e-122">Name</span></span>          | <span data-ttu-id="0288e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0288e-123">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0288e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0288e-124">Authorization</span></span> | <span data-ttu-id="0288e-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0288e-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0288e-127">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0288e-127">If-None-Match</span></span> | <span data-ttu-id="0288e-128">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="0288e-128">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0288e-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="0288e-129">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0288e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0288e-130">Response</span></span>

<span data-ttu-id="0288e-131">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="0288e-131">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0288e-132">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="0288e-132">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0288e-133">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0288e-133">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0288e-134">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="0288e-134">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0288e-135">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="0288e-135">Report Refresh Date</span></span>
- <span data-ttu-id="0288e-136">Product Type (Тип продукта)</span><span class="sxs-lookup"><span data-stu-id="0288e-136">Product Type</span></span>
- <span data-ttu-id="0288e-137">Windows</span><span class="sxs-lookup"><span data-stu-id="0288e-137">Windows</span></span>
- <span data-ttu-id="0288e-138">Mac</span><span class="sxs-lookup"><span data-stu-id="0288e-138">Mac</span></span>
- <span data-ttu-id="0288e-139">Android</span><span class="sxs-lookup"><span data-stu-id="0288e-139">Android</span></span>
- <span data-ttu-id="0288e-140">iOS</span><span class="sxs-lookup"><span data-stu-id="0288e-140">iOS</span></span>
- <span data-ttu-id="0288e-141">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="0288e-141">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="0288e-142">Пример</span><span class="sxs-lookup"><span data-stu-id="0288e-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0288e-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="0288e-143">Request</span></span>

<span data-ttu-id="0288e-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0288e-144">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activationcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```


#### <a name="response"></a><span data-ttu-id="0288e-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="0288e-145">Response</span></span>

<span data-ttu-id="0288e-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0288e-146">The following is an example of the response.</span></span>

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

<span data-ttu-id="0288e-147">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="0288e-147">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
