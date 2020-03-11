---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Получение сведений об активных пользователях Office 365.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 126c838da1e2dd52b9a9da4956fc135f32c4ecd9
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591287"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="1745a-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="1745a-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="1745a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1745a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1745a-105">Получение сведений об активных пользователях Office 365.</span><span class="sxs-lookup"><span data-stu-id="1745a-105">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="1745a-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="1745a-106">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="1745a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1745a-107">Permissions</span></span>

<span data-ttu-id="1745a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1745a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1745a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1745a-110">Permission type</span></span>                        | <span data-ttu-id="1745a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1745a-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1745a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1745a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1745a-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1745a-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1745a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1745a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1745a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1745a-115">Not supported.</span></span>                           |
| <span data-ttu-id="1745a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1745a-116">Application</span></span>                            | <span data-ttu-id="1745a-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1745a-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="1745a-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1745a-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="1745a-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="1745a-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="1745a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1745a-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="1745a-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="1745a-121">Function parameters</span></span>

<span data-ttu-id="1745a-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="1745a-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="1745a-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="1745a-123">Parameter</span></span> | <span data-ttu-id="1745a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="1745a-124">Type</span></span>   | <span data-ttu-id="1745a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1745a-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1745a-126">period</span><span class="sxs-lookup"><span data-stu-id="1745a-126">period</span></span>    | <span data-ttu-id="1745a-127">string</span><span class="sxs-lookup"><span data-stu-id="1745a-127">string</span></span> | <span data-ttu-id="1745a-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="1745a-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1745a-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="1745a-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1745a-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="1745a-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="1745a-131">date</span><span class="sxs-lookup"><span data-stu-id="1745a-131">date</span></span>      | <span data-ttu-id="1745a-132">Date</span><span class="sxs-lookup"><span data-stu-id="1745a-132">Date</span></span>   | <span data-ttu-id="1745a-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="1745a-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="1745a-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="1745a-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="1745a-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="1745a-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="1745a-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="1745a-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1745a-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1745a-137">Request headers</span></span>

| <span data-ttu-id="1745a-138">Имя</span><span class="sxs-lookup"><span data-stu-id="1745a-138">Name</span></span>          | <span data-ttu-id="1745a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="1745a-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="1745a-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1745a-140">Authorization</span></span> | <span data-ttu-id="1745a-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1745a-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="1745a-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1745a-143">If-None-Match</span></span> | <span data-ttu-id="1745a-144">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="1745a-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1745a-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1745a-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1745a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="1745a-146">Response</span></span>

<span data-ttu-id="1745a-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="1745a-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1745a-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="1745a-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1745a-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1745a-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1745a-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="1745a-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1745a-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="1745a-151">Report Refresh Date</span></span>
- <span data-ttu-id="1745a-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="1745a-152">User Principal Name</span></span>
- <span data-ttu-id="1745a-153">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="1745a-153">Display Name</span></span>
- <span data-ttu-id="1745a-154">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="1745a-154">Is Deleted</span></span>
- <span data-ttu-id="1745a-155">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="1745a-155">Deleted Date</span></span>
- <span data-ttu-id="1745a-156">"Has Exchange License" (Есть лицензия на Exchange);</span><span class="sxs-lookup"><span data-stu-id="1745a-156">Has Exchange License</span></span>
- <span data-ttu-id="1745a-157">"Has OneDrive License" (Есть лицензия на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="1745a-157">Has OneDrive License</span></span>
- <span data-ttu-id="1745a-158">"Has SharePoint License" (Есть лицензия на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="1745a-158">Has SharePoint License</span></span>
- <span data-ttu-id="1745a-159">"Has Skype For Business License" (Есть лицензия на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="1745a-159">Has Skype For Business License</span></span>
- <span data-ttu-id="1745a-160">"Has Yammer License" (Есть лицензия на Yammer);</span><span class="sxs-lookup"><span data-stu-id="1745a-160">Has Yammer License</span></span>
- <span data-ttu-id="1745a-161">"Has Teams License" (Есть лицензия на Teams);</span><span class="sxs-lookup"><span data-stu-id="1745a-161">Has Teams License</span></span>
- <span data-ttu-id="1745a-162">"Exchange Last Activity Date" (Дата последнего действия в Exchange);</span><span class="sxs-lookup"><span data-stu-id="1745a-162">Exchange Last Activity Date</span></span>
- <span data-ttu-id="1745a-163">"OneDrive Last Activity Date" (Дата последнего действия в OneDrive);</span><span class="sxs-lookup"><span data-stu-id="1745a-163">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="1745a-164">"SharePoint Last Activity Date" (Дата последнего действия в SharePoint);</span><span class="sxs-lookup"><span data-stu-id="1745a-164">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="1745a-165">"Skype For Business Last Activity Date" (Дата последнего действия в Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="1745a-165">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="1745a-166">"Yammer Last Activity Date" (Дата последнего действия в Yammer);</span><span class="sxs-lookup"><span data-stu-id="1745a-166">Yammer Last Activity Date</span></span>
- <span data-ttu-id="1745a-167">"Teams Last Activity Date" (Дата последнего действия в Teams);</span><span class="sxs-lookup"><span data-stu-id="1745a-167">Teams Last Activity Date</span></span>
- <span data-ttu-id="1745a-168">"Exchange License Assign Date" (Дата назначения лицензии на Exchange);</span><span class="sxs-lookup"><span data-stu-id="1745a-168">Exchange License Assign Date</span></span>
- <span data-ttu-id="1745a-169">"OneDrive License Assign Date" (Дата назначения лицензии на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="1745a-169">OneDrive License Assign Date</span></span>
- <span data-ttu-id="1745a-170">"SharePoint License Assign Date" (Дата назначения лицензии на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="1745a-170">SharePoint License Assign Date</span></span>
- <span data-ttu-id="1745a-171">"Skype For Business License Assign Date" (Дата назначения лицензии на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="1745a-171">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="1745a-172">"Yammer License Assign Date" (Дата назначения лицензии на Yammer);</span><span class="sxs-lookup"><span data-stu-id="1745a-172">Yammer License Assign Date</span></span>
- <span data-ttu-id="1745a-173">"Teams License Assign Date" (Дата назначения лицензии на Teams);</span><span class="sxs-lookup"><span data-stu-id="1745a-173">Teams License Assign Date</span></span>
- <span data-ttu-id="1745a-174">"Assigned Products" (Назначенные продукты).</span><span class="sxs-lookup"><span data-stu-id="1745a-174">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="1745a-175">Пример</span><span class="sxs-lookup"><span data-stu-id="1745a-175">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1745a-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="1745a-176">Request</span></span>

<span data-ttu-id="1745a-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1745a-177">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="1745a-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="1745a-178">Response</span></span>

<span data-ttu-id="1745a-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1745a-179">The following is an example of the response.</span></span>

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

<span data-ttu-id="1745a-180">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="1745a-180">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
