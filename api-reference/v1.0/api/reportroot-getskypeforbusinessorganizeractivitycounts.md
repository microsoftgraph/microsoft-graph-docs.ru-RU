---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: Получение сведений о том, как меняется количество и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: fbd35e1eddae4b6d3a492cfcdc2a207e487e0531
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865299"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="d8f04-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="d8f04-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

<span data-ttu-id="d8f04-105">Получение сведений о том, как меняется количество и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации.</span><span class="sxs-lookup"><span data-stu-id="d8f04-105">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="d8f04-106">Такие типы включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба или корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="d8f04-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="d8f04-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия организатора конференций в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="d8f04-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="d8f04-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8f04-108">Permissions</span></span>

<span data-ttu-id="d8f04-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8f04-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d8f04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8f04-111">Permission type</span></span>                        | <span data-ttu-id="d8f04-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8f04-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d8f04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8f04-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8f04-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8f04-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d8f04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8f04-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8f04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8f04-116">Not supported.</span></span>                           |
| <span data-ttu-id="d8f04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8f04-117">Application</span></span>                            | <span data-ttu-id="d8f04-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8f04-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="d8f04-119">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d8f04-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d8f04-120">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="d8f04-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d8f04-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8f04-121">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d8f04-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="d8f04-122">Function parameters</span></span>

<span data-ttu-id="d8f04-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="d8f04-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d8f04-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="d8f04-124">Parameter</span></span> | <span data-ttu-id="d8f04-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d8f04-125">Type</span></span>   | <span data-ttu-id="d8f04-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d8f04-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d8f04-127">period</span><span class="sxs-lookup"><span data-stu-id="d8f04-127">period</span></span>    | <span data-ttu-id="d8f04-128">string</span><span class="sxs-lookup"><span data-stu-id="d8f04-128">string</span></span> | <span data-ttu-id="d8f04-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="d8f04-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d8f04-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="d8f04-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d8f04-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="d8f04-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d8f04-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8f04-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d8f04-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8f04-133">Request headers</span></span>

| <span data-ttu-id="d8f04-134">Имя</span><span class="sxs-lookup"><span data-stu-id="d8f04-134">Name</span></span>          | <span data-ttu-id="d8f04-135">Описание</span><span class="sxs-lookup"><span data-stu-id="d8f04-135">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d8f04-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8f04-136">Authorization</span></span> | <span data-ttu-id="d8f04-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8f04-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d8f04-139">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d8f04-139">If-None-Match</span></span> | <span data-ttu-id="d8f04-140">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="d8f04-140">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d8f04-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d8f04-141">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d8f04-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8f04-142">Response</span></span>

<span data-ttu-id="d8f04-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="d8f04-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d8f04-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="d8f04-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d8f04-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d8f04-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d8f04-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="d8f04-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d8f04-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="d8f04-147">Report Refresh Date</span></span>
- <span data-ttu-id="d8f04-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="d8f04-148">Report Date</span></span>
- <span data-ttu-id="d8f04-149">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="d8f04-149">Report Period</span></span>
- <span data-ttu-id="d8f04-150">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="d8f04-150">IM</span></span>
- <span data-ttu-id="d8f04-151">"Audio/Video" (Аудио и видео);</span><span class="sxs-lookup"><span data-stu-id="d8f04-151">Audio/Video</span></span>
- <span data-ttu-id="d8f04-152">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="d8f04-152">App Sharing</span></span>
- <span data-ttu-id="d8f04-153">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="d8f04-153">Web</span></span>
- <span data-ttu-id="d8f04-154">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба);</span><span class="sxs-lookup"><span data-stu-id="d8f04-154">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="d8f04-155">"Dial-in/out Microsoft" (Конференции с возможностью присоединения по прямому или обратному звонку, корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="d8f04-155">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="d8f04-156">Пример</span><span class="sxs-lookup"><span data-stu-id="d8f04-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d8f04-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8f04-157">Request</span></span>

<span data-ttu-id="d8f04-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8f04-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d8f04-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8f04-159">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d8f04-160">C#</span><span class="sxs-lookup"><span data-stu-id="d8f04-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8f04-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8f04-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d8f04-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8f04-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d8f04-163">Java</span><span class="sxs-lookup"><span data-stu-id="d8f04-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d8f04-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8f04-164">Response</span></span>

<span data-ttu-id="d8f04-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d8f04-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="d8f04-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="d8f04-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
