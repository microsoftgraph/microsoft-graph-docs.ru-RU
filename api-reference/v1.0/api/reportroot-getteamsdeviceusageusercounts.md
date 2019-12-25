---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 806f931c69e08451195317ca84eebc2bb990f613
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865246"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="bb561-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="bb561-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

<span data-ttu-id="bb561-104">Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="bb561-104">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb561-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb561-105">Permissions</span></span>

<span data-ttu-id="bb561-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb561-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb561-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb561-108">Permission type</span></span>                        | <span data-ttu-id="bb561-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb561-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bb561-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb561-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb561-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb561-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bb561-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb561-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb561-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb561-113">Not supported.</span></span>                           |
| <span data-ttu-id="bb561-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb561-114">Application</span></span>                            | <span data-ttu-id="bb561-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb561-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="bb561-116">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bb561-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="bb561-117">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="bb561-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="bb561-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb561-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bb561-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="bb561-119">Function parameters</span></span>

<span data-ttu-id="bb561-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="bb561-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bb561-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="bb561-121">Parameter</span></span> | <span data-ttu-id="bb561-122">Тип</span><span class="sxs-lookup"><span data-stu-id="bb561-122">Type</span></span>   | <span data-ttu-id="bb561-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bb561-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bb561-124">period</span><span class="sxs-lookup"><span data-stu-id="bb561-124">period</span></span>    | <span data-ttu-id="bb561-125">string</span><span class="sxs-lookup"><span data-stu-id="bb561-125">string</span></span> | <span data-ttu-id="bb561-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="bb561-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bb561-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="bb561-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bb561-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="bb561-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bb561-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb561-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="bb561-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb561-130">Request headers</span></span>

| <span data-ttu-id="bb561-131">Имя</span><span class="sxs-lookup"><span data-stu-id="bb561-131">Name</span></span>          | <span data-ttu-id="bb561-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bb561-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bb561-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb561-133">Authorization</span></span> | <span data-ttu-id="bb561-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb561-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bb561-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb561-136">Response</span></span>

<span data-ttu-id="bb561-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="bb561-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bb561-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="bb561-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bb561-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bb561-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bb561-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="bb561-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="bb561-141">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="bb561-141">Report Refresh Date</span></span>
- <span data-ttu-id="bb561-142">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="bb561-142">Web</span></span>
- <span data-ttu-id="bb561-143">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="bb561-143">Windows Phone</span></span>
- <span data-ttu-id="bb561-144">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="bb561-144">Android Phone</span></span>
- <span data-ttu-id="bb561-145">"iOS";</span><span class="sxs-lookup"><span data-stu-id="bb561-145">iOS</span></span>
- <span data-ttu-id="bb561-146">"Mac";</span><span class="sxs-lookup"><span data-stu-id="bb561-146">Mac</span></span>
- <span data-ttu-id="bb561-147">"Windows";</span><span class="sxs-lookup"><span data-stu-id="bb561-147">Windows</span></span>
- <span data-ttu-id="bb561-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="bb561-148">Report Date</span></span>
- <span data-ttu-id="bb561-149">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="bb561-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="bb561-150">Пример</span><span class="sxs-lookup"><span data-stu-id="bb561-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bb561-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb561-151">Request</span></span>

<span data-ttu-id="bb561-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb561-152">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bb561-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb561-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb561-154">C#</span><span class="sxs-lookup"><span data-stu-id="bb561-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb561-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb561-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb561-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb561-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bb561-157">Java</span><span class="sxs-lookup"><span data-stu-id="bb561-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bb561-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb561-158">Response</span></span>

<span data-ttu-id="bb561-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb561-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="bb561-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="bb561-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
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
