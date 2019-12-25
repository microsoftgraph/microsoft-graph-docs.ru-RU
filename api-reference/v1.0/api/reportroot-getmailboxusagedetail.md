---
title: 'reportRoot: getMailboxUsageDetail'
description: Получите сведения об использовании почтовых ящиков.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f46c11171e053af741beebb8d999fdbc43aedc4f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864476"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="f548b-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="f548b-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="f548b-104">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="f548b-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="f548b-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="f548b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="f548b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f548b-106">Permissions</span></span>

<span data-ttu-id="f548b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f548b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f548b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f548b-109">Permission type</span></span>                        | <span data-ttu-id="f548b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f548b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f548b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f548b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f548b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f548b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f548b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f548b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f548b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f548b-114">Not supported.</span></span>                           |
| <span data-ttu-id="f548b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f548b-115">Application</span></span>                            | <span data-ttu-id="f548b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f548b-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="f548b-117">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f548b-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="f548b-118">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="f548b-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="f548b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f548b-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f548b-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="f548b-120">Function parameters</span></span>

<span data-ttu-id="f548b-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="f548b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f548b-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="f548b-122">Parameter</span></span> | <span data-ttu-id="f548b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f548b-123">Type</span></span>   | <span data-ttu-id="f548b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f548b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f548b-125">period</span><span class="sxs-lookup"><span data-stu-id="f548b-125">period</span></span>    | <span data-ttu-id="f548b-126">string</span><span class="sxs-lookup"><span data-stu-id="f548b-126">string</span></span> | <span data-ttu-id="f548b-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f548b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f548b-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="f548b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f548b-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="f548b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f548b-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f548b-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f548b-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f548b-131">Request headers</span></span>

| <span data-ttu-id="f548b-132">Имя</span><span class="sxs-lookup"><span data-stu-id="f548b-132">Name</span></span>          | <span data-ttu-id="f548b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f548b-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f548b-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f548b-134">Authorization</span></span> | <span data-ttu-id="f548b-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f548b-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f548b-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f548b-137">If-None-Match</span></span> | <span data-ttu-id="f548b-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="f548b-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f548b-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f548b-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f548b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f548b-140">Response</span></span>

<span data-ttu-id="f548b-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="f548b-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f548b-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="f548b-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f548b-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f548b-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f548b-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="f548b-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f548b-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="f548b-145">Report Refresh Date</span></span>
- <span data-ttu-id="f548b-146">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="f548b-146">User Principal Name</span></span>
- <span data-ttu-id="f548b-147">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="f548b-147">Display Name</span></span>
- <span data-ttu-id="f548b-148">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="f548b-148">Is Deleted</span></span>
- <span data-ttu-id="f548b-149">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="f548b-149">Deleted Date</span></span>
- <span data-ttu-id="f548b-150">Created Date (дата создания)</span><span class="sxs-lookup"><span data-stu-id="f548b-150">Created Date</span></span>
- <span data-ttu-id="f548b-151">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="f548b-151">Last Activity Date</span></span>
- <span data-ttu-id="f548b-152">Item Count (количество элементов)</span><span class="sxs-lookup"><span data-stu-id="f548b-152">Item Count</span></span>
- <span data-ttu-id="f548b-153">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="f548b-153">Storage Used (Byte)</span></span>
- <span data-ttu-id="f548b-154">Issue Warning Quota (Byte) [объем, при котором выводится предупреждение (байт)]</span><span class="sxs-lookup"><span data-stu-id="f548b-154">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="f548b-155">Prohibit Send Quota (Byte) [объем, при котором блокируется отправка (байт)]</span><span class="sxs-lookup"><span data-stu-id="f548b-155">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="f548b-156">Prohibit Send/Receive Quota (Byte) [объем, при котором блокируются отправка и получение (байт)]</span><span class="sxs-lookup"><span data-stu-id="f548b-156">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="f548b-157">Deleted Item Count (количество удаленных элементов)</span><span class="sxs-lookup"><span data-stu-id="f548b-157">Deleted Item Count</span></span>
- <span data-ttu-id="f548b-158">Deleted Item Size (Byte) [размер удаленных элементов (байт)]</span><span class="sxs-lookup"><span data-stu-id="f548b-158">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="f548b-159">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="f548b-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f548b-160">Пример</span><span class="sxs-lookup"><span data-stu-id="f548b-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f548b-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="f548b-161">Request</span></span>

<span data-ttu-id="f548b-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f548b-162">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f548b-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="f548b-163">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f548b-164">C#</span><span class="sxs-lookup"><span data-stu-id="f548b-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f548b-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f548b-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f548b-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f548b-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f548b-167">Java</span><span class="sxs-lookup"><span data-stu-id="f548b-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f548b-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="f548b-168">Response</span></span>

<span data-ttu-id="f548b-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f548b-169">The following is an example of the response.</span></span>

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

<span data-ttu-id="f548b-170">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="f548b-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
