---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Получение количества активных пользователей за каждый день отчетного периода по продукту.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 287e6656b3f505e96bf91bfa614ab2fa37c744d1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582211"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="12fc9-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="12fc9-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="12fc9-104">Получение количества активных пользователей за каждый день отчетного периода по продукту.</span><span class="sxs-lookup"><span data-stu-id="12fc9-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="12fc9-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="12fc9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="12fc9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12fc9-106">Permissions</span></span>

<span data-ttu-id="12fc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12fc9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12fc9-109">Permission type</span></span>                        | <span data-ttu-id="12fc9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12fc9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="12fc9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12fc9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="12fc9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="12fc9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="12fc9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12fc9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12fc9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12fc9-114">Not supported.</span></span>                           |
| <span data-ttu-id="12fc9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12fc9-115">Application</span></span>                            | <span data-ttu-id="12fc9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="12fc9-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="12fc9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12fc9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="12fc9-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="12fc9-118">Function parameters</span></span>

<span data-ttu-id="12fc9-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="12fc9-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="12fc9-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="12fc9-120">Parameter</span></span> | <span data-ttu-id="12fc9-121">Тип</span><span class="sxs-lookup"><span data-stu-id="12fc9-121">Type</span></span>   | <span data-ttu-id="12fc9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="12fc9-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="12fc9-123">period</span><span class="sxs-lookup"><span data-stu-id="12fc9-123">period</span></span>    | <span data-ttu-id="12fc9-124">string</span><span class="sxs-lookup"><span data-stu-id="12fc9-124">string</span></span> | <span data-ttu-id="12fc9-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="12fc9-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="12fc9-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="12fc9-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="12fc9-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="12fc9-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="12fc9-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12fc9-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="12fc9-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12fc9-129">Request headers</span></span>

| <span data-ttu-id="12fc9-130">Имя</span><span class="sxs-lookup"><span data-stu-id="12fc9-130">Name</span></span>          | <span data-ttu-id="12fc9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="12fc9-131">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="12fc9-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12fc9-132">Authorization</span></span> | <span data-ttu-id="12fc9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12fc9-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="12fc9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="12fc9-135">Response</span></span>

<span data-ttu-id="12fc9-136">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="12fc9-136">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="12fc9-137">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="12fc9-137">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="12fc9-138">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="12fc9-138">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="12fc9-139">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="12fc9-139">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="12fc9-140">Report Refresh Date (Дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="12fc9-140">Report Refresh Date</span></span>
- <span data-ttu-id="12fc9-141">Office 365</span><span class="sxs-lookup"><span data-stu-id="12fc9-141">Office 365</span></span>
- <span data-ttu-id="12fc9-142">Exchange</span><span class="sxs-lookup"><span data-stu-id="12fc9-142">Exchange</span></span>
- <span data-ttu-id="12fc9-143">OneDrive;</span><span class="sxs-lookup"><span data-stu-id="12fc9-143">OneDrive</span></span>
- <span data-ttu-id="12fc9-144">SharePoint;</span><span class="sxs-lookup"><span data-stu-id="12fc9-144">SharePoint</span></span>
- <span data-ttu-id="12fc9-145">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="12fc9-145">Skype For Business</span></span> 
- <span data-ttu-id="12fc9-146">Yammer</span><span class="sxs-lookup"><span data-stu-id="12fc9-146">Yammer</span></span>
- <span data-ttu-id="12fc9-147">Teams</span><span class="sxs-lookup"><span data-stu-id="12fc9-147">Teams</span></span>
- <span data-ttu-id="12fc9-148">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="12fc9-148">Report Date</span></span>
- <span data-ttu-id="12fc9-149">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="12fc9-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="12fc9-150">Пример</span><span class="sxs-lookup"><span data-stu-id="12fc9-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="12fc9-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="12fc9-151">Request</span></span>

<span data-ttu-id="12fc9-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12fc9-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="12fc9-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="12fc9-153">Response</span></span>

<span data-ttu-id="12fc9-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="12fc9-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="12fc9-155">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="12fc9-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```
