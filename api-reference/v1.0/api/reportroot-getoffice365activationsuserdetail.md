---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Получение сведений о пользователях, которые активировали Microsoft 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c009511c7001cb33321e25f853c11741c37fd6da
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897402"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="da243-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="da243-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="da243-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da243-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da243-105">Получение сведений о пользователях, которые активировали Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="da243-105">Get details about users who have activated Microsoft 365.</span></span>

> <span data-ttu-id="da243-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports — активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="da243-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="da243-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da243-107">Permissions</span></span>

<span data-ttu-id="da243-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="da243-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="da243-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da243-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da243-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da243-110">Permission type</span></span>                        | <span data-ttu-id="da243-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da243-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="da243-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da243-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="da243-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="da243-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="da243-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da243-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da243-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da243-115">Not supported.</span></span>                           |
| <span data-ttu-id="da243-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da243-116">Application</span></span>                            | <span data-ttu-id="da243-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="da243-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="da243-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da243-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="da243-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="da243-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="da243-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da243-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="da243-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da243-121">Request headers</span></span>

| <span data-ttu-id="da243-122">Имя</span><span class="sxs-lookup"><span data-stu-id="da243-122">Name</span></span>          | <span data-ttu-id="da243-123">Описание</span><span class="sxs-lookup"><span data-stu-id="da243-123">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="da243-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da243-124">Authorization</span></span> | <span data-ttu-id="da243-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="da243-125">Bearer {token}.</span></span> <span data-ttu-id="da243-126">Required.</span><span class="sxs-lookup"><span data-stu-id="da243-126">Required.</span></span>                |
| <span data-ttu-id="da243-127">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="da243-127">If-None-Match</span></span> | <span data-ttu-id="da243-128">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="da243-128">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="da243-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="da243-129">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="da243-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="da243-130">Response</span></span>

<span data-ttu-id="da243-131">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="da243-131">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="da243-132">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="da243-132">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="da243-133">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="da243-133">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="da243-134">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="da243-134">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="da243-135">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="da243-135">Report Refresh Date</span></span>
- <span data-ttu-id="da243-136">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="da243-136">User Principal Name</span></span>
- <span data-ttu-id="da243-137">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="da243-137">Display Name</span></span>
- <span data-ttu-id="da243-138">Product Type (тип продукта)</span><span class="sxs-lookup"><span data-stu-id="da243-138">Product Type</span></span>
- <span data-ttu-id="da243-139">Last Activated Date (дата последней активации)</span><span class="sxs-lookup"><span data-stu-id="da243-139">Last Activated Date</span></span>
- <span data-ttu-id="da243-140">Windows</span><span class="sxs-lookup"><span data-stu-id="da243-140">Windows</span></span>
- <span data-ttu-id="da243-141">Mac</span><span class="sxs-lookup"><span data-stu-id="da243-141">Mac</span></span>
- <span data-ttu-id="da243-142">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="da243-142">Windows 10 Mobile</span></span>
- <span data-ttu-id="da243-143">iOS</span><span class="sxs-lookup"><span data-stu-id="da243-143">iOS</span></span>
- <span data-ttu-id="da243-144">Android</span><span class="sxs-lookup"><span data-stu-id="da243-144">Android</span></span>
- <span data-ttu-id="da243-145">Активирован на общем компьютере</span><span class="sxs-lookup"><span data-stu-id="da243-145">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="da243-146">Пример</span><span class="sxs-lookup"><span data-stu-id="da243-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="da243-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="da243-147">Request</span></span>

<span data-ttu-id="da243-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da243-148">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```


#### <a name="response"></a><span data-ttu-id="da243-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="da243-149">Response</span></span>

<span data-ttu-id="da243-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da243-150">The following is an example of the response.</span></span>

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

<span data-ttu-id="da243-151">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="da243-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
