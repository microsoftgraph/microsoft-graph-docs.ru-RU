---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса. Кроме того, вы получите статистические данные с разбивкой по типу устройства (устройство с Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 79df65aa3323757bf01ce890303bfa3210d0a7ef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972779"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="75159-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="75159-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="75159-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75159-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75159-106">Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="75159-106">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="75159-107">Кроме того, вы получите статистические данные с разбивкой по типу устройства (устройство с Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.</span><span class="sxs-lookup"><span data-stu-id="75159-107">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="75159-108">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="75159-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="75159-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75159-109">Permissions</span></span>

<span data-ttu-id="75159-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75159-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75159-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75159-112">Permission type</span></span>                        | <span data-ttu-id="75159-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75159-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="75159-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75159-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="75159-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="75159-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="75159-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75159-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75159-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75159-117">Not supported.</span></span>                           |
| <span data-ttu-id="75159-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75159-118">Application</span></span>                            | <span data-ttu-id="75159-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="75159-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="75159-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="75159-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="75159-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="75159-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="75159-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75159-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="75159-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="75159-123">Function parameters</span></span>

<span data-ttu-id="75159-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="75159-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="75159-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="75159-125">Parameter</span></span> | <span data-ttu-id="75159-126">Тип</span><span class="sxs-lookup"><span data-stu-id="75159-126">Type</span></span>   | <span data-ttu-id="75159-127">Описание</span><span class="sxs-lookup"><span data-stu-id="75159-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="75159-128">period</span><span class="sxs-lookup"><span data-stu-id="75159-128">period</span></span>    | <span data-ttu-id="75159-129">string</span><span class="sxs-lookup"><span data-stu-id="75159-129">string</span></span> | <span data-ttu-id="75159-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="75159-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="75159-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="75159-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="75159-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="75159-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="75159-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75159-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="75159-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75159-134">Request headers</span></span>

| <span data-ttu-id="75159-135">Имя</span><span class="sxs-lookup"><span data-stu-id="75159-135">Name</span></span>          | <span data-ttu-id="75159-136">Описание</span><span class="sxs-lookup"><span data-stu-id="75159-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="75159-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75159-137">Authorization</span></span> | <span data-ttu-id="75159-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75159-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="75159-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="75159-140">If-None-Match</span></span> | <span data-ttu-id="75159-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="75159-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="75159-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="75159-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="75159-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="75159-143">Response</span></span>

<span data-ttu-id="75159-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="75159-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="75159-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="75159-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="75159-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="75159-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="75159-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="75159-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="75159-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="75159-148">Report Refresh Date</span></span>
- <span data-ttu-id="75159-149">"Windows";</span><span class="sxs-lookup"><span data-stu-id="75159-149">Windows</span></span>
- <span data-ttu-id="75159-150">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="75159-150">Windows Phone</span></span>
- <span data-ttu-id="75159-151">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="75159-151">Android Phone</span></span>
- <span data-ttu-id="75159-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="75159-152">iPhone</span></span>
- <span data-ttu-id="75159-153">iPad</span><span class="sxs-lookup"><span data-stu-id="75159-153">iPad</span></span>
- <span data-ttu-id="75159-154">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="75159-154">Report Date</span></span>
- <span data-ttu-id="75159-155">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="75159-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="75159-156">Пример</span><span class="sxs-lookup"><span data-stu-id="75159-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="75159-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="75159-157">Request</span></span>

<span data-ttu-id="75159-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75159-158">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="75159-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="75159-159">Response</span></span>

<span data-ttu-id="75159-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75159-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="75159-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="75159-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
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

