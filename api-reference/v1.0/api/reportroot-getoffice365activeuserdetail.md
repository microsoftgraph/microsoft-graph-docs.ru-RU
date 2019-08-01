---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Получение сведений об активных пользователях Office 365.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 03656e301bfe7fd5a91ef8b8caa4a963bb6253eb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021993"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="1303a-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="1303a-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="1303a-104">Получение сведений об активных пользователях Office 365.</span><span class="sxs-lookup"><span data-stu-id="1303a-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="1303a-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="1303a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="1303a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1303a-106">Permissions</span></span>

<span data-ttu-id="1303a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1303a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1303a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1303a-109">Permission type</span></span>                        | <span data-ttu-id="1303a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1303a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1303a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1303a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1303a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1303a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1303a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1303a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1303a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1303a-114">Not supported.</span></span>                           |
| <span data-ttu-id="1303a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1303a-115">Application</span></span>                            | <span data-ttu-id="1303a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1303a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1303a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1303a-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1303a-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="1303a-118">--Http</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="1303a-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="1303a-119">Function parameters</span></span>

<span data-ttu-id="1303a-120">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="1303a-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="1303a-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="1303a-121">Parameter</span></span> | <span data-ttu-id="1303a-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1303a-122">Type</span></span>   | <span data-ttu-id="1303a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1303a-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1303a-124">period</span><span class="sxs-lookup"><span data-stu-id="1303a-124">period</span></span>    | <span data-ttu-id="1303a-125">string</span><span class="sxs-lookup"><span data-stu-id="1303a-125">string</span></span> | <span data-ttu-id="1303a-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="1303a-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1303a-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="1303a-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1303a-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="1303a-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="1303a-129">date</span><span class="sxs-lookup"><span data-stu-id="1303a-129">date</span></span>      | <span data-ttu-id="1303a-130">Date</span><span class="sxs-lookup"><span data-stu-id="1303a-130">Date</span></span>   | <span data-ttu-id="1303a-131">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="1303a-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="1303a-132">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="1303a-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="1303a-133">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="1303a-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="1303a-134">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="1303a-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1303a-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1303a-135">Request headers</span></span>

| <span data-ttu-id="1303a-136">Имя</span><span class="sxs-lookup"><span data-stu-id="1303a-136">Name</span></span>          | <span data-ttu-id="1303a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="1303a-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="1303a-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1303a-138">Authorization</span></span> | <span data-ttu-id="1303a-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1303a-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="1303a-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1303a-141">If-None-Match</span></span> | <span data-ttu-id="1303a-142">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="1303a-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1303a-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1303a-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1303a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="1303a-144">Response</span></span>

<span data-ttu-id="1303a-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="1303a-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1303a-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="1303a-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1303a-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1303a-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1303a-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="1303a-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1303a-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="1303a-149">Report Refresh Date</span></span>
- <span data-ttu-id="1303a-150">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="1303a-150">User Principal Name</span></span>
- <span data-ttu-id="1303a-151">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="1303a-151">Display Name</span></span>
- <span data-ttu-id="1303a-152">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="1303a-152">Is Deleted</span></span>
- <span data-ttu-id="1303a-153">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="1303a-153">Deleted Date</span></span>
- <span data-ttu-id="1303a-154">"Has Exchange License" (Есть лицензия на Exchange);</span><span class="sxs-lookup"><span data-stu-id="1303a-154">Has Exchange License</span></span>
- <span data-ttu-id="1303a-155">"Has OneDrive License" (Есть лицензия на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="1303a-155">Has OneDrive License</span></span>
- <span data-ttu-id="1303a-156">"Has SharePoint License" (Есть лицензия на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="1303a-156">Has SharePoint License</span></span>
- <span data-ttu-id="1303a-157">"Has Skype For Business License" (Есть лицензия на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="1303a-157">Has Skype For Business License</span></span>
- <span data-ttu-id="1303a-158">"Has Yammer License" (Есть лицензия на Yammer);</span><span class="sxs-lookup"><span data-stu-id="1303a-158">Has Yammer License</span></span>
- <span data-ttu-id="1303a-159">"Has Teams License" (Есть лицензия на Teams);</span><span class="sxs-lookup"><span data-stu-id="1303a-159">Has Teams License</span></span>
- <span data-ttu-id="1303a-160">"Exchange Last Activity Date" (Дата последнего действия в Exchange);</span><span class="sxs-lookup"><span data-stu-id="1303a-160">Exchange Last Activity Date</span></span>
- <span data-ttu-id="1303a-161">"OneDrive Last Activity Date" (Дата последнего действия в OneDrive);</span><span class="sxs-lookup"><span data-stu-id="1303a-161">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="1303a-162">"SharePoint Last Activity Date" (Дата последнего действия в SharePoint);</span><span class="sxs-lookup"><span data-stu-id="1303a-162">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="1303a-163">"Skype For Business Last Activity Date" (Дата последнего действия в Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="1303a-163">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="1303a-164">"Yammer Last Activity Date" (Дата последнего действия в Yammer);</span><span class="sxs-lookup"><span data-stu-id="1303a-164">Yammer Last Activity Date</span></span>
- <span data-ttu-id="1303a-165">"Teams Last Activity Date" (Дата последнего действия в Teams);</span><span class="sxs-lookup"><span data-stu-id="1303a-165">Teams Last Activity Date</span></span>
- <span data-ttu-id="1303a-166">"Exchange License Assign Date" (Дата назначения лицензии на Exchange);</span><span class="sxs-lookup"><span data-stu-id="1303a-166">Exchange License Assign Date</span></span>
- <span data-ttu-id="1303a-167">"OneDrive License Assign Date" (Дата назначения лицензии на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="1303a-167">OneDrive License Assign Date</span></span>
- <span data-ttu-id="1303a-168">"SharePoint License Assign Date" (Дата назначения лицензии на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="1303a-168">SharePoint License Assign Date</span></span>
- <span data-ttu-id="1303a-169">"Skype For Business License Assign Date" (Дата назначения лицензии на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="1303a-169">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="1303a-170">"Yammer License Assign Date" (Дата назначения лицензии на Yammer);</span><span class="sxs-lookup"><span data-stu-id="1303a-170">Yammer License Assign Date</span></span>
- <span data-ttu-id="1303a-171">"Teams License Assign Date" (Дата назначения лицензии на Teams);</span><span class="sxs-lookup"><span data-stu-id="1303a-171">Teams License Assign Date</span></span>
- <span data-ttu-id="1303a-172">"Assigned Products" (Назначенные продукты).</span><span class="sxs-lookup"><span data-stu-id="1303a-172">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="1303a-173">Пример</span><span class="sxs-lookup"><span data-stu-id="1303a-173">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1303a-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="1303a-174">Request</span></span>

<span data-ttu-id="1303a-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1303a-175">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1303a-176">C#</span><span class="sxs-lookup"><span data-stu-id="1303a-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1303a-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1303a-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1303a-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1303a-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1303a-179">Java</span><span class="sxs-lookup"><span data-stu-id="1303a-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activeuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1303a-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="1303a-180">Response</span></span>

<span data-ttu-id="1303a-181">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1303a-181">The following is an example of the response.</span></span>

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

<span data-ttu-id="1303a-182">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="1303a-182">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
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
