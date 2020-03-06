---
title: 'reportRoot: getMailboxUsageDetail'
description: Получите сведения об использовании почтовых ящиков.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9871804dfec0b143072c9b7746c418d3f7064f1f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510405"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="a6898-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="a6898-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="a6898-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6898-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a6898-105">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="a6898-105">Get details about mailbox usage.</span></span>

> <span data-ttu-id="a6898-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="a6898-106">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6898-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6898-107">Permissions</span></span>

<span data-ttu-id="a6898-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6898-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6898-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6898-110">Permission type</span></span>                        | <span data-ttu-id="a6898-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6898-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a6898-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6898-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6898-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6898-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a6898-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6898-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6898-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6898-115">Not supported.</span></span>                           |
| <span data-ttu-id="a6898-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6898-116">Application</span></span>                            | <span data-ttu-id="a6898-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6898-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="a6898-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a6898-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a6898-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a6898-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a6898-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6898-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a6898-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="a6898-121">Function parameters</span></span>

<span data-ttu-id="a6898-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="a6898-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a6898-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="a6898-123">Parameter</span></span> | <span data-ttu-id="a6898-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a6898-124">Type</span></span>   | <span data-ttu-id="a6898-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a6898-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a6898-126">period</span><span class="sxs-lookup"><span data-stu-id="a6898-126">period</span></span>    | <span data-ttu-id="a6898-127">string</span><span class="sxs-lookup"><span data-stu-id="a6898-127">string</span></span> | <span data-ttu-id="a6898-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="a6898-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a6898-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="a6898-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a6898-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="a6898-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a6898-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6898-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a6898-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6898-132">Request headers</span></span>

| <span data-ttu-id="a6898-133">Имя</span><span class="sxs-lookup"><span data-stu-id="a6898-133">Name</span></span>          | <span data-ttu-id="a6898-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a6898-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a6898-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6898-135">Authorization</span></span> | <span data-ttu-id="a6898-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6898-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a6898-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a6898-138">If-None-Match</span></span> | <span data-ttu-id="a6898-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="a6898-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a6898-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a6898-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a6898-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6898-141">Response</span></span>

<span data-ttu-id="a6898-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="a6898-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a6898-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="a6898-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a6898-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a6898-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a6898-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="a6898-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a6898-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="a6898-146">Report Refresh Date</span></span>
- <span data-ttu-id="a6898-147">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="a6898-147">User Principal Name</span></span>
- <span data-ttu-id="a6898-148">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="a6898-148">Display Name</span></span>
- <span data-ttu-id="a6898-149">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="a6898-149">Is Deleted</span></span>
- <span data-ttu-id="a6898-150">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="a6898-150">Deleted Date</span></span>
- <span data-ttu-id="a6898-151">Created Date (дата создания)</span><span class="sxs-lookup"><span data-stu-id="a6898-151">Created Date</span></span>
- <span data-ttu-id="a6898-152">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="a6898-152">Last Activity Date</span></span>
- <span data-ttu-id="a6898-153">Item Count (количество элементов)</span><span class="sxs-lookup"><span data-stu-id="a6898-153">Item Count</span></span>
- <span data-ttu-id="a6898-154">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="a6898-154">Storage Used (Byte)</span></span>
- <span data-ttu-id="a6898-155">Issue Warning Quota (Byte) [объем, при котором выводится предупреждение (байт)]</span><span class="sxs-lookup"><span data-stu-id="a6898-155">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="a6898-156">Prohibit Send Quota (Byte) [объем, при котором блокируется отправка (байт)]</span><span class="sxs-lookup"><span data-stu-id="a6898-156">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="a6898-157">Prohibit Send/Receive Quota (Byte) [объем, при котором блокируются отправка и получение (байт)]</span><span class="sxs-lookup"><span data-stu-id="a6898-157">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="a6898-158">Deleted Item Count (количество удаленных элементов)</span><span class="sxs-lookup"><span data-stu-id="a6898-158">Deleted Item Count</span></span>
- <span data-ttu-id="a6898-159">Deleted Item Size (Byte) [размер удаленных элементов (байт)]</span><span class="sxs-lookup"><span data-stu-id="a6898-159">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="a6898-160">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="a6898-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a6898-161">Пример</span><span class="sxs-lookup"><span data-stu-id="a6898-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a6898-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6898-162">Request</span></span>

<span data-ttu-id="a6898-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6898-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a6898-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6898-164">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="a6898-165">C#</span><span class="sxs-lookup"><span data-stu-id="a6898-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6898-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6898-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6898-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6898-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6898-168">Java</span><span class="sxs-lookup"><span data-stu-id="a6898-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a6898-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6898-169">Response</span></span>

<span data-ttu-id="a6898-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a6898-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="a6898-171">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="a6898-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Deleted Item Count,Deleted Item Size (Byte),Report Period
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
