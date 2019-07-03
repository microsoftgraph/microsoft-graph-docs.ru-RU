---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Получение сведений об активных пользователях Office 365.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d25a818137352f01407b2cfffa4cab846de4662d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459225"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="d5daa-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="d5daa-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="d5daa-104">Получение сведений об активных пользователях Office 365.</span><span class="sxs-lookup"><span data-stu-id="d5daa-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="d5daa-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="d5daa-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5daa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5daa-106">Permissions</span></span>

<span data-ttu-id="d5daa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5daa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5daa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5daa-109">Permission type</span></span>                        | <span data-ttu-id="d5daa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5daa-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d5daa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5daa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5daa-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5daa-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d5daa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5daa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5daa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5daa-114">Not supported.</span></span>                           |
| <span data-ttu-id="d5daa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5daa-115">Application</span></span>                            | <span data-ttu-id="d5daa-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5daa-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d5daa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5daa-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5daa-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5daa-118">--Http</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="d5daa-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="d5daa-119">Function parameters</span></span>

<span data-ttu-id="d5daa-120">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="d5daa-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d5daa-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="d5daa-121">Parameter</span></span> | <span data-ttu-id="d5daa-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d5daa-122">Type</span></span>   | <span data-ttu-id="d5daa-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d5daa-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d5daa-124">period</span><span class="sxs-lookup"><span data-stu-id="d5daa-124">period</span></span>    | <span data-ttu-id="d5daa-125">string</span><span class="sxs-lookup"><span data-stu-id="d5daa-125">string</span></span> | <span data-ttu-id="d5daa-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="d5daa-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d5daa-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="d5daa-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d5daa-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="d5daa-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d5daa-129">date</span><span class="sxs-lookup"><span data-stu-id="d5daa-129">date</span></span>      | <span data-ttu-id="d5daa-130">Date</span><span class="sxs-lookup"><span data-stu-id="d5daa-130">Date</span></span>   | <span data-ttu-id="d5daa-131">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="d5daa-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d5daa-132">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="d5daa-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d5daa-133">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="d5daa-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d5daa-134">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="d5daa-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5daa-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5daa-135">Request headers</span></span>

| <span data-ttu-id="d5daa-136">Имя</span><span class="sxs-lookup"><span data-stu-id="d5daa-136">Name</span></span>          | <span data-ttu-id="d5daa-137">Описание</span><span class="sxs-lookup"><span data-stu-id="d5daa-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d5daa-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5daa-138">Authorization</span></span> | <span data-ttu-id="d5daa-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5daa-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d5daa-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d5daa-141">If-None-Match</span></span> | <span data-ttu-id="d5daa-142">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="d5daa-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d5daa-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d5daa-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d5daa-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5daa-144">Response</span></span>

<span data-ttu-id="d5daa-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="d5daa-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d5daa-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="d5daa-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d5daa-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d5daa-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d5daa-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="d5daa-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d5daa-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="d5daa-149">Report Refresh Date</span></span>
- <span data-ttu-id="d5daa-150">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="d5daa-150">User Principal Name</span></span>
- <span data-ttu-id="d5daa-151">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="d5daa-151">Display Name</span></span>
- <span data-ttu-id="d5daa-152">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="d5daa-152">Is Deleted</span></span>
- <span data-ttu-id="d5daa-153">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="d5daa-153">Deleted Date</span></span>
- <span data-ttu-id="d5daa-154">"Has Exchange License" (Есть лицензия на Exchange);</span><span class="sxs-lookup"><span data-stu-id="d5daa-154">Has Exchange License</span></span>
- <span data-ttu-id="d5daa-155">"Has OneDrive License" (Есть лицензия на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="d5daa-155">Has OneDrive License</span></span>
- <span data-ttu-id="d5daa-156">"Has SharePoint License" (Есть лицензия на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="d5daa-156">Has SharePoint License</span></span>
- <span data-ttu-id="d5daa-157">"Has Skype For Business License" (Есть лицензия на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="d5daa-157">Has Skype For Business License</span></span>
- <span data-ttu-id="d5daa-158">"Has Yammer License" (Есть лицензия на Yammer);</span><span class="sxs-lookup"><span data-stu-id="d5daa-158">Has Yammer License</span></span>
- <span data-ttu-id="d5daa-159">"Has Teams License" (Есть лицензия на Teams);</span><span class="sxs-lookup"><span data-stu-id="d5daa-159">Has Teams License</span></span>
- <span data-ttu-id="d5daa-160">"Exchange Last Activity Date" (Дата последнего действия в Exchange);</span><span class="sxs-lookup"><span data-stu-id="d5daa-160">Exchange Last Activity Date</span></span>
- <span data-ttu-id="d5daa-161">"OneDrive Last Activity Date" (Дата последнего действия в OneDrive);</span><span class="sxs-lookup"><span data-stu-id="d5daa-161">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="d5daa-162">"SharePoint Last Activity Date" (Дата последнего действия в SharePoint);</span><span class="sxs-lookup"><span data-stu-id="d5daa-162">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="d5daa-163">"Skype For Business Last Activity Date" (Дата последнего действия в Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="d5daa-163">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="d5daa-164">"Yammer Last Activity Date" (Дата последнего действия в Yammer);</span><span class="sxs-lookup"><span data-stu-id="d5daa-164">Yammer Last Activity Date</span></span>
- <span data-ttu-id="d5daa-165">"Teams Last Activity Date" (Дата последнего действия в Teams);</span><span class="sxs-lookup"><span data-stu-id="d5daa-165">Teams Last Activity Date</span></span>
- <span data-ttu-id="d5daa-166">"Exchange License Assign Date" (Дата назначения лицензии на Exchange);</span><span class="sxs-lookup"><span data-stu-id="d5daa-166">Exchange License Assign Date</span></span>
- <span data-ttu-id="d5daa-167">"OneDrive License Assign Date" (Дата назначения лицензии на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="d5daa-167">OneDrive License Assign Date</span></span>
- <span data-ttu-id="d5daa-168">"SharePoint License Assign Date" (Дата назначения лицензии на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="d5daa-168">SharePoint License Assign Date</span></span>
- <span data-ttu-id="d5daa-169">"Skype For Business License Assign Date" (Дата назначения лицензии на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="d5daa-169">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="d5daa-170">"Yammer License Assign Date" (Дата назначения лицензии на Yammer);</span><span class="sxs-lookup"><span data-stu-id="d5daa-170">Yammer License Assign Date</span></span>
- <span data-ttu-id="d5daa-171">"Teams License Assign Date" (Дата назначения лицензии на Teams);</span><span class="sxs-lookup"><span data-stu-id="d5daa-171">Teams License Assign Date</span></span>
- <span data-ttu-id="d5daa-172">"Assigned Products" (Назначенные продукты).</span><span class="sxs-lookup"><span data-stu-id="d5daa-172">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="d5daa-173">Пример</span><span class="sxs-lookup"><span data-stu-id="d5daa-173">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d5daa-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5daa-174">Request</span></span>

<span data-ttu-id="d5daa-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5daa-175">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5daa-176">C#</span><span class="sxs-lookup"><span data-stu-id="d5daa-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5daa-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5daa-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5daa-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5daa-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d5daa-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5daa-179">Response</span></span>

<span data-ttu-id="d5daa-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d5daa-180">The following is an example of the response.</span></span>

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

<span data-ttu-id="d5daa-181">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="d5daa-181">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
