---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 55fc8154ae1a6135d105b0dedc00482df3cbbe35
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021713"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="45c3b-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="45c3b-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

<span data-ttu-id="45c3b-105">Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации</span><span class="sxs-lookup"><span data-stu-id="45c3b-105">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="45c3b-106">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).</span><span class="sxs-lookup"><span data-stu-id="45c3b-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="45c3b-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия участников конференций Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="45c3b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="45c3b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45c3b-108">Permissions</span></span>

<span data-ttu-id="45c3b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45c3b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="45c3b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45c3b-111">Permission type</span></span>                        | <span data-ttu-id="45c3b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45c3b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="45c3b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45c3b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="45c3b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="45c3b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="45c3b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45c3b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45c3b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45c3b-116">Not supported.</span></span>                           |
| <span data-ttu-id="45c3b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45c3b-117">Application</span></span>                            | <span data-ttu-id="45c3b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="45c3b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="45c3b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45c3b-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="45c3b-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="45c3b-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="45c3b-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="45c3b-121">Function parameters</span></span>

<span data-ttu-id="45c3b-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="45c3b-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="45c3b-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="45c3b-123">Parameter</span></span> | <span data-ttu-id="45c3b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="45c3b-124">Type</span></span>   | <span data-ttu-id="45c3b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="45c3b-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="45c3b-126">period</span><span class="sxs-lookup"><span data-stu-id="45c3b-126">period</span></span>    | <span data-ttu-id="45c3b-127">string</span><span class="sxs-lookup"><span data-stu-id="45c3b-127">string</span></span> | <span data-ttu-id="45c3b-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="45c3b-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="45c3b-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="45c3b-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="45c3b-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="45c3b-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="45c3b-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45c3b-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="45c3b-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45c3b-132">Request headers</span></span>

| <span data-ttu-id="45c3b-133">Имя</span><span class="sxs-lookup"><span data-stu-id="45c3b-133">Name</span></span>          | <span data-ttu-id="45c3b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="45c3b-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="45c3b-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45c3b-135">Authorization</span></span> | <span data-ttu-id="45c3b-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45c3b-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="45c3b-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="45c3b-138">If-None-Match</span></span> | <span data-ttu-id="45c3b-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="45c3b-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="45c3b-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="45c3b-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="45c3b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="45c3b-141">Response</span></span>

<span data-ttu-id="45c3b-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="45c3b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="45c3b-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="45c3b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="45c3b-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="45c3b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="45c3b-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="45c3b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="45c3b-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="45c3b-146">Report Refresh Date</span></span>
- <span data-ttu-id="45c3b-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="45c3b-147">Report Date</span></span>
- <span data-ttu-id="45c3b-148">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="45c3b-148">Report Period</span></span>
- <span data-ttu-id="45c3b-149">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="45c3b-149">IM</span></span>
- <span data-ttu-id="45c3b-150">"Audio/Video" (Аудио и видео);</span><span class="sxs-lookup"><span data-stu-id="45c3b-150">Audio/Video</span></span>
- <span data-ttu-id="45c3b-151">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="45c3b-151">App Sharing</span></span>
- <span data-ttu-id="45c3b-152">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="45c3b-152">Web</span></span>
- <span data-ttu-id="45c3b-153">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба).</span><span class="sxs-lookup"><span data-stu-id="45c3b-153">Dial-in/out 3rd Party</span></span>

## <a name="example"></a><span data-ttu-id="45c3b-154">Пример</span><span class="sxs-lookup"><span data-stu-id="45c3b-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="45c3b-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="45c3b-155">Request</span></span>

<span data-ttu-id="45c3b-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45c3b-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="45c3b-157">C#</span><span class="sxs-lookup"><span data-stu-id="45c3b-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45c3b-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="45c3b-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="45c3b-159">Цель — C</span><span class="sxs-lookup"><span data-stu-id="45c3b-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="45c3b-160">Java</span><span class="sxs-lookup"><span data-stu-id="45c3b-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessparticipantactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="45c3b-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="45c3b-161">Response</span></span>

<span data-ttu-id="45c3b-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="45c3b-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="45c3b-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="45c3b-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
