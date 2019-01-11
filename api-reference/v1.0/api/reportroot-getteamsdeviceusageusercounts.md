---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.
localization_priority: Normal
ms.openlocfilehash: 4a865a91436301ad932d50cf104df74fcf4ead85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878850"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="2ce4c-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="2ce4c-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

<span data-ttu-id="2ce4c-104">Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-104">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ce4c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ce4c-105">Permissions</span></span>

<span data-ttu-id="2ce4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ce4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ce4c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ce4c-108">Permission type</span></span>                        | <span data-ttu-id="2ce4c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ce4c-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2ce4c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ce4c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ce4c-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ce4c-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2ce4c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ce4c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ce4c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-113">Not supported.</span></span>                           |
| <span data-ttu-id="2ce4c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ce4c-114">Application</span></span>                            | <span data-ttu-id="2ce4c-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ce4c-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2ce4c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ce4c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2ce4c-117">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="2ce4c-117">Function parameters</span></span>

<span data-ttu-id="2ce4c-118">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2ce4c-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="2ce4c-119">Parameter</span></span> | <span data-ttu-id="2ce4c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2ce4c-120">Type</span></span>   | <span data-ttu-id="2ce4c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2ce4c-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2ce4c-122">period</span><span class="sxs-lookup"><span data-stu-id="2ce4c-122">period</span></span>    | <span data-ttu-id="2ce4c-123">строка</span><span class="sxs-lookup"><span data-stu-id="2ce4c-123">string</span></span> | <span data-ttu-id="2ce4c-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2ce4c-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2ce4c-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2ce4c-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="2ce4c-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ce4c-128">Request headers</span></span>

| <span data-ttu-id="2ce4c-129">Имя</span><span class="sxs-lookup"><span data-stu-id="2ce4c-129">Name</span></span>          | <span data-ttu-id="2ce4c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2ce4c-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2ce4c-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ce4c-131">Authorization</span></span> | <span data-ttu-id="2ce4c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2ce4c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ce4c-134">Response</span></span>

<span data-ttu-id="2ce4c-135">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-135">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2ce4c-136">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-136">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2ce4c-137">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-137">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2ce4c-138">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="2ce4c-138">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="2ce4c-139">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="2ce4c-139">Report Refresh Date</span></span>
- <span data-ttu-id="2ce4c-140">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="2ce4c-140">Web</span></span>
- <span data-ttu-id="2ce4c-141">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="2ce4c-141">Windows Phone</span></span>
- <span data-ttu-id="2ce4c-142">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="2ce4c-142">Android Phone</span></span>
- <span data-ttu-id="2ce4c-143">"iOS";</span><span class="sxs-lookup"><span data-stu-id="2ce4c-143">iOS</span></span>
- <span data-ttu-id="2ce4c-144">"Mac";</span><span class="sxs-lookup"><span data-stu-id="2ce4c-144">Mac</span></span>
- <span data-ttu-id="2ce4c-145">"Windows";</span><span class="sxs-lookup"><span data-stu-id="2ce4c-145">Windows</span></span>
- <span data-ttu-id="2ce4c-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="2ce4c-146">Report Date</span></span>
- <span data-ttu-id="2ce4c-147">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="2ce4c-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="2ce4c-148">Пример</span><span class="sxs-lookup"><span data-stu-id="2ce4c-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2ce4c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ce4c-149">Request</span></span>

<span data-ttu-id="2ce4c-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="2ce4c-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ce4c-151">Response</span></span>

<span data-ttu-id="2ce4c-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="2ce4c-153">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="2ce4c-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
```
