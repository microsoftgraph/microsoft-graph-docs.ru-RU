---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса. Кроме того, вы получите статистические данные с разбивкой по типу устройства (устройство с Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 980e83838833e2fc7c16218417eb84df4949cc83
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584798"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="9e9d6-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="9e9d6-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="9e9d6-105">Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="9e9d6-106">Кроме того, вы получите статистические данные с разбивкой по типу устройства (Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="9e9d6-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: используемые клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="9e9d6-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="9e9d6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e9d6-108">Permissions</span></span>

<span data-ttu-id="9e9d6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e9d6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e9d6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e9d6-111">Permission type</span></span>                        | <span data-ttu-id="9e9d6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e9d6-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9e9d6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e9d6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e9d6-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e9d6-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9e9d6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e9d6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e9d6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-116">Not supported.</span></span>                           |
| <span data-ttu-id="9e9d6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e9d6-117">Application</span></span>                            | <span data-ttu-id="9e9d6-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e9d6-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9e9d6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e9d6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9e9d6-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="9e9d6-120">Function parameters</span></span>

<span data-ttu-id="9e9d6-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9e9d6-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="9e9d6-122">Parameter</span></span> | <span data-ttu-id="9e9d6-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9e9d6-123">Type</span></span>   | <span data-ttu-id="9e9d6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9e9d6-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9e9d6-125">period</span><span class="sxs-lookup"><span data-stu-id="9e9d6-125">period</span></span>    | <span data-ttu-id="9e9d6-126">string</span><span class="sxs-lookup"><span data-stu-id="9e9d6-126">string</span></span> | <span data-ttu-id="9e9d6-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9e9d6-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9e9d6-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9e9d6-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9e9d6-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e9d6-131">Request headers</span></span>

| <span data-ttu-id="9e9d6-132">Имя</span><span class="sxs-lookup"><span data-stu-id="9e9d6-132">Name</span></span>          | <span data-ttu-id="9e9d6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9e9d6-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="9e9d6-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e9d6-134">Authorization</span></span> | <span data-ttu-id="9e9d6-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="9e9d6-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9e9d6-137">If-None-Match</span></span> | <span data-ttu-id="9e9d6-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="9e9d6-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9e9d6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e9d6-140">Response</span></span>

<span data-ttu-id="9e9d6-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9e9d6-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9e9d6-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9e9d6-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="9e9d6-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9e9d6-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="9e9d6-145">Report Refresh Date</span></span>
- <span data-ttu-id="9e9d6-146">"Windows";</span><span class="sxs-lookup"><span data-stu-id="9e9d6-146">Windows</span></span>
- <span data-ttu-id="9e9d6-147">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="9e9d6-147">Windows Phone</span></span>
- <span data-ttu-id="9e9d6-148">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="9e9d6-148">Android Phone</span></span>
- <span data-ttu-id="9e9d6-149">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="9e9d6-149">iPhone</span></span>
- <span data-ttu-id="9e9d6-150">"iPad";</span><span class="sxs-lookup"><span data-stu-id="9e9d6-150">iPad</span></span>
- <span data-ttu-id="9e9d6-151">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="9e9d6-151">Report Date</span></span>
- <span data-ttu-id="9e9d6-152">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="9e9d6-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="9e9d6-153">Пример</span><span class="sxs-lookup"><span data-stu-id="9e9d6-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9e9d6-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e9d6-154">Request</span></span>

<span data-ttu-id="9e9d6-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="9e9d6-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e9d6-156">Response</span></span>

<span data-ttu-id="9e9d6-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="9e9d6-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="9e9d6-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```
