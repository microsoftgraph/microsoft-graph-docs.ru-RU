---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Узнайте, сколько пользователей были активны и неактивны в каждой службе.
ms.openlocfilehash: ce594cc38ba62d70ee0a849342a6c2add0b3e602
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026853"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="6d15a-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="6d15a-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="6d15a-104">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="6d15a-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="6d15a-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="6d15a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="6d15a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d15a-106">Permissions</span></span>

<span data-ttu-id="6d15a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d15a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d15a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d15a-109">Permission type</span></span>                        | <span data-ttu-id="6d15a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d15a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6d15a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d15a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d15a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d15a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6d15a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d15a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d15a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d15a-114">Not supported.</span></span>                           |
| <span data-ttu-id="6d15a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d15a-115">Application</span></span>                            | <span data-ttu-id="6d15a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d15a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6d15a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d15a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6d15a-118">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="6d15a-118">Function parameters</span></span>

<span data-ttu-id="6d15a-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="6d15a-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6d15a-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="6d15a-120">Parameter</span></span> | <span data-ttu-id="6d15a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6d15a-121">Type</span></span>   | <span data-ttu-id="6d15a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6d15a-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6d15a-123">period</span><span class="sxs-lookup"><span data-stu-id="6d15a-123">period</span></span>    | <span data-ttu-id="6d15a-124">строка</span><span class="sxs-lookup"><span data-stu-id="6d15a-124">string</span></span> | <span data-ttu-id="6d15a-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="6d15a-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6d15a-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="6d15a-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6d15a-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="6d15a-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6d15a-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d15a-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6d15a-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d15a-129">Request headers</span></span>

| <span data-ttu-id="6d15a-130">Имя</span><span class="sxs-lookup"><span data-stu-id="6d15a-130">Name</span></span>          | <span data-ttu-id="6d15a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6d15a-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6d15a-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d15a-132">Authorization</span></span> | <span data-ttu-id="6d15a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d15a-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6d15a-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6d15a-135">If-None-Match</span></span> | <span data-ttu-id="6d15a-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="6d15a-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6d15a-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6d15a-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6d15a-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d15a-138">Response</span></span>

<span data-ttu-id="6d15a-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6d15a-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6d15a-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6d15a-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6d15a-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6d15a-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6d15a-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6d15a-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6d15a-143">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="6d15a-143">Report Refresh Date</span></span>
- <span data-ttu-id="6d15a-144">Exchange Active (активны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="6d15a-144">Exchange Active</span></span>
- <span data-ttu-id="6d15a-145">Exchange Inactive (неактивны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="6d15a-145">Exchange Inactive</span></span>
- <span data-ttu-id="6d15a-146">OneDrive Active (активны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="6d15a-146">OneDrive Active</span></span>
- <span data-ttu-id="6d15a-147">OneDrive Inactive (неактивны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="6d15a-147">OneDrive Inactive</span></span>
- <span data-ttu-id="6d15a-148">SharePoint Active (активны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="6d15a-148">SharePoint Active</span></span>
- <span data-ttu-id="6d15a-149">SharePoint Inactive (неактивны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="6d15a-149">SharePoint Inactive</span></span>
- <span data-ttu-id="6d15a-150">Skype For Business Active (активны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="6d15a-150">Skype For Business Active</span></span>
- <span data-ttu-id="6d15a-151">Skype For Business Inactive (неактивны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="6d15a-151">Skype For Business Inactive</span></span>
- <span data-ttu-id="6d15a-152">Yammer Active (активны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="6d15a-152">Yammer Active</span></span>
- <span data-ttu-id="6d15a-153">Yammer Inactive (неактивны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="6d15a-153">Yammer Inactive</span></span>
- <span data-ttu-id="6d15a-154">Teams Active (активны в Teams)</span><span class="sxs-lookup"><span data-stu-id="6d15a-154">Teams Active</span></span>
- <span data-ttu-id="6d15a-155">Teams Inactive (неактивны в Teams)</span><span class="sxs-lookup"><span data-stu-id="6d15a-155">Teams Inactive</span></span>
- <span data-ttu-id="6d15a-156">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="6d15a-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="6d15a-157">Пример</span><span class="sxs-lookup"><span data-stu-id="6d15a-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6d15a-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d15a-158">Request</span></span>

<span data-ttu-id="6d15a-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d15a-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="6d15a-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d15a-160">Response</span></span>

<span data-ttu-id="6d15a-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6d15a-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="6d15a-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6d15a-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```
