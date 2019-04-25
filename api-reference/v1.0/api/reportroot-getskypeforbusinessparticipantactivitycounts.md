---
title: 'reportRoot: getSkypeForBusinessParticipantActivityCounts'
description: Отследите динамику использования по количеству и типу сеансов конференц-связи, в которых участвовали сотрудники организации. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 344c8d202ed413bc2c8e80b9a7f671a300112707
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580899"
---
# <a name="reportroot-getskypeforbusinessparticipantactivitycounts"></a><span data-ttu-id="04c43-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="04c43-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span></span>

<span data-ttu-id="04c43-105">Отследите динамику использования по количеству и типу сеансов конференц-связи, в которых участвовали сотрудники организации.</span><span class="sxs-lookup"><span data-stu-id="04c43-105">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="04c43-106">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).</span><span class="sxs-lookup"><span data-stu-id="04c43-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="04c43-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия участников конференций Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="04c43-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="04c43-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04c43-108">Permissions</span></span>

<span data-ttu-id="04c43-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04c43-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04c43-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04c43-111">Permission type</span></span>                        | <span data-ttu-id="04c43-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04c43-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="04c43-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04c43-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="04c43-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="04c43-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="04c43-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04c43-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04c43-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04c43-116">Not supported.</span></span>                           |
| <span data-ttu-id="04c43-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04c43-117">Application</span></span>                            | <span data-ttu-id="04c43-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="04c43-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="04c43-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04c43-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="04c43-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="04c43-120">Function parameters</span></span>

<span data-ttu-id="04c43-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="04c43-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="04c43-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="04c43-122">Parameter</span></span> | <span data-ttu-id="04c43-123">Тип</span><span class="sxs-lookup"><span data-stu-id="04c43-123">Type</span></span>   | <span data-ttu-id="04c43-124">Описание</span><span class="sxs-lookup"><span data-stu-id="04c43-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="04c43-125">period</span><span class="sxs-lookup"><span data-stu-id="04c43-125">period</span></span>    | <span data-ttu-id="04c43-126">string</span><span class="sxs-lookup"><span data-stu-id="04c43-126">string</span></span> | <span data-ttu-id="04c43-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="04c43-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="04c43-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="04c43-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="04c43-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="04c43-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="04c43-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04c43-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="04c43-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04c43-131">Request headers</span></span>

| <span data-ttu-id="04c43-132">Имя</span><span class="sxs-lookup"><span data-stu-id="04c43-132">Name</span></span>          | <span data-ttu-id="04c43-133">Описание</span><span class="sxs-lookup"><span data-stu-id="04c43-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="04c43-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04c43-134">Authorization</span></span> | <span data-ttu-id="04c43-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04c43-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="04c43-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="04c43-137">If-None-Match</span></span> | <span data-ttu-id="04c43-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="04c43-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="04c43-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="04c43-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="04c43-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="04c43-140">Response</span></span>

<span data-ttu-id="04c43-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="04c43-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="04c43-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="04c43-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="04c43-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="04c43-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="04c43-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="04c43-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="04c43-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="04c43-145">Report Refresh Date</span></span>
- <span data-ttu-id="04c43-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="04c43-146">Report Date</span></span>
- <span data-ttu-id="04c43-147">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="04c43-147">Report Period</span></span>
- <span data-ttu-id="04c43-148">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="04c43-148">IM</span></span>
- <span data-ttu-id="04c43-149">"Audio/Video" (Аудио и видео);</span><span class="sxs-lookup"><span data-stu-id="04c43-149">Audio/Video</span></span>
- <span data-ttu-id="04c43-150">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="04c43-150">App Sharing</span></span>
- <span data-ttu-id="04c43-151">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="04c43-151">Web</span></span>
- <span data-ttu-id="04c43-152">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба).</span><span class="sxs-lookup"><span data-stu-id="04c43-152">Dial-in/out 3rd Party</span></span>

## <a name="example"></a><span data-ttu-id="04c43-153">Пример</span><span class="sxs-lookup"><span data-stu-id="04c43-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="04c43-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="04c43-154">Request</span></span>

<span data-ttu-id="04c43-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04c43-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="04c43-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="04c43-156">Response</span></span>

<span data-ttu-id="04c43-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04c43-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="04c43-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="04c43-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```
