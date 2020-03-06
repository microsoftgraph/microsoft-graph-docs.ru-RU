---
title: 'reportRoot: getOneDriveActivityFileCounts'
description: Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d87dc791e1509f946760e29af16cec3776cf0a69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510300"
---
# <a name="reportroot-getonedriveactivityfilecounts"></a><span data-ttu-id="3fcdc-103">reportRoot: getOneDriveActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="3fcdc-103">reportRoot: getOneDriveActivityFileCounts</span></span>

<span data-ttu-id="3fcdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fcdc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3fcdc-105">Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-105">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span>

> <span data-ttu-id="3fcdc-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="3fcdc-106">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="3fcdc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fcdc-107">Permissions</span></span>

<span data-ttu-id="3fcdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fcdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3fcdc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fcdc-110">Permission type</span></span>                        | <span data-ttu-id="3fcdc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fcdc-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3fcdc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fcdc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3fcdc-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fcdc-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3fcdc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fcdc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fcdc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-115">Not supported.</span></span>                           |
| <span data-ttu-id="3fcdc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fcdc-116">Application</span></span>                            | <span data-ttu-id="3fcdc-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fcdc-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="3fcdc-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3fcdc-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="3fcdc-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3fcdc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fcdc-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3fcdc-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3fcdc-121">Function parameters</span></span>

<span data-ttu-id="3fcdc-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3fcdc-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="3fcdc-123">Parameter</span></span> | <span data-ttu-id="3fcdc-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3fcdc-124">Type</span></span>   | <span data-ttu-id="3fcdc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3fcdc-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3fcdc-126">period</span><span class="sxs-lookup"><span data-stu-id="3fcdc-126">period</span></span>    | <span data-ttu-id="3fcdc-127">string</span><span class="sxs-lookup"><span data-stu-id="3fcdc-127">string</span></span> | <span data-ttu-id="3fcdc-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3fcdc-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3fcdc-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3fcdc-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3fcdc-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fcdc-132">Request headers</span></span>

| <span data-ttu-id="3fcdc-133">Имя</span><span class="sxs-lookup"><span data-stu-id="3fcdc-133">Name</span></span>          | <span data-ttu-id="3fcdc-134">Описание</span><span class="sxs-lookup"><span data-stu-id="3fcdc-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3fcdc-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3fcdc-135">Authorization</span></span> | <span data-ttu-id="3fcdc-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3fcdc-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3fcdc-138">If-None-Match</span></span> | <span data-ttu-id="3fcdc-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3fcdc-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3fcdc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fcdc-141">Response</span></span>

<span data-ttu-id="3fcdc-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3fcdc-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3fcdc-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3fcdc-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3fcdc-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3fcdc-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3fcdc-146">Report Refresh Date</span></span>
- <span data-ttu-id="3fcdc-147">"Viewed Or Edited" (Просмотрены или изменены);</span><span class="sxs-lookup"><span data-stu-id="3fcdc-147">Viewed Or Edited</span></span>
- <span data-ttu-id="3fcdc-148">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="3fcdc-148">Synced</span></span>
- <span data-ttu-id="3fcdc-149">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="3fcdc-149">Shared Internally</span></span>
- <span data-ttu-id="3fcdc-150">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="3fcdc-150">Shared Externally</span></span>
- <span data-ttu-id="3fcdc-151">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="3fcdc-151">Report Date</span></span>
- <span data-ttu-id="3fcdc-152">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="3fcdc-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3fcdc-153">Пример</span><span class="sxs-lookup"><span data-stu-id="3fcdc-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3fcdc-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fcdc-154">Request</span></span>

<span data-ttu-id="3fcdc-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3fcdc-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fcdc-156">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityfilecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityFileCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="3fcdc-157">C#</span><span class="sxs-lookup"><span data-stu-id="3fcdc-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityfilecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3fcdc-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3fcdc-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityfilecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3fcdc-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3fcdc-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityfilecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3fcdc-160">Java</span><span class="sxs-lookup"><span data-stu-id="3fcdc-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveactivityfilecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3fcdc-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fcdc-161">Response</span></span>

<span data-ttu-id="3fcdc-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="3fcdc-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3fcdc-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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
