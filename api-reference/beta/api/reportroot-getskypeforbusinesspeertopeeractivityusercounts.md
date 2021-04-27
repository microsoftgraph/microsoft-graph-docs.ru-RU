---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts'
description: Отследите динамику использования по количеству уникальных пользователей и типу проведенных в организации одноранговых сеансов. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов в одноранговых сеансах).
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 8163d6dd01028eaaad08a94815bb5cb74b84e5ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052756"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="ae90d-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="ae90d-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

<span data-ttu-id="ae90d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae90d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae90d-106">Отслеживайте динамику использования по количеству уникальных пользователей и типу проведенных в организации одноранговых сеансов</span><span class="sxs-lookup"><span data-stu-id="ae90d-106">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="ae90d-107">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов в одноранговых сеансах).</span><span class="sxs-lookup"><span data-stu-id="ae90d-107">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="ae90d-108">**Примечание:** Подробные сведения о различных представлениях и именах отчетов см. в Microsoft 365 отчетов — Skype для бизнеса одноранговых [действий.](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)</span><span class="sxs-lookup"><span data-stu-id="ae90d-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="ae90d-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae90d-109">Permissions</span></span>

<span data-ttu-id="ae90d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae90d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae90d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae90d-112">Permission type</span></span>                        | <span data-ttu-id="ae90d-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae90d-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ae90d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae90d-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae90d-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae90d-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ae90d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae90d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae90d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae90d-117">Not supported.</span></span>                           |
| <span data-ttu-id="ae90d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae90d-118">Application</span></span>                            | <span data-ttu-id="ae90d-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae90d-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="ae90d-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ae90d-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ae90d-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ae90d-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ae90d-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae90d-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ae90d-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ae90d-123">Function parameters</span></span>

<span data-ttu-id="ae90d-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ae90d-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ae90d-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="ae90d-125">Parameter</span></span> | <span data-ttu-id="ae90d-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ae90d-126">Type</span></span>   | <span data-ttu-id="ae90d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ae90d-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ae90d-128">period</span><span class="sxs-lookup"><span data-stu-id="ae90d-128">period</span></span>    | <span data-ttu-id="ae90d-129">string</span><span class="sxs-lookup"><span data-stu-id="ae90d-129">string</span></span> | <span data-ttu-id="ae90d-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ae90d-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ae90d-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ae90d-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ae90d-132">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ae90d-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ae90d-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae90d-133">Required.</span></span> |

<span data-ttu-id="ae90d-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ae90d-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ae90d-135">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="ae90d-135">The default output type is text/csv.</span></span> <span data-ttu-id="ae90d-136">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="ae90d-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae90d-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae90d-137">Request headers</span></span>

| <span data-ttu-id="ae90d-138">Имя</span><span class="sxs-lookup"><span data-stu-id="ae90d-138">Name</span></span>          | <span data-ttu-id="ae90d-139">Описание</span><span class="sxs-lookup"><span data-stu-id="ae90d-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ae90d-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae90d-140">Authorization</span></span> | <span data-ttu-id="ae90d-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae90d-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ae90d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae90d-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ae90d-144">CSV</span><span class="sxs-lookup"><span data-stu-id="ae90d-144">CSV</span></span>

<span data-ttu-id="ae90d-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ae90d-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ae90d-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ae90d-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ae90d-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ae90d-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ae90d-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ae90d-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ae90d-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ae90d-149">Report Refresh Date</span></span>
- <span data-ttu-id="ae90d-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="ae90d-150">Report Date</span></span>
- <span data-ttu-id="ae90d-151">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="ae90d-151">Report Period</span></span>
- <span data-ttu-id="ae90d-152">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="ae90d-152">IM</span></span>
- <span data-ttu-id="ae90d-153">"Audio" (Аудио);</span><span class="sxs-lookup"><span data-stu-id="ae90d-153">Audio</span></span>
- <span data-ttu-id="ae90d-154">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="ae90d-154">Video</span></span>
- <span data-ttu-id="ae90d-155">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="ae90d-155">App Sharing</span></span>
- <span data-ttu-id="ae90d-156">"File Transfer" (Передача файлов).</span><span class="sxs-lookup"><span data-stu-id="ae90d-156">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="ae90d-157">JSON</span><span class="sxs-lookup"><span data-stu-id="ae90d-157">JSON</span></span>

<span data-ttu-id="ae90d-158">В случае успеха этот метод возвращает код ответа и `200 OK` **[объект SkypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ae90d-158">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae90d-159">Пример</span><span class="sxs-lookup"><span data-stu-id="ae90d-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ae90d-160">CSV</span><span class="sxs-lookup"><span data-stu-id="ae90d-160">CSV</span></span>

<span data-ttu-id="ae90d-161">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="ae90d-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ae90d-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae90d-162">Request</span></span>

<span data-ttu-id="ae90d-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae90d-163">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="ae90d-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae90d-164">Response</span></span>

<span data-ttu-id="ae90d-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae90d-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ae90d-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ae90d-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```

### <a name="json"></a><span data-ttu-id="ae90d-167">JSON</span><span class="sxs-lookup"><span data-stu-id="ae90d-167">JSON</span></span>

<span data-ttu-id="ae90d-168">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="ae90d-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ae90d-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae90d-169">Request</span></span>

<span data-ttu-id="ae90d-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae90d-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="ae90d-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae90d-171">Response</span></span>

<span data-ttu-id="ae90d-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ae90d-172">The following is an example of the response.</span></span>

> <span data-ttu-id="ae90d-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ae90d-173">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 290

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts)", 
  "value": [
    {
      "im": 379, 
      "audio": 42, 
      "video": 2, 
      "appSharing": 34, 
      "fileTransfer": 36, 
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


