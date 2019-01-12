---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Получите сведения о пользователях, которые активировали Office 365.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 02e06e36a2329a3a302c042d71ff259b3e6c57b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978062"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="0a4f6-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="0a4f6-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="0a4f6-104">Получите сведения о пользователях, которые активировали Office 365.</span><span class="sxs-lookup"><span data-stu-id="0a4f6-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="0a4f6-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="0a4f6-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="0a4f6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a4f6-106">Permissions</span></span>

<span data-ttu-id="0a4f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a4f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a4f6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a4f6-109">Permission type</span></span>                        | <span data-ttu-id="0a4f6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a4f6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0a4f6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a4f6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a4f6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a4f6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0a4f6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a4f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a4f6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a4f6-114">Not supported.</span></span>                           |
| <span data-ttu-id="0a4f6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a4f6-115">Application</span></span>                            | <span data-ttu-id="0a4f6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a4f6-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0a4f6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a4f6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="0a4f6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a4f6-118">Request headers</span></span>

| <span data-ttu-id="0a4f6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0a4f6-119">Name</span></span>          | <span data-ttu-id="0a4f6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0a4f6-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0a4f6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a4f6-121">Authorization</span></span> | <span data-ttu-id="0a4f6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a4f6-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0a4f6-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0a4f6-124">If-None-Match</span></span> | <span data-ttu-id="0a4f6-125">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="0a4f6-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0a4f6-126">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="0a4f6-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0a4f6-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a4f6-127">Response</span></span>

<span data-ttu-id="0a4f6-128">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="0a4f6-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0a4f6-129">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="0a4f6-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0a4f6-130">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0a4f6-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0a4f6-131">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="0a4f6-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0a4f6-132">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="0a4f6-132">Report Refresh Date</span></span>
- <span data-ttu-id="0a4f6-133">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="0a4f6-133">User Principal Name</span></span>
- <span data-ttu-id="0a4f6-134">Display Name (отображаемое имя)</span><span class="sxs-lookup"><span data-stu-id="0a4f6-134">Display Name</span></span>
- <span data-ttu-id="0a4f6-135">Product Type (тип продукта)</span><span class="sxs-lookup"><span data-stu-id="0a4f6-135">Product Type</span></span>
- <span data-ttu-id="0a4f6-136">Last Activated Date (дата последней активации)</span><span class="sxs-lookup"><span data-stu-id="0a4f6-136">Last Activated Date</span></span>
- <span data-ttu-id="0a4f6-137">Windows</span><span class="sxs-lookup"><span data-stu-id="0a4f6-137">Windows</span></span>
- <span data-ttu-id="0a4f6-138">Mac</span><span class="sxs-lookup"><span data-stu-id="0a4f6-138">Mac</span></span>
- <span data-ttu-id="0a4f6-139">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="0a4f6-139">Windows 10 Mobile</span></span>
- <span data-ttu-id="0a4f6-140">iOS</span><span class="sxs-lookup"><span data-stu-id="0a4f6-140">iOS</span></span>
- <span data-ttu-id="0a4f6-141">Android</span><span class="sxs-lookup"><span data-stu-id="0a4f6-141">Android</span></span>
- <span data-ttu-id="0a4f6-142">Активированные на совместно используемый компьютер</span><span class="sxs-lookup"><span data-stu-id="0a4f6-142">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="0a4f6-143">Пример</span><span class="sxs-lookup"><span data-stu-id="0a4f6-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0a4f6-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a4f6-144">Request</span></span>

<span data-ttu-id="0a4f6-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a4f6-145">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```

#### <a name="response"></a><span data-ttu-id="0a4f6-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a4f6-146">Response</span></span>

<span data-ttu-id="0a4f6-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0a4f6-147">The following is an example of the response.</span></span>

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

<span data-ttu-id="0a4f6-148">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="0a4f6-148">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
```
