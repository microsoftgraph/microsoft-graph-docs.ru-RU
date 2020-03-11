---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 13f48514263783fc924ac60d25da605e021eef9a
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590113"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="62bba-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="62bba-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

<span data-ttu-id="62bba-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62bba-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62bba-106">Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации</span><span class="sxs-lookup"><span data-stu-id="62bba-106">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="62bba-107">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).</span><span class="sxs-lookup"><span data-stu-id="62bba-107">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="62bba-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия участников конференций Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="62bba-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="62bba-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62bba-109">Permissions</span></span>

<span data-ttu-id="62bba-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62bba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62bba-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62bba-112">Permission type</span></span>                        | <span data-ttu-id="62bba-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62bba-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="62bba-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62bba-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="62bba-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="62bba-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="62bba-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62bba-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62bba-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62bba-117">Not supported.</span></span>                           |
| <span data-ttu-id="62bba-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62bba-118">Application</span></span>                            | <span data-ttu-id="62bba-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="62bba-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="62bba-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="62bba-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="62bba-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="62bba-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="62bba-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62bba-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="62bba-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="62bba-123">Function parameters</span></span>

<span data-ttu-id="62bba-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="62bba-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="62bba-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="62bba-125">Parameter</span></span> | <span data-ttu-id="62bba-126">Тип</span><span class="sxs-lookup"><span data-stu-id="62bba-126">Type</span></span>   | <span data-ttu-id="62bba-127">Описание</span><span class="sxs-lookup"><span data-stu-id="62bba-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="62bba-128">period</span><span class="sxs-lookup"><span data-stu-id="62bba-128">period</span></span>    | <span data-ttu-id="62bba-129">string</span><span class="sxs-lookup"><span data-stu-id="62bba-129">string</span></span> | <span data-ttu-id="62bba-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="62bba-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="62bba-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="62bba-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="62bba-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="62bba-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="62bba-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62bba-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="62bba-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62bba-134">Request headers</span></span>

| <span data-ttu-id="62bba-135">Имя</span><span class="sxs-lookup"><span data-stu-id="62bba-135">Name</span></span>          | <span data-ttu-id="62bba-136">Описание</span><span class="sxs-lookup"><span data-stu-id="62bba-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="62bba-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62bba-137">Authorization</span></span> | <span data-ttu-id="62bba-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62bba-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="62bba-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="62bba-140">If-None-Match</span></span> | <span data-ttu-id="62bba-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="62bba-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="62bba-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="62bba-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="62bba-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="62bba-143">Response</span></span>

<span data-ttu-id="62bba-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="62bba-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="62bba-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="62bba-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="62bba-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="62bba-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="62bba-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="62bba-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="62bba-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="62bba-148">Report Refresh Date</span></span>
- <span data-ttu-id="62bba-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="62bba-149">Report Date</span></span>
- <span data-ttu-id="62bba-150">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="62bba-150">Report Period</span></span>
- <span data-ttu-id="62bba-151">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="62bba-151">IM</span></span>
- <span data-ttu-id="62bba-152">"Audio/Video" (Аудио и видео);</span><span class="sxs-lookup"><span data-stu-id="62bba-152">Audio/Video</span></span>
- <span data-ttu-id="62bba-153">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="62bba-153">App Sharing</span></span>
- <span data-ttu-id="62bba-154">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="62bba-154">Web</span></span>
- <span data-ttu-id="62bba-155">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба).</span><span class="sxs-lookup"><span data-stu-id="62bba-155">Dial-in/out 3rd Party</span></span>

## <a name="example"></a><span data-ttu-id="62bba-156">Пример</span><span class="sxs-lookup"><span data-stu-id="62bba-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="62bba-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="62bba-157">Request</span></span>

<span data-ttu-id="62bba-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62bba-158">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="62bba-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="62bba-159">Response</span></span>

<span data-ttu-id="62bba-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="62bba-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="62bba-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="62bba-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
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
