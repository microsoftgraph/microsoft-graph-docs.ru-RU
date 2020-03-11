---
title: 'reportRoot: getMailboxUsageDetail'
description: Получите сведения об использовании почтовых ящиков.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c9aa01ba4e0698197b0a8407c4dab98d97b7314a
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590979"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="aecc3-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="aecc3-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="aecc3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aecc3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aecc3-105">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="aecc3-105">Get details about mailbox usage.</span></span>

> <span data-ttu-id="aecc3-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="aecc3-106">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="aecc3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aecc3-107">Permissions</span></span>

<span data-ttu-id="aecc3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aecc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aecc3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aecc3-110">Permission type</span></span>                        | <span data-ttu-id="aecc3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aecc3-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="aecc3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aecc3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="aecc3-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aecc3-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="aecc3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aecc3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aecc3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aecc3-115">Not supported.</span></span>                           |
| <span data-ttu-id="aecc3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aecc3-116">Application</span></span>                            | <span data-ttu-id="aecc3-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aecc3-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="aecc3-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="aecc3-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="aecc3-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="aecc3-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="aecc3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aecc3-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="aecc3-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="aecc3-121">Function parameters</span></span>

<span data-ttu-id="aecc3-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="aecc3-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="aecc3-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="aecc3-123">Parameter</span></span> | <span data-ttu-id="aecc3-124">Тип</span><span class="sxs-lookup"><span data-stu-id="aecc3-124">Type</span></span>   | <span data-ttu-id="aecc3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="aecc3-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="aecc3-126">period</span><span class="sxs-lookup"><span data-stu-id="aecc3-126">period</span></span>    | <span data-ttu-id="aecc3-127">string</span><span class="sxs-lookup"><span data-stu-id="aecc3-127">string</span></span> | <span data-ttu-id="aecc3-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="aecc3-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="aecc3-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="aecc3-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="aecc3-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="aecc3-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="aecc3-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aecc3-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="aecc3-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aecc3-132">Request headers</span></span>

| <span data-ttu-id="aecc3-133">Имя</span><span class="sxs-lookup"><span data-stu-id="aecc3-133">Name</span></span>          | <span data-ttu-id="aecc3-134">Описание</span><span class="sxs-lookup"><span data-stu-id="aecc3-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="aecc3-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aecc3-135">Authorization</span></span> | <span data-ttu-id="aecc3-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aecc3-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="aecc3-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="aecc3-138">If-None-Match</span></span> | <span data-ttu-id="aecc3-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="aecc3-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="aecc3-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="aecc3-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="aecc3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="aecc3-141">Response</span></span>

<span data-ttu-id="aecc3-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="aecc3-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="aecc3-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="aecc3-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="aecc3-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="aecc3-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="aecc3-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="aecc3-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="aecc3-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="aecc3-146">Report Refresh Date</span></span>
- <span data-ttu-id="aecc3-147">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="aecc3-147">User Principal Name</span></span>
- <span data-ttu-id="aecc3-148">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="aecc3-148">Display Name</span></span>
- <span data-ttu-id="aecc3-149">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="aecc3-149">Is Deleted</span></span>
- <span data-ttu-id="aecc3-150">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="aecc3-150">Deleted Date</span></span>
- <span data-ttu-id="aecc3-151">Created Date (дата создания)</span><span class="sxs-lookup"><span data-stu-id="aecc3-151">Created Date</span></span>
- <span data-ttu-id="aecc3-152">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="aecc3-152">Last Activity Date</span></span>
- <span data-ttu-id="aecc3-153">Item Count (количество элементов)</span><span class="sxs-lookup"><span data-stu-id="aecc3-153">Item Count</span></span>
- <span data-ttu-id="aecc3-154">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="aecc3-154">Storage Used (Byte)</span></span>
- <span data-ttu-id="aecc3-155">Issue Warning Quota (Byte) [объем, при котором выводится предупреждение (байт)]</span><span class="sxs-lookup"><span data-stu-id="aecc3-155">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="aecc3-156">Prohibit Send Quota (Byte) [объем, при котором блокируется отправка (байт)]</span><span class="sxs-lookup"><span data-stu-id="aecc3-156">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="aecc3-157">Prohibit Send/Receive Quota (Byte) [объем, при котором блокируются отправка и получение (байт)]</span><span class="sxs-lookup"><span data-stu-id="aecc3-157">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="aecc3-158">Deleted Item Count (количество удаленных элементов)</span><span class="sxs-lookup"><span data-stu-id="aecc3-158">Deleted Item Count</span></span>
- <span data-ttu-id="aecc3-159">Deleted Item Size (Byte) [размер удаленных элементов (байт)]</span><span class="sxs-lookup"><span data-stu-id="aecc3-159">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="aecc3-160">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="aecc3-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="aecc3-161">Пример</span><span class="sxs-lookup"><span data-stu-id="aecc3-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="aecc3-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="aecc3-162">Request</span></span>

<span data-ttu-id="aecc3-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aecc3-163">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="aecc3-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="aecc3-164">Response</span></span>

<span data-ttu-id="aecc3-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aecc3-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="aecc3-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="aecc3-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
