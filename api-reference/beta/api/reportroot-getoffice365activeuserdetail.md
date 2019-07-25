---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Получение сведений об активных пользователях Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e41c67aa2b21a97b96fe42132bb65491220d9b6c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873462"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="9a8ce-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="9a8ce-103">reportRoot: getOffice365ActiveUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a8ce-104">Получение сведений об активных пользователях Office 365.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="9a8ce-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="9a8ce-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="9a8ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a8ce-106">Permissions</span></span>

<span data-ttu-id="9a8ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a8ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a8ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a8ce-109">Permission type</span></span>                        | <span data-ttu-id="9a8ce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a8ce-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9a8ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a8ce-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a8ce-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a8ce-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9a8ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a8ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a8ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-114">Not supported.</span></span>                           |
| <span data-ttu-id="9a8ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a8ce-115">Application</span></span>                            | <span data-ttu-id="9a8ce-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a8ce-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9a8ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a8ce-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="9a8ce-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="9a8ce-118">Function parameters</span></span>

<span data-ttu-id="9a8ce-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="9a8ce-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="9a8ce-120">Parameter</span></span> | <span data-ttu-id="9a8ce-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9a8ce-121">Type</span></span>   | <span data-ttu-id="9a8ce-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9a8ce-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9a8ce-123">period</span><span class="sxs-lookup"><span data-stu-id="9a8ce-123">period</span></span>    | <span data-ttu-id="9a8ce-124">string</span><span class="sxs-lookup"><span data-stu-id="9a8ce-124">string</span></span> | <span data-ttu-id="9a8ce-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9a8ce-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9a8ce-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="9a8ce-128">date</span><span class="sxs-lookup"><span data-stu-id="9a8ce-128">date</span></span>      | <span data-ttu-id="9a8ce-129">Date</span><span class="sxs-lookup"><span data-stu-id="9a8ce-129">Date</span></span>   | <span data-ttu-id="9a8ce-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="9a8ce-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="9a8ce-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="9a8ce-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="9a8ce-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9a8ce-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-135">The default output type is text/csv.</span></span> <span data-ttu-id="9a8ce-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a8ce-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a8ce-137">Request headers</span></span>

| <span data-ttu-id="9a8ce-138">Имя</span><span class="sxs-lookup"><span data-stu-id="9a8ce-138">Name</span></span>          | <span data-ttu-id="9a8ce-139">Описание</span><span class="sxs-lookup"><span data-stu-id="9a8ce-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9a8ce-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a8ce-140">Authorization</span></span> | <span data-ttu-id="9a8ce-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9a8ce-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a8ce-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9a8ce-144">CSV</span><span class="sxs-lookup"><span data-stu-id="9a8ce-144">CSV</span></span>

