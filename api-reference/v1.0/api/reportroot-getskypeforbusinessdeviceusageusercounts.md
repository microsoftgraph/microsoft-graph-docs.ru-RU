---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса. Кроме того, вы получите статистические данные с разбивкой по типу устройства (Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.
localization_priority: Normal
ms.openlocfilehash: 9b4f86079a1ce4a12ce3e480c148c588361bd9b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875817"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="8412e-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="8412e-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="8412e-105">Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8412e-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="8412e-106">Кроме того, вы получите статистические данные с разбивкой по типу устройства (Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.</span><span class="sxs-lookup"><span data-stu-id="8412e-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="8412e-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: используемые клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="8412e-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="8412e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8412e-108">Permissions</span></span>

<span data-ttu-id="8412e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8412e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8412e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8412e-111">Permission type</span></span>                        | <span data-ttu-id="8412e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8412e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8412e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8412e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8412e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8412e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8412e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8412e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8412e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8412e-116">Not supported.</span></span>                           |
| <span data-ttu-id="8412e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8412e-117">Application</span></span>                            | <span data-ttu-id="8412e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8412e-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8412e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8412e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8412e-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="8412e-120">Function parameters</span></span>

<span data-ttu-id="8412e-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="8412e-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8412e-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="8412e-122">Parameter</span></span> | <span data-ttu-id="8412e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8412e-123">Type</span></span>   | <span data-ttu-id="8412e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8412e-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8412e-125">period</span><span class="sxs-lookup"><span data-stu-id="8412e-125">period</span></span>    | <span data-ttu-id="8412e-126">строка</span><span class="sxs-lookup"><span data-stu-id="8412e-126">string</span></span> | <span data-ttu-id="8412e-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="8412e-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8412e-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="8412e-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8412e-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="8412e-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8412e-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8412e-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8412e-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8412e-131">Request headers</span></span>

| <span data-ttu-id="8412e-132">Имя</span><span class="sxs-lookup"><span data-stu-id="8412e-132">Name</span></span>          | <span data-ttu-id="8412e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8412e-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8412e-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8412e-134">Authorization</span></span> | <span data-ttu-id="8412e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8412e-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8412e-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8412e-137">If-None-Match</span></span> | <span data-ttu-id="8412e-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="8412e-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8412e-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="8412e-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8412e-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="8412e-140">Response</span></span>

<span data-ttu-id="8412e-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="8412e-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8412e-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="8412e-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8412e-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8412e-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8412e-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="8412e-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8412e-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="8412e-145">Report Refresh Date</span></span>
- <span data-ttu-id="8412e-146">Windows</span><span class="sxs-lookup"><span data-stu-id="8412e-146">Windows</span></span>
- <span data-ttu-id="8412e-147">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="8412e-147">Windows Phone</span></span>
- <span data-ttu-id="8412e-148">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="8412e-148">Android Phone</span></span>
- <span data-ttu-id="8412e-149">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="8412e-149">iPhone</span></span>
- <span data-ttu-id="8412e-150">"iPad";</span><span class="sxs-lookup"><span data-stu-id="8412e-150">iPad</span></span>
- <span data-ttu-id="8412e-151">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="8412e-151">Report Date</span></span>
- <span data-ttu-id="8412e-152">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="8412e-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="8412e-153">Пример</span><span class="sxs-lookup"><span data-stu-id="8412e-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8412e-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="8412e-154">Request</span></span>

<span data-ttu-id="8412e-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8412e-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="8412e-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="8412e-156">Response</span></span>

<span data-ttu-id="8412e-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8412e-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="8412e-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="8412e-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```
