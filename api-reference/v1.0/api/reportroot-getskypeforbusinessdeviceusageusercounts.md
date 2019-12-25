---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса. Кроме того, вы получите статистические данные с разбивкой по типу устройства (устройство с Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: eab4bccf576b5a6a7b69f32e8f3ca777b7c63575
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865309"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="c4631-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="c4631-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="c4631-105">Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c4631-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="c4631-106">Кроме того, вы получите статистические данные с разбивкой по типу устройства (Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.</span><span class="sxs-lookup"><span data-stu-id="c4631-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="c4631-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: используемые клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="c4631-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4631-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4631-108">Permissions</span></span>

<span data-ttu-id="c4631-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4631-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4631-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4631-111">Permission type</span></span>                        | <span data-ttu-id="c4631-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4631-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c4631-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4631-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4631-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4631-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c4631-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4631-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4631-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4631-116">Not supported.</span></span>                           |
| <span data-ttu-id="c4631-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4631-117">Application</span></span>                            | <span data-ttu-id="c4631-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4631-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="c4631-119">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c4631-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="c4631-120">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="c4631-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="c4631-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4631-121">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c4631-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c4631-122">Function parameters</span></span>

<span data-ttu-id="c4631-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c4631-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c4631-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="c4631-124">Parameter</span></span> | <span data-ttu-id="c4631-125">Тип</span><span class="sxs-lookup"><span data-stu-id="c4631-125">Type</span></span>   | <span data-ttu-id="c4631-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c4631-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c4631-127">period</span><span class="sxs-lookup"><span data-stu-id="c4631-127">period</span></span>    | <span data-ttu-id="c4631-128">string</span><span class="sxs-lookup"><span data-stu-id="c4631-128">string</span></span> | <span data-ttu-id="c4631-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c4631-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c4631-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c4631-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c4631-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c4631-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c4631-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4631-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c4631-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4631-133">Request headers</span></span>

| <span data-ttu-id="c4631-134">Имя</span><span class="sxs-lookup"><span data-stu-id="c4631-134">Name</span></span>          | <span data-ttu-id="c4631-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c4631-135">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c4631-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4631-136">Authorization</span></span> | <span data-ttu-id="c4631-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4631-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c4631-139">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c4631-139">If-None-Match</span></span> | <span data-ttu-id="c4631-140">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="c4631-140">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c4631-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c4631-141">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c4631-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4631-142">Response</span></span>

<span data-ttu-id="c4631-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c4631-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c4631-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c4631-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c4631-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c4631-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c4631-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c4631-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c4631-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c4631-147">Report Refresh Date</span></span>
- <span data-ttu-id="c4631-148">"Windows";</span><span class="sxs-lookup"><span data-stu-id="c4631-148">Windows</span></span>
- <span data-ttu-id="c4631-149">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="c4631-149">Windows Phone</span></span>
- <span data-ttu-id="c4631-150">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="c4631-150">Android Phone</span></span>
- <span data-ttu-id="c4631-151">iPhone</span><span class="sxs-lookup"><span data-stu-id="c4631-151">iPhone</span></span>
- <span data-ttu-id="c4631-152">iPad</span><span class="sxs-lookup"><span data-stu-id="c4631-152">iPad</span></span>
- <span data-ttu-id="c4631-153">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="c4631-153">Report Date</span></span>
- <span data-ttu-id="c4631-154">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="c4631-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c4631-155">Пример</span><span class="sxs-lookup"><span data-stu-id="c4631-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c4631-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4631-156">Request</span></span>

<span data-ttu-id="c4631-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4631-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c4631-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4631-158">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4631-159">C#</span><span class="sxs-lookup"><span data-stu-id="c4631-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4631-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4631-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4631-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4631-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c4631-162">Java</span><span class="sxs-lookup"><span data-stu-id="c4631-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessdeviceusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c4631-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4631-163">Response</span></span>

<span data-ttu-id="c4631-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4631-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="c4631-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c4631-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
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
