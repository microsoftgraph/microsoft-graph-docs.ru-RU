---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу конференций, в которых участвовали сотрудники организации (аудио и видео).
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: ac9924c04fd069a3defe76cc100fe80344f70c57
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981209"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="9f88a-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="9f88a-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

<span data-ttu-id="9f88a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f88a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f88a-106">Отслеживайте динамику использования по продолжительности (в минутах) и типу конференций, в которых участвовали сотрудники организации</span><span class="sxs-lookup"><span data-stu-id="9f88a-106">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="9f88a-107">(аудио и видео).</span><span class="sxs-lookup"><span data-stu-id="9f88a-107">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="9f88a-108">**Примечание.** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="9f88a-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f88a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f88a-109">Permissions</span></span>

<span data-ttu-id="9f88a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f88a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f88a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f88a-112">Permission type</span></span>                        | <span data-ttu-id="9f88a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f88a-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9f88a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f88a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f88a-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f88a-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9f88a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f88a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f88a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f88a-117">Not supported.</span></span>                           |
| <span data-ttu-id="9f88a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f88a-118">Application</span></span>                            | <span data-ttu-id="9f88a-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f88a-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="9f88a-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9f88a-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="9f88a-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="9f88a-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="9f88a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f88a-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9f88a-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="9f88a-123">Function parameters</span></span>

<span data-ttu-id="9f88a-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="9f88a-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9f88a-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="9f88a-125">Parameter</span></span> | <span data-ttu-id="9f88a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9f88a-126">Type</span></span>   | <span data-ttu-id="9f88a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9f88a-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9f88a-128">period</span><span class="sxs-lookup"><span data-stu-id="9f88a-128">period</span></span>    | <span data-ttu-id="9f88a-129">string</span><span class="sxs-lookup"><span data-stu-id="9f88a-129">string</span></span> | <span data-ttu-id="9f88a-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="9f88a-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9f88a-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="9f88a-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9f88a-132">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="9f88a-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9f88a-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f88a-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9f88a-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f88a-134">Request headers</span></span>

| <span data-ttu-id="9f88a-135">Имя</span><span class="sxs-lookup"><span data-stu-id="9f88a-135">Name</span></span>          | <span data-ttu-id="9f88a-136">Описание</span><span class="sxs-lookup"><span data-stu-id="9f88a-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="9f88a-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f88a-137">Authorization</span></span> | <span data-ttu-id="9f88a-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f88a-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="9f88a-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9f88a-140">If-None-Match</span></span> | <span data-ttu-id="9f88a-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="9f88a-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="9f88a-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9f88a-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9f88a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f88a-143">Response</span></span>

<span data-ttu-id="9f88a-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="9f88a-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9f88a-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="9f88a-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9f88a-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9f88a-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9f88a-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="9f88a-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9f88a-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="9f88a-148">Report Refresh Date</span></span>
- <span data-ttu-id="9f88a-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="9f88a-149">Report Date</span></span>
- <span data-ttu-id="9f88a-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="9f88a-150">Report Period</span></span>
- <span data-ttu-id="9f88a-151">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="9f88a-151">Audio/Video</span></span>

## <a name="example"></a><span data-ttu-id="9f88a-152">Пример</span><span class="sxs-lookup"><span data-stu-id="9f88a-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9f88a-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f88a-153">Request</span></span>

<span data-ttu-id="9f88a-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f88a-154">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="9f88a-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f88a-155">Response</span></span>

<span data-ttu-id="9f88a-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f88a-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="9f88a-157">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="9f88a-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
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

