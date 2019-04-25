---
title: 'reportRoot: getOffice365GroupsActivityStorage'
description: Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a0b752387e55c54ded35b6faf5c87868fad0b2f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582320"
---
# <a name="reportroot-getoffice365groupsactivitystorage"></a><span data-ttu-id="3bea4-103">reportRoot: getOffice365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="3bea4-103">reportRoot: getOffice365GroupsActivityStorage</span></span>

<span data-ttu-id="3bea4-104">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="3bea4-104">Get the total storage used across all group mailboxes and group sites.</span></span>

> <span data-ttu-id="3bea4-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="3bea4-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="3bea4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3bea4-106">Permissions</span></span>

<span data-ttu-id="3bea4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bea4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3bea4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bea4-109">Permission type</span></span>                        | <span data-ttu-id="3bea4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bea4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3bea4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bea4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3bea4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bea4-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3bea4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bea4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bea4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bea4-114">Not supported.</span></span>                           |
| <span data-ttu-id="3bea4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bea4-115">Application</span></span>                            | <span data-ttu-id="3bea4-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bea4-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3bea4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bea4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3bea4-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3bea4-118">Function parameters</span></span>

<span data-ttu-id="3bea4-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3bea4-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3bea4-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="3bea4-120">Parameter</span></span> | <span data-ttu-id="3bea4-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3bea4-121">Type</span></span>   | <span data-ttu-id="3bea4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3bea4-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3bea4-123">period</span><span class="sxs-lookup"><span data-stu-id="3bea4-123">period</span></span>    | <span data-ttu-id="3bea4-124">string</span><span class="sxs-lookup"><span data-stu-id="3bea4-124">string</span></span> | <span data-ttu-id="3bea4-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3bea4-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3bea4-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3bea4-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3bea4-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3bea4-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3bea4-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3bea4-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3bea4-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bea4-129">Request headers</span></span>

| <span data-ttu-id="3bea4-130">Имя</span><span class="sxs-lookup"><span data-stu-id="3bea4-130">Name</span></span>          | <span data-ttu-id="3bea4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3bea4-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3bea4-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3bea4-132">Authorization</span></span> | <span data-ttu-id="3bea4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3bea4-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3bea4-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3bea4-135">If-None-Match</span></span> | <span data-ttu-id="3bea4-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="3bea4-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3bea4-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3bea4-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3bea4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bea4-138">Response</span></span>

<span data-ttu-id="3bea4-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3bea4-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3bea4-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3bea4-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3bea4-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3bea4-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3bea4-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3bea4-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3bea4-143">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="3bea4-143">Report Refresh Date</span></span>
- <span data-ttu-id="3bea4-144">Mailbox Storage Used (Byte) [занято почтовыми ящиками (байт)]</span><span class="sxs-lookup"><span data-stu-id="3bea4-144">Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="3bea4-145">Site Storage Used (Byte) [занято сайтами (байт)]</span><span class="sxs-lookup"><span data-stu-id="3bea4-145">Site Storage Used (Byte)</span></span>
- <span data-ttu-id="3bea4-146">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="3bea4-146">Report Date</span></span>
- <span data-ttu-id="3bea4-147">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="3bea4-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3bea4-148">Пример</span><span class="sxs-lookup"><span data-stu-id="3bea4-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3bea4-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bea4-149">Request</span></span>

<span data-ttu-id="3bea4-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bea4-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitystorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityStorage(period='D7')
```

#### <a name="response"></a><span data-ttu-id="3bea4-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bea4-151">Response</span></span>

<span data-ttu-id="3bea4-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3bea4-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="3bea4-153">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3bea4-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mailbox Storage Used (Byte),Site Storage Used (Byte),Report Date,Report Period
```
