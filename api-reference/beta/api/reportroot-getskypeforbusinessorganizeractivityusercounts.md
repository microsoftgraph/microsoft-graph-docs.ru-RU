---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityUserCounts'
description: Получение сведений о том, как меняется количество уникальных пользователей и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9fdf5e4bdf6413898d4d7f4e463830df195281a3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896674"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="8a793-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8a793-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

<span data-ttu-id="8a793-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a793-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a793-106">Отслеживайте динамику использования по количеству уникальных пользователей и типу проведенных и организованных конференций</span><span class="sxs-lookup"><span data-stu-id="8a793-106">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="8a793-107">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу).</span><span class="sxs-lookup"><span data-stu-id="8a793-107">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="8a793-108">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-действия для конференц-связи Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="8a793-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="8a793-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a793-109">Permissions</span></span>

<span data-ttu-id="8a793-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a793-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a793-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a793-112">Permission type</span></span>                        | <span data-ttu-id="8a793-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a793-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8a793-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a793-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a793-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a793-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8a793-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a793-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a793-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a793-117">Not supported.</span></span>                           |
| <span data-ttu-id="8a793-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a793-118">Application</span></span>                            | <span data-ttu-id="8a793-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a793-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="8a793-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a793-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="8a793-121">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="8a793-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="8a793-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a793-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8a793-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="8a793-123">Function parameters</span></span>

<span data-ttu-id="8a793-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="8a793-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8a793-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="8a793-125">Parameter</span></span> | <span data-ttu-id="8a793-126">Тип</span><span class="sxs-lookup"><span data-stu-id="8a793-126">Type</span></span>   | <span data-ttu-id="8a793-127">Описание</span><span class="sxs-lookup"><span data-stu-id="8a793-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8a793-128">period</span><span class="sxs-lookup"><span data-stu-id="8a793-128">period</span></span>    | <span data-ttu-id="8a793-129">string</span><span class="sxs-lookup"><span data-stu-id="8a793-129">string</span></span> | <span data-ttu-id="8a793-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="8a793-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8a793-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="8a793-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8a793-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="8a793-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8a793-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a793-133">Required.</span></span> |

<span data-ttu-id="8a793-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8a793-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8a793-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="8a793-135">The default output type is text/csv.</span></span> <span data-ttu-id="8a793-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="8a793-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a793-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a793-137">Request headers</span></span>

| <span data-ttu-id="8a793-138">Имя</span><span class="sxs-lookup"><span data-stu-id="8a793-138">Name</span></span>          | <span data-ttu-id="8a793-139">Описание</span><span class="sxs-lookup"><span data-stu-id="8a793-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8a793-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a793-140">Authorization</span></span> | <span data-ttu-id="8a793-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a793-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8a793-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a793-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8a793-144">CSV</span><span class="sxs-lookup"><span data-stu-id="8a793-144">CSV</span></span>

<span data-ttu-id="8a793-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="8a793-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8a793-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="8a793-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8a793-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8a793-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8a793-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="8a793-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8a793-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="8a793-149">Report Refresh Date</span></span>
- <span data-ttu-id="8a793-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="8a793-150">Report Date</span></span>
- <span data-ttu-id="8a793-151">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="8a793-151">Report Period</span></span>
- <span data-ttu-id="8a793-152">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="8a793-152">IM</span></span>
- <span data-ttu-id="8a793-153">"Audio/Video" (Аудио и видео);</span><span class="sxs-lookup"><span data-stu-id="8a793-153">Audio/Video</span></span>
- <span data-ttu-id="8a793-154">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="8a793-154">App Sharing</span></span>
- <span data-ttu-id="8a793-155">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="8a793-155">Web</span></span>
- <span data-ttu-id="8a793-156">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба);</span><span class="sxs-lookup"><span data-stu-id="8a793-156">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="8a793-157">"Dial-in/out Microsoft" (Конференции с возможностью присоединения по прямому или обратному звонку, корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="8a793-157">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="8a793-158">JSON</span><span class="sxs-lookup"><span data-stu-id="8a793-158">JSON</span></span>

<span data-ttu-id="8a793-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессорганизерактивитюсеркаунтс](../resources/skypeforbusinessorganizeractivityusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a793-159">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a793-160">Пример</span><span class="sxs-lookup"><span data-stu-id="8a793-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8a793-161">CSV</span><span class="sxs-lookup"><span data-stu-id="8a793-161">CSV</span></span>

<span data-ttu-id="8a793-162">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="8a793-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8a793-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a793-163">Request</span></span>

<span data-ttu-id="8a793-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a793-164">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="8a793-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a793-165">Response</span></span>

<span data-ttu-id="8a793-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a793-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8a793-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="8a793-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="8a793-168">JSON</span><span class="sxs-lookup"><span data-stu-id="8a793-168">JSON</span></span>

<span data-ttu-id="8a793-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="8a793-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8a793-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a793-170">Request</span></span>

<span data-ttu-id="8a793-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a793-171">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="8a793-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a793-172">Response</span></span>

<span data-ttu-id="8a793-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a793-173">The following is an example of the response.</span></span>

> <span data-ttu-id="8a793-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a793-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
