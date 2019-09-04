---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityUserCounts'
description: Получение сведений о том, как меняется количество уникальных пользователей и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 056b5436044b99c920d1f5fcd3ed903c23418240
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727980"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="8e424-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8e424-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

<span data-ttu-id="8e424-105">Получение сведений о том, как меняется количество уникальных пользователей и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации.</span><span class="sxs-lookup"><span data-stu-id="8e424-105">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="8e424-106">Типы сеансов конференц-связи включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба или корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="8e424-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="8e424-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия организатора конференций в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="8e424-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e424-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e424-108">Permissions</span></span>

<span data-ttu-id="8e424-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e424-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e424-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e424-111">Permission type</span></span>                        | <span data-ttu-id="8e424-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e424-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8e424-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e424-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e424-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e424-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8e424-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e424-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e424-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e424-116">Not supported.</span></span>                           |
| <span data-ttu-id="8e424-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e424-117">Application</span></span>                            | <span data-ttu-id="8e424-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e424-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8e424-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e424-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8e424-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="8e424-120">Function parameters</span></span>

<span data-ttu-id="8e424-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="8e424-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8e424-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="8e424-122">Parameter</span></span> | <span data-ttu-id="8e424-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8e424-123">Type</span></span>   | <span data-ttu-id="8e424-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8e424-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8e424-125">period</span><span class="sxs-lookup"><span data-stu-id="8e424-125">period</span></span>    | <span data-ttu-id="8e424-126">string</span><span class="sxs-lookup"><span data-stu-id="8e424-126">string</span></span> | <span data-ttu-id="8e424-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="8e424-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8e424-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="8e424-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8e424-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="8e424-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8e424-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e424-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8e424-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e424-131">Request headers</span></span>

| <span data-ttu-id="8e424-132">Имя</span><span class="sxs-lookup"><span data-stu-id="8e424-132">Name</span></span>          | <span data-ttu-id="8e424-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8e424-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8e424-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e424-134">Authorization</span></span> | <span data-ttu-id="8e424-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e424-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8e424-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8e424-137">If-None-Match</span></span> | <span data-ttu-id="8e424-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="8e424-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8e424-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="8e424-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8e424-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e424-140">Response</span></span>

<span data-ttu-id="8e424-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="8e424-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8e424-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="8e424-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8e424-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8e424-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8e424-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="8e424-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8e424-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="8e424-145">Report Refresh Date</span></span>
- <span data-ttu-id="8e424-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="8e424-146">Report Date</span></span>
- <span data-ttu-id="8e424-147">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="8e424-147">Report Period</span></span>
- <span data-ttu-id="8e424-148">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="8e424-148">IM</span></span>
- <span data-ttu-id="8e424-149">"Audio/Video" (Аудио и видео);</span><span class="sxs-lookup"><span data-stu-id="8e424-149">Audio/Video</span></span>
- <span data-ttu-id="8e424-150">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="8e424-150">App Sharing</span></span>
- <span data-ttu-id="8e424-151">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="8e424-151">Web</span></span>
- <span data-ttu-id="8e424-152">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба);</span><span class="sxs-lookup"><span data-stu-id="8e424-152">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="8e424-153">"Dial-in/out Microsoft" (Конференции с возможностью присоединения по прямому или обратному звонку, корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="8e424-153">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="8e424-154">Пример</span><span class="sxs-lookup"><span data-stu-id="8e424-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8e424-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e424-155">Request</span></span>

<span data-ttu-id="8e424-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e424-156">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8e424-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e424-157">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e424-158">C#</span><span class="sxs-lookup"><span data-stu-id="8e424-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e424-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e424-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e424-160">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8e424-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8e424-161">Java</span><span class="sxs-lookup"><span data-stu-id="8e424-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e424-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e424-162">Response</span></span>

<span data-ttu-id="8e424-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e424-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="8e424-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="8e424-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
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
