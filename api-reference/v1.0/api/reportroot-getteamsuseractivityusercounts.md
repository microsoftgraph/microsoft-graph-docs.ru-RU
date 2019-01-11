---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Получение количества пользователей Microsoft Teams по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.
localization_priority: Normal
ms.openlocfilehash: 5db9ccb20d79e487b564487f528c7f90289123e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831299"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="7265c-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="7265c-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="7265c-105">Получение количества пользователей Microsoft Teams по типу действия.</span><span class="sxs-lookup"><span data-stu-id="7265c-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="7265c-106">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="7265c-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="7265c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7265c-107">Permissions</span></span>

<span data-ttu-id="7265c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7265c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7265c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7265c-110">Permission type</span></span>                        | <span data-ttu-id="7265c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7265c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7265c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7265c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7265c-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7265c-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7265c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7265c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7265c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7265c-115">Not supported.</span></span>                           |
| <span data-ttu-id="7265c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7265c-116">Application</span></span>                            | <span data-ttu-id="7265c-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7265c-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7265c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7265c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7265c-119">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="7265c-119">Function parameters</span></span>

<span data-ttu-id="7265c-120">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="7265c-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7265c-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="7265c-121">Parameter</span></span> | <span data-ttu-id="7265c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="7265c-122">Type</span></span>   | <span data-ttu-id="7265c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7265c-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7265c-124">period</span><span class="sxs-lookup"><span data-stu-id="7265c-124">period</span></span>    | <span data-ttu-id="7265c-125">строка</span><span class="sxs-lookup"><span data-stu-id="7265c-125">string</span></span> | <span data-ttu-id="7265c-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="7265c-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7265c-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="7265c-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7265c-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="7265c-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7265c-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7265c-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7265c-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7265c-130">Request headers</span></span>

| <span data-ttu-id="7265c-131">Имя</span><span class="sxs-lookup"><span data-stu-id="7265c-131">Name</span></span>          | <span data-ttu-id="7265c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7265c-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7265c-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7265c-133">Authorization</span></span> | <span data-ttu-id="7265c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7265c-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7265c-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7265c-136">Response</span></span>

<span data-ttu-id="7265c-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="7265c-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7265c-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="7265c-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7265c-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7265c-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7265c-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="7265c-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="7265c-141">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="7265c-141">Report Refresh Date</span></span>
- <span data-ttu-id="7265c-142">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="7265c-142">Report Date</span></span>
- <span data-ttu-id="7265c-143">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="7265c-143">Team Chat Messages</span></span>
- <span data-ttu-id="7265c-144">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="7265c-144">Private Chat Messages</span></span>
- <span data-ttu-id="7265c-145">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="7265c-145">Calls</span></span>
- <span data-ttu-id="7265c-146">Meetings (Собрания);</span><span class="sxs-lookup"><span data-stu-id="7265c-146">Meetings</span></span>
- <span data-ttu-id="7265c-147">Other Actions (Другие действия);</span><span class="sxs-lookup"><span data-stu-id="7265c-147">Other Actions</span></span>
- <span data-ttu-id="7265c-148">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="7265c-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7265c-149">Пример</span><span class="sxs-lookup"><span data-stu-id="7265c-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7265c-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="7265c-150">Request</span></span>

<span data-ttu-id="7265c-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7265c-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7265c-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="7265c-152">Response</span></span>

<span data-ttu-id="7265c-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7265c-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="7265c-154">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="7265c-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```
