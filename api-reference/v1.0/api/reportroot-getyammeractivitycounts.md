---
title: 'reportRoot: getYammerActivityCounts'
description: Отслеживайте динамику активности пользователей в Yammer по количеству опубликованных, прочитанных и понравившихся сообщений.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 822b3daabfee12c2520fd79b27f16650da48625c
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589168"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="a637d-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="a637d-103">reportRoot: getYammerActivityCounts</span></span>

<span data-ttu-id="a637d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a637d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a637d-105">Отслеживайте динамику активности пользователей в Yammer по количеству опубликованных, прочитанных и понравившихся сообщений.</span><span class="sxs-lookup"><span data-stu-id="a637d-105">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="a637d-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="a637d-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="a637d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a637d-107">Permissions</span></span>

<span data-ttu-id="a637d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a637d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a637d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a637d-110">Permission type</span></span>                        | <span data-ttu-id="a637d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a637d-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a637d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a637d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a637d-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a637d-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a637d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a637d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a637d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a637d-115">Not supported.</span></span>                           |
| <span data-ttu-id="a637d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a637d-116">Application</span></span>                            | <span data-ttu-id="a637d-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a637d-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="a637d-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a637d-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a637d-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a637d-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a637d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a637d-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a637d-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="a637d-121">Function parameters</span></span>

<span data-ttu-id="a637d-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="a637d-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a637d-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="a637d-123">Parameter</span></span> | <span data-ttu-id="a637d-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a637d-124">Type</span></span>   | <span data-ttu-id="a637d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a637d-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a637d-126">period</span><span class="sxs-lookup"><span data-stu-id="a637d-126">period</span></span>    | <span data-ttu-id="a637d-127">string</span><span class="sxs-lookup"><span data-stu-id="a637d-127">string</span></span> | <span data-ttu-id="a637d-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="a637d-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a637d-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="a637d-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a637d-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="a637d-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a637d-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a637d-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a637d-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a637d-132">Request headers</span></span>

| <span data-ttu-id="a637d-133">Имя</span><span class="sxs-lookup"><span data-stu-id="a637d-133">Name</span></span>          | <span data-ttu-id="a637d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a637d-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a637d-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a637d-135">Authorization</span></span> | <span data-ttu-id="a637d-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a637d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a637d-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a637d-138">If-None-Match</span></span> | <span data-ttu-id="a637d-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="a637d-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a637d-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a637d-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a637d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a637d-141">Response</span></span>

<span data-ttu-id="a637d-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="a637d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a637d-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="a637d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a637d-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a637d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a637d-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="a637d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a637d-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="a637d-146">Report Refresh Date</span></span>
- <span data-ttu-id="a637d-147">"Liked" (Понравилось);</span><span class="sxs-lookup"><span data-stu-id="a637d-147">Liked</span></span>
- <span data-ttu-id="a637d-148">"Posted" (Опубликовано);</span><span class="sxs-lookup"><span data-stu-id="a637d-148">Posted</span></span>
- <span data-ttu-id="a637d-149">"Read" (Чтение);</span><span class="sxs-lookup"><span data-stu-id="a637d-149">Read</span></span>
- <span data-ttu-id="a637d-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="a637d-150">Report Date</span></span>
- <span data-ttu-id="a637d-151">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="a637d-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a637d-152">Пример</span><span class="sxs-lookup"><span data-stu-id="a637d-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a637d-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="a637d-153">Request</span></span>

<span data-ttu-id="a637d-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a637d-154">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getyammeractivitycounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="a637d-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="a637d-155">Response</span></span>

<span data-ttu-id="a637d-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a637d-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="a637d-157">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="a637d-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
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
