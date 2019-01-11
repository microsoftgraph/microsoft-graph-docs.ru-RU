---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityUserCounts'
description: Получение сведений о том, как меняется количество уникальных пользователей и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации. Типы сеансов конференц-связи включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба или корпорация Майкрософт).
localization_priority: Normal
ms.openlocfilehash: 2285062ea40a4e0dc9b1468a926dc2ec6fac5564
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886221"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="17717-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="17717-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

> <span data-ttu-id="17717-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="17717-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17717-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17717-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17717-107">Получение сведений о том, как меняется количество уникальных пользователей и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации.</span><span class="sxs-lookup"><span data-stu-id="17717-107">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="17717-108">Типы сеансов конференц-связи включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба или корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="17717-108">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="17717-109">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия организатора конференций в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="17717-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="17717-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17717-110">Permissions</span></span>

<span data-ttu-id="17717-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17717-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="17717-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17717-113">Permission type</span></span>                        | <span data-ttu-id="17717-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17717-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="17717-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17717-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="17717-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="17717-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="17717-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17717-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17717-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17717-118">Not supported.</span></span>                           |
| <span data-ttu-id="17717-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17717-119">Application</span></span>                            | <span data-ttu-id="17717-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="17717-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="17717-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17717-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="17717-122">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="17717-122">Function parameters</span></span>

<span data-ttu-id="17717-123">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="17717-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="17717-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="17717-124">Parameter</span></span> | <span data-ttu-id="17717-125">Тип</span><span class="sxs-lookup"><span data-stu-id="17717-125">Type</span></span>   | <span data-ttu-id="17717-126">Описание</span><span class="sxs-lookup"><span data-stu-id="17717-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="17717-127">period</span><span class="sxs-lookup"><span data-stu-id="17717-127">period</span></span>    | <span data-ttu-id="17717-128">строка</span><span class="sxs-lookup"><span data-stu-id="17717-128">string</span></span> | <span data-ttu-id="17717-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="17717-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="17717-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="17717-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="17717-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="17717-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="17717-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17717-132">Required.</span></span> |

<span data-ttu-id="17717-133">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="17717-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="17717-134">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="17717-134">The default output type is text/csv.</span></span> <span data-ttu-id="17717-135">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="17717-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17717-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17717-136">Request headers</span></span>

| <span data-ttu-id="17717-137">Имя</span><span class="sxs-lookup"><span data-stu-id="17717-137">Name</span></span>          | <span data-ttu-id="17717-138">Описание</span><span class="sxs-lookup"><span data-stu-id="17717-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="17717-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17717-139">Authorization</span></span> | <span data-ttu-id="17717-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17717-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="17717-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="17717-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="17717-143">CSV</span><span class="sxs-lookup"><span data-stu-id="17717-143">CSV</span></span>

<span data-ttu-id="17717-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="17717-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="17717-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="17717-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="17717-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="17717-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="17717-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="17717-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="17717-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="17717-148">Report Refresh Date</span></span>
- <span data-ttu-id="17717-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="17717-149">Report Date</span></span>
- <span data-ttu-id="17717-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="17717-150">Report Period</span></span>
- <span data-ttu-id="17717-151">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="17717-151">IM</span></span>
- <span data-ttu-id="17717-152">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="17717-152">Audio/Video</span></span>
- <span data-ttu-id="17717-153">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="17717-153">App Sharing</span></span>
- <span data-ttu-id="17717-154">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="17717-154">Web</span></span>
- <span data-ttu-id="17717-155">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба);</span><span class="sxs-lookup"><span data-stu-id="17717-155">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="17717-156">"Dial-in/out Microsoft" (Конференции с возможностью присоединения по прямому или обратному звонку, корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="17717-156">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="17717-157">JSON</span><span class="sxs-lookup"><span data-stu-id="17717-157">JSON</span></span>

<span data-ttu-id="17717-158">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="17717-158">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17717-159">Пример</span><span class="sxs-lookup"><span data-stu-id="17717-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="17717-160">CSV</span><span class="sxs-lookup"><span data-stu-id="17717-160">CSV</span></span>

<span data-ttu-id="17717-161">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="17717-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="17717-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="17717-162">Request</span></span>

<span data-ttu-id="17717-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17717-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="17717-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="17717-164">Response</span></span>

<span data-ttu-id="17717-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="17717-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="17717-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="17717-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```

### <a name="json"></a><span data-ttu-id="17717-167">JSON</span><span class="sxs-lookup"><span data-stu-id="17717-167">JSON</span></span>

<span data-ttu-id="17717-168">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="17717-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="17717-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="17717-169">Request</span></span>

<span data-ttu-id="17717-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17717-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="17717-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="17717-171">Response</span></span>

<span data-ttu-id="17717-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="17717-172">The following is an example of the response.</span></span>

> <span data-ttu-id="17717-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17717-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 319

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityUserCounts)", 
  "value": [
    {
      "im": 37, 
      "audioVideo": 42, 
      "appSharing": 35, 
      "web": 3, 
      "dialInOut3rdParty": 0, 
      "dialInOutMicrosoft": 36, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
