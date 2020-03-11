---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов (аудио и видео).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d58fb093ec2896c32cd63b0cae18b7a0f643c36d
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590078"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="e12f7-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="e12f7-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

<span data-ttu-id="e12f7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e12f7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e12f7-106">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов</span><span class="sxs-lookup"><span data-stu-id="e12f7-106">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="e12f7-107">(аудио и видео).</span><span class="sxs-lookup"><span data-stu-id="e12f7-107">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="e12f7-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="e12f7-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="e12f7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e12f7-109">Permissions</span></span>

<span data-ttu-id="e12f7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e12f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e12f7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e12f7-112">Permission type</span></span>                        | <span data-ttu-id="e12f7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e12f7-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e12f7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e12f7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e12f7-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e12f7-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e12f7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e12f7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e12f7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e12f7-117">Not supported.</span></span>                           |
| <span data-ttu-id="e12f7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e12f7-118">Application</span></span>                            | <span data-ttu-id="e12f7-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e12f7-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="e12f7-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e12f7-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e12f7-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="e12f7-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e12f7-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e12f7-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e12f7-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="e12f7-123">Function parameters</span></span>

<span data-ttu-id="e12f7-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="e12f7-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e12f7-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="e12f7-125">Parameter</span></span> | <span data-ttu-id="e12f7-126">Тип</span><span class="sxs-lookup"><span data-stu-id="e12f7-126">Type</span></span>   | <span data-ttu-id="e12f7-127">Описание</span><span class="sxs-lookup"><span data-stu-id="e12f7-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e12f7-128">period</span><span class="sxs-lookup"><span data-stu-id="e12f7-128">period</span></span>    | <span data-ttu-id="e12f7-129">string</span><span class="sxs-lookup"><span data-stu-id="e12f7-129">string</span></span> | <span data-ttu-id="e12f7-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="e12f7-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e12f7-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="e12f7-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e12f7-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="e12f7-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e12f7-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e12f7-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e12f7-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e12f7-134">Request headers</span></span>

| <span data-ttu-id="e12f7-135">Имя</span><span class="sxs-lookup"><span data-stu-id="e12f7-135">Name</span></span>          | <span data-ttu-id="e12f7-136">Описание</span><span class="sxs-lookup"><span data-stu-id="e12f7-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e12f7-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e12f7-137">Authorization</span></span> | <span data-ttu-id="e12f7-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e12f7-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e12f7-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e12f7-140">If-None-Match</span></span> | <span data-ttu-id="e12f7-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="e12f7-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e12f7-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e12f7-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e12f7-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e12f7-143">Response</span></span>

<span data-ttu-id="e12f7-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="e12f7-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e12f7-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="e12f7-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e12f7-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e12f7-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e12f7-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="e12f7-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e12f7-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="e12f7-148">Report Refresh Date</span></span>
- <span data-ttu-id="e12f7-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="e12f7-149">Report Date</span></span>
- <span data-ttu-id="e12f7-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="e12f7-150">Report Period</span></span>
- <span data-ttu-id="e12f7-151">Audio (аудио)</span><span class="sxs-lookup"><span data-stu-id="e12f7-151">Audio</span></span>
- <span data-ttu-id="e12f7-152">Video (видео)</span><span class="sxs-lookup"><span data-stu-id="e12f7-152">Video</span></span>

## <a name="example"></a><span data-ttu-id="e12f7-153">Пример</span><span class="sxs-lookup"><span data-stu-id="e12f7-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e12f7-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="e12f7-154">Request</span></span>

<span data-ttu-id="e12f7-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e12f7-155">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="e12f7-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="e12f7-156">Response</span></span>

<span data-ttu-id="e12f7-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e12f7-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="e12f7-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="e12f7-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
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
