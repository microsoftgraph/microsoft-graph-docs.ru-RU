---
title: 'reportRoot: getOneDriveUsageFileCounts'
description: Получение общего количества файлов на всех сайтах и количества активных файлов. Файл считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 644847c2dbc8a2d9155432dff0ec6e3404df6d65
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510265"
---
# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="9b324-104">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="9b324-104">reportRoot: getOneDriveUsageFileCounts</span></span>

<span data-ttu-id="9b324-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b324-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9b324-106">Получение общего количества файлов на всех сайтах и количества активных файлов.</span><span class="sxs-lookup"><span data-stu-id="9b324-106">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="9b324-107">Файл считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="9b324-107">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="9b324-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="9b324-108">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b324-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b324-109">Permissions</span></span>

<span data-ttu-id="9b324-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b324-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b324-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b324-112">Permission type</span></span>                        | <span data-ttu-id="9b324-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b324-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9b324-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b324-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b324-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b324-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9b324-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b324-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b324-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b324-117">Not supported.</span></span>                           |
| <span data-ttu-id="9b324-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b324-118">Application</span></span>                            | <span data-ttu-id="9b324-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b324-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="9b324-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9b324-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="9b324-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="9b324-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="9b324-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b324-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9b324-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="9b324-123">Function parameters</span></span>

<span data-ttu-id="9b324-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="9b324-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9b324-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="9b324-125">Parameter</span></span> | <span data-ttu-id="9b324-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9b324-126">Type</span></span>   | <span data-ttu-id="9b324-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9b324-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9b324-128">period</span><span class="sxs-lookup"><span data-stu-id="9b324-128">period</span></span>    | <span data-ttu-id="9b324-129">string</span><span class="sxs-lookup"><span data-stu-id="9b324-129">string</span></span> | <span data-ttu-id="9b324-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="9b324-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9b324-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="9b324-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9b324-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="9b324-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9b324-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b324-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9b324-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b324-134">Request headers</span></span>

| <span data-ttu-id="9b324-135">Имя</span><span class="sxs-lookup"><span data-stu-id="9b324-135">Name</span></span>          | <span data-ttu-id="9b324-136">Описание</span><span class="sxs-lookup"><span data-stu-id="9b324-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="9b324-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b324-137">Authorization</span></span> | <span data-ttu-id="9b324-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b324-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="9b324-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9b324-140">If-None-Match</span></span> | <span data-ttu-id="9b324-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="9b324-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="9b324-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9b324-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9b324-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b324-143">Response</span></span>

<span data-ttu-id="9b324-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="9b324-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9b324-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="9b324-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9b324-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9b324-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9b324-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="9b324-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9b324-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="9b324-148">Report Refresh Date</span></span>
- <span data-ttu-id="9b324-149">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="9b324-149">Site Type</span></span>
- <span data-ttu-id="9b324-150">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="9b324-150">Total</span></span>
- <span data-ttu-id="9b324-151">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="9b324-151">Active</span></span>
- <span data-ttu-id="9b324-152">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="9b324-152">Report Date</span></span>
- <span data-ttu-id="9b324-153">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="9b324-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="9b324-154">Пример</span><span class="sxs-lookup"><span data-stu-id="9b324-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9b324-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b324-155">Request</span></span>

<span data-ttu-id="9b324-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b324-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9b324-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b324-157">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusagefilecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageFileCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="9b324-158">C#</span><span class="sxs-lookup"><span data-stu-id="9b324-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagefilecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b324-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b324-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagefilecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b324-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b324-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagefilecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b324-161">Java</span><span class="sxs-lookup"><span data-stu-id="9b324-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusagefilecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9b324-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b324-162">Response</span></span>

<span data-ttu-id="9b324-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9b324-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="9b324-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="9b324-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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
