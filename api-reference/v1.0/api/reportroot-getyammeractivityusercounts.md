---
title: 'reportRoot: getYammerActivityUserCounts'
description: Отслеживайте динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5449d0adcf6a676572987293130d4c7b0b3ad443
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575400"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="3d16a-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="3d16a-103">reportRoot: getYammerActivityUserCounts</span></span>

<span data-ttu-id="3d16a-104">Отслеживайте динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer.</span><span class="sxs-lookup"><span data-stu-id="3d16a-104">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="3d16a-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="3d16a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="3d16a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d16a-106">Permissions</span></span>

<span data-ttu-id="3d16a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d16a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3d16a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d16a-109">Permission type</span></span>                        | <span data-ttu-id="3d16a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d16a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3d16a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d16a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3d16a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d16a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3d16a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d16a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d16a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d16a-114">Not supported.</span></span>                           |
| <span data-ttu-id="3d16a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d16a-115">Application</span></span>                            | <span data-ttu-id="3d16a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d16a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3d16a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d16a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3d16a-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3d16a-118">Function parameters</span></span>

<span data-ttu-id="3d16a-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3d16a-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3d16a-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="3d16a-120">Parameter</span></span> | <span data-ttu-id="3d16a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3d16a-121">Type</span></span>   | <span data-ttu-id="3d16a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3d16a-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3d16a-123">period</span><span class="sxs-lookup"><span data-stu-id="3d16a-123">period</span></span>    | <span data-ttu-id="3d16a-124">строка</span><span class="sxs-lookup"><span data-stu-id="3d16a-124">string</span></span> | <span data-ttu-id="3d16a-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3d16a-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3d16a-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3d16a-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3d16a-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3d16a-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3d16a-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d16a-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3d16a-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d16a-129">Request headers</span></span>

| <span data-ttu-id="3d16a-130">Имя</span><span class="sxs-lookup"><span data-stu-id="3d16a-130">Name</span></span>          | <span data-ttu-id="3d16a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3d16a-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3d16a-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d16a-132">Authorization</span></span> | <span data-ttu-id="3d16a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d16a-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3d16a-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3d16a-135">If-None-Match</span></span> | <span data-ttu-id="3d16a-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="3d16a-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3d16a-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3d16a-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3d16a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d16a-138">Response</span></span>

<span data-ttu-id="3d16a-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3d16a-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3d16a-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3d16a-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3d16a-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3d16a-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3d16a-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3d16a-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3d16a-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3d16a-143">Report Refresh Date</span></span>
- <span data-ttu-id="3d16a-144">"Liked" (Понравилось);</span><span class="sxs-lookup"><span data-stu-id="3d16a-144">Liked</span></span>
- <span data-ttu-id="3d16a-145">"Posted" (Опубликовано);</span><span class="sxs-lookup"><span data-stu-id="3d16a-145">Posted</span></span>
- <span data-ttu-id="3d16a-146">"Read" (Чтение);</span><span class="sxs-lookup"><span data-stu-id="3d16a-146">Read</span></span>
- <span data-ttu-id="3d16a-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="3d16a-147">Report Date</span></span>
- <span data-ttu-id="3d16a-148">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="3d16a-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3d16a-149">Пример</span><span class="sxs-lookup"><span data-stu-id="3d16a-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3d16a-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d16a-150">Request</span></span>

<span data-ttu-id="3d16a-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d16a-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="3d16a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d16a-152">Response</span></span>

<span data-ttu-id="3d16a-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3d16a-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="3d16a-154">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3d16a-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```
