---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Получение сведений об активных пользователях Office 365.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e759936f736a5949ca154943bcfa9cf12672271c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268714"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="5b631-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="5b631-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="5b631-104">Получение сведений об активных пользователях Office 365.</span><span class="sxs-lookup"><span data-stu-id="5b631-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="5b631-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="5b631-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b631-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b631-106">Permissions</span></span>

<span data-ttu-id="5b631-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b631-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b631-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b631-109">Permission type</span></span>                        | <span data-ttu-id="5b631-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b631-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5b631-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b631-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b631-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b631-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5b631-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b631-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b631-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b631-114">Not supported.</span></span>                           |
| <span data-ttu-id="5b631-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b631-115">Application</span></span>                            | <span data-ttu-id="5b631-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b631-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5b631-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b631-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5b631-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="5b631-118">Function parameters</span></span>

<span data-ttu-id="5b631-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="5b631-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="5b631-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="5b631-120">Parameter</span></span> | <span data-ttu-id="5b631-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5b631-121">Type</span></span>   | <span data-ttu-id="5b631-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5b631-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5b631-123">period</span><span class="sxs-lookup"><span data-stu-id="5b631-123">period</span></span>    | <span data-ttu-id="5b631-124">string</span><span class="sxs-lookup"><span data-stu-id="5b631-124">string</span></span> | <span data-ttu-id="5b631-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5b631-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5b631-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="5b631-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5b631-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="5b631-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5b631-128">date</span><span class="sxs-lookup"><span data-stu-id="5b631-128">date</span></span>      | <span data-ttu-id="5b631-129">Date</span><span class="sxs-lookup"><span data-stu-id="5b631-129">Date</span></span>   | <span data-ttu-id="5b631-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="5b631-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5b631-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="5b631-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5b631-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="5b631-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5b631-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="5b631-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b631-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b631-134">Request headers</span></span>

| <span data-ttu-id="5b631-135">Имя</span><span class="sxs-lookup"><span data-stu-id="5b631-135">Name</span></span>          | <span data-ttu-id="5b631-136">Описание</span><span class="sxs-lookup"><span data-stu-id="5b631-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5b631-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b631-137">Authorization</span></span> | <span data-ttu-id="5b631-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b631-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5b631-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5b631-140">If-None-Match</span></span> | <span data-ttu-id="5b631-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="5b631-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5b631-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5b631-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5b631-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b631-143">Response</span></span>

<span data-ttu-id="5b631-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="5b631-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5b631-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="5b631-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5b631-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5b631-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5b631-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="5b631-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5b631-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="5b631-148">Report Refresh Date</span></span>
- <span data-ttu-id="5b631-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="5b631-149">User Principal Name</span></span>
- <span data-ttu-id="5b631-150">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="5b631-150">Display Name</span></span>
- <span data-ttu-id="5b631-151">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="5b631-151">Is Deleted</span></span>
- <span data-ttu-id="5b631-152">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="5b631-152">Deleted Date</span></span>
- <span data-ttu-id="5b631-153">"Has Exchange License" (Есть лицензия на Exchange);</span><span class="sxs-lookup"><span data-stu-id="5b631-153">Has Exchange License</span></span>
- <span data-ttu-id="5b631-154">"Has OneDrive License" (Есть лицензия на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="5b631-154">Has OneDrive License</span></span>
- <span data-ttu-id="5b631-155">"Has SharePoint License" (Есть лицензия на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="5b631-155">Has SharePoint License</span></span>
- <span data-ttu-id="5b631-156">"Has Skype For Business License" (Есть лицензия на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="5b631-156">Has Skype For Business License</span></span>
- <span data-ttu-id="5b631-157">"Has Yammer License" (Есть лицензия на Yammer);</span><span class="sxs-lookup"><span data-stu-id="5b631-157">Has Yammer License</span></span>
- <span data-ttu-id="5b631-158">"Has Teams License" (Есть лицензия на Teams);</span><span class="sxs-lookup"><span data-stu-id="5b631-158">Has Teams License</span></span>
- <span data-ttu-id="5b631-159">"Exchange Last Activity Date" (Дата последнего действия в Exchange);</span><span class="sxs-lookup"><span data-stu-id="5b631-159">Exchange Last Activity Date</span></span>
- <span data-ttu-id="5b631-160">"OneDrive Last Activity Date" (Дата последнего действия в OneDrive);</span><span class="sxs-lookup"><span data-stu-id="5b631-160">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="5b631-161">"SharePoint Last Activity Date" (Дата последнего действия в SharePoint);</span><span class="sxs-lookup"><span data-stu-id="5b631-161">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="5b631-162">"Skype For Business Last Activity Date" (Дата последнего действия в Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="5b631-162">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="5b631-163">"Yammer Last Activity Date" (Дата последнего действия в Yammer);</span><span class="sxs-lookup"><span data-stu-id="5b631-163">Yammer Last Activity Date</span></span>
- <span data-ttu-id="5b631-164">"Teams Last Activity Date" (Дата последнего действия в Teams);</span><span class="sxs-lookup"><span data-stu-id="5b631-164">Teams Last Activity Date</span></span>
- <span data-ttu-id="5b631-165">"Exchange License Assign Date" (Дата назначения лицензии на Exchange);</span><span class="sxs-lookup"><span data-stu-id="5b631-165">Exchange License Assign Date</span></span>
- <span data-ttu-id="5b631-166">"OneDrive License Assign Date" (Дата назначения лицензии на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="5b631-166">OneDrive License Assign Date</span></span>
- <span data-ttu-id="5b631-167">"SharePoint License Assign Date" (Дата назначения лицензии на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="5b631-167">SharePoint License Assign Date</span></span>
- <span data-ttu-id="5b631-168">"Skype For Business License Assign Date" (Дата назначения лицензии на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="5b631-168">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="5b631-169">"Yammer License Assign Date" (Дата назначения лицензии на Yammer);</span><span class="sxs-lookup"><span data-stu-id="5b631-169">Yammer License Assign Date</span></span>
- <span data-ttu-id="5b631-170">"Teams License Assign Date" (Дата назначения лицензии на Teams);</span><span class="sxs-lookup"><span data-stu-id="5b631-170">Teams License Assign Date</span></span>
- <span data-ttu-id="5b631-171">"Assigned Products" (Назначенные продукты).</span><span class="sxs-lookup"><span data-stu-id="5b631-171">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="5b631-172">Пример</span><span class="sxs-lookup"><span data-stu-id="5b631-172">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5b631-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b631-173">Request</span></span>

<span data-ttu-id="5b631-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b631-174">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="5b631-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b631-175">Response</span></span>

<span data-ttu-id="5b631-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b631-176">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5b631-177">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5b631-177">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5b631-178">C#</span><span class="sxs-lookup"><span data-stu-id="5b631-178">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b631-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b631-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5b631-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b631-180">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="5b631-181">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="5b631-181">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
