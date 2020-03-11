---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Получите число включенных пользователей, которые активировали подписку на Office на настольных компьютерах, устройствах или общих компьютерах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0a34df3ab05166802e96256207190c3d9e278009
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590008"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="a6c37-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="a6c37-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="a6c37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6c37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a6c37-105">Получите число включенных пользователей, которые активировали подписку на Office на настольных компьютерах, устройствах или общих компьютерах.</span><span class="sxs-lookup"><span data-stu-id="a6c37-105">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="a6c37-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="a6c37-106">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6c37-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6c37-107">Permissions</span></span>

<span data-ttu-id="a6c37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6c37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6c37-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6c37-110">Permission type</span></span>                        | <span data-ttu-id="a6c37-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6c37-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a6c37-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6c37-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6c37-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6c37-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a6c37-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6c37-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6c37-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6c37-115">Not supported.</span></span>                           |
| <span data-ttu-id="a6c37-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6c37-116">Application</span></span>                            | <span data-ttu-id="a6c37-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6c37-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="a6c37-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a6c37-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a6c37-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a6c37-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a6c37-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6c37-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="a6c37-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6c37-121">Request headers</span></span>

| <span data-ttu-id="a6c37-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a6c37-122">Name</span></span>          | <span data-ttu-id="a6c37-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a6c37-123">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a6c37-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6c37-124">Authorization</span></span> | <span data-ttu-id="a6c37-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6c37-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a6c37-127">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a6c37-127">If-None-Match</span></span> | <span data-ttu-id="a6c37-128">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="a6c37-128">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a6c37-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a6c37-129">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a6c37-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6c37-130">Response</span></span>

<span data-ttu-id="a6c37-131">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="a6c37-131">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a6c37-132">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="a6c37-132">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a6c37-133">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a6c37-133">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a6c37-134">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="a6c37-134">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a6c37-135">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="a6c37-135">Report Refresh Date</span></span>
- <span data-ttu-id="a6c37-136">"Product Type" (Тип продукта);</span><span class="sxs-lookup"><span data-stu-id="a6c37-136">Product Type</span></span>
- <span data-ttu-id="a6c37-137">"Assigned" (Назначенные);</span><span class="sxs-lookup"><span data-stu-id="a6c37-137">Assigned</span></span>
- <span data-ttu-id="a6c37-138">"Activated" (Активированные).</span><span class="sxs-lookup"><span data-stu-id="a6c37-138">Activated</span></span>
- <span data-ttu-id="a6c37-139">Активация на общем компьютере</span><span class="sxs-lookup"><span data-stu-id="a6c37-139">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="a6c37-140">Пример</span><span class="sxs-lookup"><span data-stu-id="a6c37-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a6c37-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6c37-141">Request</span></span>

<span data-ttu-id="a6c37-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6c37-142">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```


#### <a name="response"></a><span data-ttu-id="a6c37-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6c37-143">Response</span></span>

<span data-ttu-id="a6c37-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a6c37-144">The following is an example of the response.</span></span>

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

<span data-ttu-id="a6c37-145">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="a6c37-145">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
