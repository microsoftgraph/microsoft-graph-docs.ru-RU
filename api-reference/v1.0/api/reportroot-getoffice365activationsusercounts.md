---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Получение числа пользователей, для которых включено и те, которые активации подписки Office на настольных ПК или устройства или на общедоступном компьютере.
localization_priority: Normal
ms.openlocfilehash: 79f6f67525aa500fd6e852a5b1322166769caff7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875707"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="5c5ba-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="5c5ba-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="5c5ba-104">Получение числа пользователей, для которых включено и те, которые активации подписки Office на настольных ПК или устройства или на общедоступном компьютере.</span><span class="sxs-lookup"><span data-stu-id="5c5ba-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="5c5ba-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="5c5ba-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="5c5ba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c5ba-106">Permissions</span></span>

<span data-ttu-id="5c5ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c5ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c5ba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c5ba-109">Permission type</span></span>                        | <span data-ttu-id="5c5ba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c5ba-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5c5ba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c5ba-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c5ba-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c5ba-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5c5ba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c5ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c5ba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c5ba-114">Not supported.</span></span>                           |
| <span data-ttu-id="5c5ba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c5ba-115">Application</span></span>                            | <span data-ttu-id="5c5ba-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c5ba-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5c5ba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c5ba-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="5c5ba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c5ba-118">Request headers</span></span>

| <span data-ttu-id="5c5ba-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5c5ba-119">Name</span></span>          | <span data-ttu-id="5c5ba-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5c5ba-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5c5ba-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c5ba-121">Authorization</span></span> | <span data-ttu-id="5c5ba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c5ba-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5c5ba-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5c5ba-124">If-None-Match</span></span> | <span data-ttu-id="5c5ba-125">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="5c5ba-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5c5ba-126">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5c5ba-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5c5ba-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c5ba-127">Response</span></span>

<span data-ttu-id="5c5ba-128">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="5c5ba-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5c5ba-129">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="5c5ba-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5c5ba-130">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5c5ba-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5c5ba-131">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="5c5ba-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5c5ba-132">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="5c5ba-132">Report Refresh Date</span></span>
- <span data-ttu-id="5c5ba-133">"Product Type" (Тип продукта);</span><span class="sxs-lookup"><span data-stu-id="5c5ba-133">Product Type</span></span>
- <span data-ttu-id="5c5ba-134">"Assigned" (Назначенные);</span><span class="sxs-lookup"><span data-stu-id="5c5ba-134">Assigned</span></span>
- <span data-ttu-id="5c5ba-135">"Activated" (Активированные).</span><span class="sxs-lookup"><span data-stu-id="5c5ba-135">Activated</span></span>
- <span data-ttu-id="5c5ba-136">Активация совместно используемый компьютер</span><span class="sxs-lookup"><span data-stu-id="5c5ba-136">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="5c5ba-137">Пример</span><span class="sxs-lookup"><span data-stu-id="5c5ba-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5c5ba-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c5ba-138">Request</span></span>

<span data-ttu-id="5c5ba-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c5ba-139">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```

#### <a name="response"></a><span data-ttu-id="5c5ba-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c5ba-140">Response</span></span>

<span data-ttu-id="5c5ba-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5c5ba-141">The following is an example of the response.</span></span>

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

<span data-ttu-id="5c5ba-142">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="5c5ba-142">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```
