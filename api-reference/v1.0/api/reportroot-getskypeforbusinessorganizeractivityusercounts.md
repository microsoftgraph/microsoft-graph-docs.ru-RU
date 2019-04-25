---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityUserCounts'
description: Получение сведений о том, как меняется количество уникальных пользователей и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 513755bc878cbb3f9d80753e108448996759cda1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580885"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="91765-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="91765-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

<span data-ttu-id="91765-105">Получение сведений о том, как меняется количество уникальных пользователей и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации.</span><span class="sxs-lookup"><span data-stu-id="91765-105">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="91765-106">Типы сеансов конференц-связи включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба или корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="91765-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="91765-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия организатора конференций в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="91765-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="91765-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91765-108">Permissions</span></span>

<span data-ttu-id="91765-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91765-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91765-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91765-111">Permission type</span></span>                        | <span data-ttu-id="91765-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91765-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="91765-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91765-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="91765-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="91765-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="91765-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91765-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91765-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91765-116">Not supported.</span></span>                           |
| <span data-ttu-id="91765-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91765-117">Application</span></span>                            | <span data-ttu-id="91765-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="91765-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="91765-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91765-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="91765-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="91765-120">Function parameters</span></span>

<span data-ttu-id="91765-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="91765-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="91765-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="91765-122">Parameter</span></span> | <span data-ttu-id="91765-123">Тип</span><span class="sxs-lookup"><span data-stu-id="91765-123">Type</span></span>   | <span data-ttu-id="91765-124">Описание</span><span class="sxs-lookup"><span data-stu-id="91765-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="91765-125">period</span><span class="sxs-lookup"><span data-stu-id="91765-125">period</span></span>    | <span data-ttu-id="91765-126">string</span><span class="sxs-lookup"><span data-stu-id="91765-126">string</span></span> | <span data-ttu-id="91765-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="91765-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="91765-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="91765-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="91765-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="91765-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="91765-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91765-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="91765-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91765-131">Request headers</span></span>

| <span data-ttu-id="91765-132">Имя</span><span class="sxs-lookup"><span data-stu-id="91765-132">Name</span></span>          | <span data-ttu-id="91765-133">Описание</span><span class="sxs-lookup"><span data-stu-id="91765-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="91765-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91765-134">Authorization</span></span> | <span data-ttu-id="91765-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91765-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="91765-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="91765-137">If-None-Match</span></span> | <span data-ttu-id="91765-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="91765-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="91765-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="91765-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="91765-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="91765-140">Response</span></span>

<span data-ttu-id="91765-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="91765-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="91765-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="91765-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="91765-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="91765-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="91765-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="91765-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="91765-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="91765-145">Report Refresh Date</span></span>
- <span data-ttu-id="91765-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="91765-146">Report Date</span></span>
- <span data-ttu-id="91765-147">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="91765-147">Report Period</span></span>
- <span data-ttu-id="91765-148">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="91765-148">IM</span></span>
- <span data-ttu-id="91765-149">"Audio/Video" (Аудио и видео);</span><span class="sxs-lookup"><span data-stu-id="91765-149">Audio/Video</span></span>
- <span data-ttu-id="91765-150">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="91765-150">App Sharing</span></span>
- <span data-ttu-id="91765-151">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="91765-151">Web</span></span>
- <span data-ttu-id="91765-152">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба);</span><span class="sxs-lookup"><span data-stu-id="91765-152">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="91765-153">"Dial-in/out Microsoft" (Конференции с возможностью присоединения по прямому или обратному звонку, корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="91765-153">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="91765-154">Пример</span><span class="sxs-lookup"><span data-stu-id="91765-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="91765-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="91765-155">Request</span></span>

<span data-ttu-id="91765-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91765-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="91765-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="91765-157">Response</span></span>

<span data-ttu-id="91765-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="91765-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="91765-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="91765-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```
