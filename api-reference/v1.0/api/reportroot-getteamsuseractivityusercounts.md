---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Получение количества пользователей Microsoft Teams по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f3c57a19224ca2a04f435526c1ec846b3eed90a2
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44892446"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="44c5e-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="44c5e-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="44c5e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44c5e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44c5e-106">Получение количества пользователей Microsoft Teams по типу действия.</span><span class="sxs-lookup"><span data-stu-id="44c5e-106">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="44c5e-107">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="44c5e-107">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="44c5e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44c5e-108">Permissions</span></span>

<span data-ttu-id="44c5e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44c5e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44c5e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44c5e-111">Permission type</span></span>                        | <span data-ttu-id="44c5e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44c5e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="44c5e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44c5e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="44c5e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44c5e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="44c5e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44c5e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44c5e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44c5e-116">Not supported.</span></span>                           |
| <span data-ttu-id="44c5e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44c5e-117">Application</span></span>                            | <span data-ttu-id="44c5e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44c5e-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="44c5e-119">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="44c5e-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="44c5e-120">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="44c5e-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="44c5e-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44c5e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="44c5e-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="44c5e-122">Function parameters</span></span>

<span data-ttu-id="44c5e-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="44c5e-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="44c5e-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="44c5e-124">Parameter</span></span> | <span data-ttu-id="44c5e-125">Тип</span><span class="sxs-lookup"><span data-stu-id="44c5e-125">Type</span></span>   | <span data-ttu-id="44c5e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="44c5e-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="44c5e-127">period</span><span class="sxs-lookup"><span data-stu-id="44c5e-127">period</span></span>    | <span data-ttu-id="44c5e-128">string</span><span class="sxs-lookup"><span data-stu-id="44c5e-128">string</span></span> | <span data-ttu-id="44c5e-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="44c5e-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="44c5e-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="44c5e-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="44c5e-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="44c5e-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="44c5e-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44c5e-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="44c5e-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44c5e-133">Request headers</span></span>

| <span data-ttu-id="44c5e-134">Имя</span><span class="sxs-lookup"><span data-stu-id="44c5e-134">Name</span></span>          | <span data-ttu-id="44c5e-135">Описание</span><span class="sxs-lookup"><span data-stu-id="44c5e-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="44c5e-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44c5e-136">Authorization</span></span> | <span data-ttu-id="44c5e-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44c5e-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="44c5e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="44c5e-139">Response</span></span>

<span data-ttu-id="44c5e-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="44c5e-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="44c5e-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="44c5e-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="44c5e-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="44c5e-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="44c5e-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="44c5e-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="44c5e-144">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="44c5e-144">Report Refresh Date</span></span>
- <span data-ttu-id="44c5e-145">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="44c5e-145">Report Date</span></span>
- <span data-ttu-id="44c5e-146">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="44c5e-146">Team Chat Messages</span></span>
- <span data-ttu-id="44c5e-147">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="44c5e-147">Private Chat Messages</span></span>
- <span data-ttu-id="44c5e-148">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="44c5e-148">Calls</span></span>
- <span data-ttu-id="44c5e-149">Meetings (Собрания);</span><span class="sxs-lookup"><span data-stu-id="44c5e-149">Meetings</span></span>
- <span data-ttu-id="44c5e-150">Other Actions (Другие действия);</span><span class="sxs-lookup"><span data-stu-id="44c5e-150">Other Actions</span></span>
- <span data-ttu-id="44c5e-151">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="44c5e-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="44c5e-152">Пример</span><span class="sxs-lookup"><span data-stu-id="44c5e-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="44c5e-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="44c5e-153">Request</span></span>

<span data-ttu-id="44c5e-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44c5e-154">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="44c5e-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="44c5e-155">Response</span></span>

<span data-ttu-id="44c5e-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44c5e-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="44c5e-157">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="44c5e-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
