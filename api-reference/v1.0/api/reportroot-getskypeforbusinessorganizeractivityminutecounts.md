---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций (аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).
localization_priority: Normal
ms.openlocfilehash: ef53641ef8e2a9063fe988bcb1a8daac0bed8d9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840098"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="d9de6-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="d9de6-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

<span data-ttu-id="d9de6-105">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций</span><span class="sxs-lookup"><span data-stu-id="d9de6-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="d9de6-106">(аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="d9de6-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="d9de6-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="d9de6-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="d9de6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9de6-108">Permissions</span></span>

<span data-ttu-id="d9de6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9de6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9de6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9de6-111">Permission type</span></span>                        | <span data-ttu-id="d9de6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9de6-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d9de6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9de6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9de6-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9de6-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d9de6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9de6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9de6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9de6-116">Not supported.</span></span>                           |
| <span data-ttu-id="d9de6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9de6-117">Application</span></span>                            | <span data-ttu-id="d9de6-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9de6-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d9de6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9de6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d9de6-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="d9de6-120">Function parameters</span></span>

<span data-ttu-id="d9de6-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="d9de6-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d9de6-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="d9de6-122">Parameter</span></span> | <span data-ttu-id="d9de6-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d9de6-123">Type</span></span>   | <span data-ttu-id="d9de6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d9de6-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d9de6-125">period</span><span class="sxs-lookup"><span data-stu-id="d9de6-125">period</span></span>    | <span data-ttu-id="d9de6-126">строка</span><span class="sxs-lookup"><span data-stu-id="d9de6-126">string</span></span> | <span data-ttu-id="d9de6-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="d9de6-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d9de6-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="d9de6-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d9de6-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="d9de6-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d9de6-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9de6-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d9de6-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9de6-131">Request headers</span></span>

| <span data-ttu-id="d9de6-132">Имя</span><span class="sxs-lookup"><span data-stu-id="d9de6-132">Name</span></span>          | <span data-ttu-id="d9de6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d9de6-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d9de6-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9de6-134">Authorization</span></span> | <span data-ttu-id="d9de6-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9de6-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d9de6-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d9de6-137">If-None-Match</span></span> | <span data-ttu-id="d9de6-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="d9de6-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d9de6-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d9de6-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d9de6-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9de6-140">Response</span></span>

<span data-ttu-id="d9de6-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="d9de6-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d9de6-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="d9de6-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d9de6-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d9de6-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d9de6-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="d9de6-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d9de6-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="d9de6-145">Report Refresh Date</span></span>
- <span data-ttu-id="d9de6-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="d9de6-146">Report Date</span></span>
- <span data-ttu-id="d9de6-147">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="d9de6-147">Report Period</span></span>
- <span data-ttu-id="d9de6-148">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="d9de6-148">Audio/Video</span></span>
- <span data-ttu-id="d9de6-149">Dial-in Microsoft (с телефонным подключением через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9de6-149">Dial-in Microsoft</span></span>
- <span data-ttu-id="d9de6-150">Dial-out Microsoft (с присоединением обратным звонком через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9de6-150">Dial-out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="d9de6-151">Пример</span><span class="sxs-lookup"><span data-stu-id="d9de6-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d9de6-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9de6-152">Request</span></span>

<span data-ttu-id="d9de6-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9de6-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="d9de6-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9de6-154">Response</span></span>

<span data-ttu-id="d9de6-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d9de6-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="d9de6-156">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="d9de6-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
```
