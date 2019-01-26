---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Получение числа пользователей, для которых включено и те, которые активации подписки Office на настольных ПК или устройства или на общедоступном компьютере.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9a150911e9234cde7258acbeed7f825fb9db4c66
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576103"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="9cbb9-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="9cbb9-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="9cbb9-104">Получение числа пользователей, для которых включено и те, которые активации подписки Office на настольных ПК или устройства или на общедоступном компьютере.</span><span class="sxs-lookup"><span data-stu-id="9cbb9-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="9cbb9-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="9cbb9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="9cbb9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9cbb9-106">Permissions</span></span>

<span data-ttu-id="9cbb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cbb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9cbb9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cbb9-109">Permission type</span></span>                        | <span data-ttu-id="9cbb9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cbb9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9cbb9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cbb9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cbb9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cbb9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9cbb9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cbb9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cbb9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cbb9-114">Not supported.</span></span>                           |
| <span data-ttu-id="9cbb9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cbb9-115">Application</span></span>                            | <span data-ttu-id="9cbb9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cbb9-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9cbb9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cbb9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="9cbb9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9cbb9-118">Request headers</span></span>

| <span data-ttu-id="9cbb9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9cbb9-119">Name</span></span>          | <span data-ttu-id="9cbb9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9cbb9-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="9cbb9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cbb9-121">Authorization</span></span> | <span data-ttu-id="9cbb9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cbb9-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="9cbb9-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9cbb9-124">If-None-Match</span></span> | <span data-ttu-id="9cbb9-125">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="9cbb9-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="9cbb9-126">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9cbb9-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9cbb9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cbb9-127">Response</span></span>

<span data-ttu-id="9cbb9-128">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="9cbb9-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9cbb9-129">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="9cbb9-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9cbb9-130">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9cbb9-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9cbb9-131">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="9cbb9-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9cbb9-132">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="9cbb9-132">Report Refresh Date</span></span>
- <span data-ttu-id="9cbb9-133">"Product Type" (Тип продукта);</span><span class="sxs-lookup"><span data-stu-id="9cbb9-133">Product Type</span></span>
- <span data-ttu-id="9cbb9-134">"Assigned" (Назначенные);</span><span class="sxs-lookup"><span data-stu-id="9cbb9-134">Assigned</span></span>
- <span data-ttu-id="9cbb9-135">"Activated" (Активированные).</span><span class="sxs-lookup"><span data-stu-id="9cbb9-135">Activated</span></span>
- <span data-ttu-id="9cbb9-136">Активация совместно используемый компьютер</span><span class="sxs-lookup"><span data-stu-id="9cbb9-136">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="9cbb9-137">Пример</span><span class="sxs-lookup"><span data-stu-id="9cbb9-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9cbb9-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cbb9-138">Request</span></span>

<span data-ttu-id="9cbb9-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cbb9-139">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```

#### <a name="response"></a><span data-ttu-id="9cbb9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cbb9-140">Response</span></span>

<span data-ttu-id="9cbb9-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9cbb9-141">The following is an example of the response.</span></span>

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

<span data-ttu-id="9cbb9-142">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="9cbb9-142">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```
