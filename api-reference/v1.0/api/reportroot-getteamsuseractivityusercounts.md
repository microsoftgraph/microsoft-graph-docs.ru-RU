---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Получение количества пользователей Microsoft Teams по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 5eec54e07b4f5cfc8bdb4f5c0f24c6988ef38007
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983108"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="858dd-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="858dd-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="858dd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="858dd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="858dd-106">Получение количества пользователей Microsoft Teams по типу действия.</span><span class="sxs-lookup"><span data-stu-id="858dd-106">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="858dd-107">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="858dd-107">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="858dd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="858dd-108">Permissions</span></span>

<span data-ttu-id="858dd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="858dd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="858dd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="858dd-111">Permission type</span></span>                        | <span data-ttu-id="858dd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="858dd-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="858dd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="858dd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="858dd-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="858dd-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="858dd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="858dd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="858dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="858dd-116">Not supported.</span></span>                           |
| <span data-ttu-id="858dd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="858dd-117">Application</span></span>                            | <span data-ttu-id="858dd-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="858dd-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="858dd-119">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="858dd-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="858dd-120">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="858dd-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="858dd-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="858dd-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="858dd-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="858dd-122">Function parameters</span></span>

<span data-ttu-id="858dd-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="858dd-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="858dd-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="858dd-124">Parameter</span></span> | <span data-ttu-id="858dd-125">Тип</span><span class="sxs-lookup"><span data-stu-id="858dd-125">Type</span></span>   | <span data-ttu-id="858dd-126">Описание</span><span class="sxs-lookup"><span data-stu-id="858dd-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="858dd-127">period</span><span class="sxs-lookup"><span data-stu-id="858dd-127">period</span></span>    | <span data-ttu-id="858dd-128">string</span><span class="sxs-lookup"><span data-stu-id="858dd-128">string</span></span> | <span data-ttu-id="858dd-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="858dd-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="858dd-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="858dd-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="858dd-131">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="858dd-131">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="858dd-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="858dd-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="858dd-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="858dd-133">Request headers</span></span>

| <span data-ttu-id="858dd-134">Имя</span><span class="sxs-lookup"><span data-stu-id="858dd-134">Name</span></span>          | <span data-ttu-id="858dd-135">Описание</span><span class="sxs-lookup"><span data-stu-id="858dd-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="858dd-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="858dd-136">Authorization</span></span> | <span data-ttu-id="858dd-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="858dd-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="858dd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="858dd-139">Response</span></span>

<span data-ttu-id="858dd-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="858dd-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="858dd-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="858dd-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="858dd-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="858dd-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="858dd-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="858dd-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="858dd-144">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="858dd-144">Report Refresh Date</span></span>
- <span data-ttu-id="858dd-145">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="858dd-145">Report Date</span></span>
- <span data-ttu-id="858dd-146">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="858dd-146">Team Chat Messages</span></span>
- <span data-ttu-id="858dd-147">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="858dd-147">Private Chat Messages</span></span>
- <span data-ttu-id="858dd-148">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="858dd-148">Calls</span></span>
- <span data-ttu-id="858dd-149">Meetings (Собрания);</span><span class="sxs-lookup"><span data-stu-id="858dd-149">Meetings</span></span>
- <span data-ttu-id="858dd-150">Other Actions (Другие действия);</span><span class="sxs-lookup"><span data-stu-id="858dd-150">Other Actions</span></span>
- <span data-ttu-id="858dd-151">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="858dd-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="858dd-152">Пример</span><span class="sxs-lookup"><span data-stu-id="858dd-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="858dd-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="858dd-153">Request</span></span>

<span data-ttu-id="858dd-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="858dd-154">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="858dd-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="858dd-155">Response</span></span>

<span data-ttu-id="858dd-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="858dd-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="858dd-157">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="858dd-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
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

