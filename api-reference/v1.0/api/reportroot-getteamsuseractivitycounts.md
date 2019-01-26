---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Получение количества действий в Microsoft Teams по каждому типу. К типам действий относятся сообщения в чатах групп, сообщения в приватных чатах, звонки и собрания.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4a47a85748fe2cfa195da0654b980541908ae71f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572817"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="63d99-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="63d99-104">reportRoot: getTeamsUserActivityCounts</span></span>

<span data-ttu-id="63d99-105">Получение количества действий в Microsoft Teams по каждому типу.</span><span class="sxs-lookup"><span data-stu-id="63d99-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="63d99-106">К типам действий относятся сообщения в чатах групп, сообщения в приватных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="63d99-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="63d99-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63d99-107">Permissions</span></span>

<span data-ttu-id="63d99-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63d99-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63d99-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63d99-110">Permission type</span></span>                        | <span data-ttu-id="63d99-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63d99-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="63d99-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63d99-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="63d99-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="63d99-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="63d99-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63d99-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63d99-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63d99-115">Not supported.</span></span>                           |
| <span data-ttu-id="63d99-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63d99-116">Application</span></span>                            | <span data-ttu-id="63d99-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="63d99-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="63d99-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63d99-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="63d99-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="63d99-119">Function parameters</span></span>

<span data-ttu-id="63d99-120">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="63d99-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="63d99-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="63d99-121">Parameter</span></span> | <span data-ttu-id="63d99-122">Тип</span><span class="sxs-lookup"><span data-stu-id="63d99-122">Type</span></span>   | <span data-ttu-id="63d99-123">Описание</span><span class="sxs-lookup"><span data-stu-id="63d99-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="63d99-124">period</span><span class="sxs-lookup"><span data-stu-id="63d99-124">period</span></span>    | <span data-ttu-id="63d99-125">строка</span><span class="sxs-lookup"><span data-stu-id="63d99-125">string</span></span> | <span data-ttu-id="63d99-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="63d99-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="63d99-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="63d99-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="63d99-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="63d99-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="63d99-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63d99-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="63d99-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63d99-130">Request headers</span></span>

| <span data-ttu-id="63d99-131">Имя</span><span class="sxs-lookup"><span data-stu-id="63d99-131">Name</span></span>          | <span data-ttu-id="63d99-132">Описание</span><span class="sxs-lookup"><span data-stu-id="63d99-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="63d99-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63d99-133">Authorization</span></span> | <span data-ttu-id="63d99-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63d99-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="63d99-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="63d99-136">Response</span></span>

<span data-ttu-id="63d99-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="63d99-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="63d99-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="63d99-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="63d99-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="63d99-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="63d99-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="63d99-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="63d99-141">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="63d99-141">Report Refresh Date</span></span>
- <span data-ttu-id="63d99-142">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="63d99-142">Report Date</span></span>
- <span data-ttu-id="63d99-143">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="63d99-143">Team Chat Messages</span></span>
- <span data-ttu-id="63d99-144">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="63d99-144">Private Chat Messages</span></span>
- <span data-ttu-id="63d99-145">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="63d99-145">Calls</span></span>
- <span data-ttu-id="63d99-146">Meetings (собрания);</span><span class="sxs-lookup"><span data-stu-id="63d99-146">Meetings</span></span>
- <span data-ttu-id="63d99-147">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="63d99-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="63d99-148">Пример</span><span class="sxs-lookup"><span data-stu-id="63d99-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="63d99-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="63d99-149">Request</span></span>

<span data-ttu-id="63d99-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63d99-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="63d99-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="63d99-151">Response</span></span>

<span data-ttu-id="63d99-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="63d99-152">The following is an example of the response.</span></span>

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
<span data-ttu-id="63d99-153">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="63d99-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```