<span data-ttu-id="9a8ce-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9a8ce-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9a8ce-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9a8ce-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="9a8ce-148">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="9a8ce-149">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-149">Report Refresh Date</span></span>
- <span data-ttu-id="9a8ce-150">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-150">User Principal Name</span></span>
- <span data-ttu-id="9a8ce-151">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-151">Display Name</span></span>
- <span data-ttu-id="9a8ce-152">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-152">Is Deleted</span></span>
- <span data-ttu-id="9a8ce-153">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-153">Deleted Date</span></span>
- <span data-ttu-id="9a8ce-154">"Has Exchange License" (Есть лицензия на Exchange);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-154">Has Exchange License</span></span>
- <span data-ttu-id="9a8ce-155">"Has OneDrive License" (Есть лицензия на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-155">Has OneDrive License</span></span>
- <span data-ttu-id="9a8ce-156">"Has SharePoint License" (Есть лицензия на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-156">Has SharePoint License</span></span>
- <span data-ttu-id="9a8ce-157">"Has Skype For Business License" (Есть лицензия на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-157">Has Skype For Business License</span></span>
- <span data-ttu-id="9a8ce-158">"Has Yammer License" (Есть лицензия на Yammer);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-158">Has Yammer License</span></span>
- <span data-ttu-id="9a8ce-159">"Has Teams License" (Есть лицензия на Teams);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-159">Has Teams License</span></span>
- <span data-ttu-id="9a8ce-160">"Exchange Last Activity Date" (Дата последнего действия в Exchange);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-160">Exchange Last Activity Date</span></span>
- <span data-ttu-id="9a8ce-161">"OneDrive Last Activity Date" (Дата последнего действия в OneDrive);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-161">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="9a8ce-162">"SharePoint Last Activity Date" (Дата последнего действия в SharePoint);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-162">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="9a8ce-163">"Skype For Business Last Activity Date" (Дата последнего действия в Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-163">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="9a8ce-164">"Yammer Last Activity Date" (Дата последнего действия в Yammer);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-164">Yammer Last Activity Date</span></span>
- <span data-ttu-id="9a8ce-165">"Teams Last Activity Date" (Дата последнего действия в Teams);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-165">Teams Last Activity Date</span></span>
- <span data-ttu-id="9a8ce-166">"Exchange License Assign Date" (Дата назначения лицензии на Exchange);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-166">Exchange License Assign Date</span></span>
- <span data-ttu-id="9a8ce-167">"OneDrive License Assign Date" (Дата назначения лицензии на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-167">OneDrive License Assign Date</span></span>
- <span data-ttu-id="9a8ce-168">"SharePoint License Assign Date" (Дата назначения лицензии на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-168">SharePoint License Assign Date</span></span>
- <span data-ttu-id="9a8ce-169">"Skype For Business License Assign Date" (Дата назначения лицензии на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-169">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="9a8ce-170">"Yammer License Assign Date" (Дата назначения лицензии на Yammer);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-170">Yammer License Assign Date</span></span>
- <span data-ttu-id="9a8ce-171">"Teams License Assign Date" (Дата назначения лицензии на Teams);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-171">Teams License Assign Date</span></span>
- <span data-ttu-id="9a8ce-172">"Assigned Products" (Назначенные продукты).</span><span class="sxs-lookup"><span data-stu-id="9a8ce-172">Assigned Products</span></span>

<span data-ttu-id="9a8ce-173">Следующие столбцы не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="9a8ce-173">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="9a8ce-174">"Has Yammer License" (Есть лицензия на Yammer);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-174">Has Yammer License</span></span>
- <span data-ttu-id="9a8ce-175">"Has Teams License" (Есть лицензия на Teams);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-175">Has Teams License</span></span>
- <span data-ttu-id="9a8ce-176">"Yammer Last Activity Date" (Дата последнего действия в Yammer);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-176">Yammer Last Activity Date</span></span>
- <span data-ttu-id="9a8ce-177">"Teams Last Activity Date" (Дата последнего действия в Teams);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-177">Teams Last Activity Date</span></span>
- <span data-ttu-id="9a8ce-178">"Yammer License Assign Date" (Дата назначения лицензии на Yammer);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-178">Yammer License Assign Date</span></span>
- <span data-ttu-id="9a8ce-179">"Teams License Assign Date" (Дата назначения лицензии на Teams);</span><span class="sxs-lookup"><span data-stu-id="9a8ce-179">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="9a8ce-180">JSON</span><span class="sxs-lookup"><span data-stu-id="9a8ce-180">JSON</span></span>

<span data-ttu-id="9a8ce-181">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-181">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="9a8ce-182">Следующие свойства в объекте **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21vianet:</span><span class="sxs-lookup"><span data-stu-id="9a8ce-182">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="9a8ce-183">Хасяммерлиценсе</span><span class="sxs-lookup"><span data-stu-id="9a8ce-183">hasYammerLicense</span></span>
- <span data-ttu-id="9a8ce-184">Хастеамслиценсе</span><span class="sxs-lookup"><span data-stu-id="9a8ce-184">hasTeamsLicense</span></span>
- <span data-ttu-id="9a8ce-185">Яммерластактивитидате</span><span class="sxs-lookup"><span data-stu-id="9a8ce-185">yammerLastActivityDate</span></span>
- <span data-ttu-id="9a8ce-186">Теамсластактивитидате</span><span class="sxs-lookup"><span data-stu-id="9a8ce-186">teamsLastActivityDate</span></span>
- <span data-ttu-id="9a8ce-187">Яммерлиценсеассигндате</span><span class="sxs-lookup"><span data-stu-id="9a8ce-187">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="9a8ce-188">Теамслиценсеассигндате</span><span class="sxs-lookup"><span data-stu-id="9a8ce-188">teamsLicenseAssignDate</span></span>

<span data-ttu-id="9a8ce-189">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-189">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="9a8ce-190">Пример</span><span class="sxs-lookup"><span data-stu-id="9a8ce-190">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9a8ce-191">CSV</span><span class="sxs-lookup"><span data-stu-id="9a8ce-191">CSV</span></span>

<span data-ttu-id="9a8ce-192">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-192">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9a8ce-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a8ce-193">Request</span></span>

<span data-ttu-id="9a8ce-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-194">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9a8ce-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a8ce-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a8ce-196">C#</span><span class="sxs-lookup"><span data-stu-id="9a8ce-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a8ce-197">Javascript</span><span class="sxs-lookup"><span data-stu-id="9a8ce-197">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a8ce-198">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9a8ce-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9a8ce-199">Java</span><span class="sxs-lookup"><span data-stu-id="9a8ce-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activeuserdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a8ce-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a8ce-200">Response</span></span>

<span data-ttu-id="9a8ce-201">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-201">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9a8ce-202">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-202">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
```

### <a name="json"></a><span data-ttu-id="9a8ce-203">JSON</span><span class="sxs-lookup"><span data-stu-id="9a8ce-203">JSON</span></span>

<span data-ttu-id="9a8ce-204">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-204">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9a8ce-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a8ce-205">Request</span></span>

<span data-ttu-id="9a8ce-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-206">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9a8ce-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a8ce-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a8ce-208">C#</span><span class="sxs-lookup"><span data-stu-id="9a8ce-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a8ce-209">Javascript</span><span class="sxs-lookup"><span data-stu-id="9a8ce-209">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a8ce-210">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9a8ce-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9a8ce-211">Java</span><span class="sxs-lookup"><span data-stu-id="9a8ce-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activeuserdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a8ce-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a8ce-212">Response</span></span>

<span data-ttu-id="9a8ce-213">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-213">The following is an example of the response.</span></span>

> <span data-ttu-id="9a8ce-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a8ce-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 853

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "hasExchangeLicense": true, 
      "hasOneDriveLicense": false, 
      "hasSharePointLicense": false, 
      "hasSkypeForBusinessLicense": false, 
      "hasYammerLicense": false, 
      "hasTeamsLicense": false, 
      "exchangeLastActivityDate": "2017-08-30", 
      "oneDriveLastActivityDate": null, 
      "sharePointLastActivityDate": null, 
      "skypeForBusinessLastActivityDate": null, 
      "yammerLastActivityDate": null, 
      "teamsLastActivityDate": null, 
      "exchangeLicenseAssignDate": "2016-05-03", 
      "oneDriveLicenseAssignDate": null, 
      "sharePointLicenseAssignDate": null, 
      "skypeForBusinessLicenseAssignDate": null, 
      "yammerLicenseAssignDate": null, 
      "teamsLicenseAssignDate": null, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ]
    }
  ]
}
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
