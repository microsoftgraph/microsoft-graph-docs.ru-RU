---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Получение сведений об активных пользователях Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2f703f7b1bc67c277c5c7256c305b95905fce20c
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589046"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="df689-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="df689-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="df689-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df689-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df689-105">Получение сведений об активных пользователях Office 365.</span><span class="sxs-lookup"><span data-stu-id="df689-105">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="df689-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="df689-106">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="df689-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df689-107">Permissions</span></span>

<span data-ttu-id="df689-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df689-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df689-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df689-110">Permission type</span></span>                        | <span data-ttu-id="df689-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df689-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="df689-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df689-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="df689-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="df689-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="df689-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df689-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df689-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df689-115">Not supported.</span></span>                           |
| <span data-ttu-id="df689-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df689-116">Application</span></span>                            | <span data-ttu-id="df689-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="df689-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="df689-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="df689-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="df689-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="df689-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="df689-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df689-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="df689-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="df689-121">Function parameters</span></span>

<span data-ttu-id="df689-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="df689-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="df689-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="df689-123">Parameter</span></span> | <span data-ttu-id="df689-124">Тип</span><span class="sxs-lookup"><span data-stu-id="df689-124">Type</span></span>   | <span data-ttu-id="df689-125">Описание</span><span class="sxs-lookup"><span data-stu-id="df689-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="df689-126">period</span><span class="sxs-lookup"><span data-stu-id="df689-126">period</span></span>    | <span data-ttu-id="df689-127">string</span><span class="sxs-lookup"><span data-stu-id="df689-127">string</span></span> | <span data-ttu-id="df689-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="df689-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="df689-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="df689-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="df689-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="df689-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="df689-131">date</span><span class="sxs-lookup"><span data-stu-id="df689-131">date</span></span>      | <span data-ttu-id="df689-132">Date</span><span class="sxs-lookup"><span data-stu-id="df689-132">Date</span></span>   | <span data-ttu-id="df689-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="df689-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="df689-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="df689-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="df689-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="df689-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="df689-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="df689-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="df689-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="df689-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="df689-138">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="df689-138">The default output type is text/csv.</span></span> <span data-ttu-id="df689-139">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="df689-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df689-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df689-140">Request headers</span></span>

| <span data-ttu-id="df689-141">Имя</span><span class="sxs-lookup"><span data-stu-id="df689-141">Name</span></span>          | <span data-ttu-id="df689-142">Описание</span><span class="sxs-lookup"><span data-stu-id="df689-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="df689-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df689-143">Authorization</span></span> | <span data-ttu-id="df689-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df689-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="df689-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="df689-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="df689-147">CSV</span><span class="sxs-lookup"><span data-stu-id="df689-147">CSV</span></span>

<span data-ttu-id="df689-148">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="df689-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="df689-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="df689-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="df689-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="df689-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="df689-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="df689-151">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="df689-152">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="df689-152">Report Refresh Date</span></span>
- <span data-ttu-id="df689-153">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="df689-153">User Principal Name</span></span>
- <span data-ttu-id="df689-154">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="df689-154">Display Name</span></span>
- <span data-ttu-id="df689-155">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="df689-155">Is Deleted</span></span>
- <span data-ttu-id="df689-156">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="df689-156">Deleted Date</span></span>
- <span data-ttu-id="df689-157">"Has Exchange License" (Есть лицензия на Exchange);</span><span class="sxs-lookup"><span data-stu-id="df689-157">Has Exchange License</span></span>
- <span data-ttu-id="df689-158">"Has OneDrive License" (Есть лицензия на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="df689-158">Has OneDrive License</span></span>
- <span data-ttu-id="df689-159">"Has SharePoint License" (Есть лицензия на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="df689-159">Has SharePoint License</span></span>
- <span data-ttu-id="df689-160">"Has Skype For Business License" (Есть лицензия на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="df689-160">Has Skype For Business License</span></span>
- <span data-ttu-id="df689-161">"Has Yammer License" (Есть лицензия на Yammer);</span><span class="sxs-lookup"><span data-stu-id="df689-161">Has Yammer License</span></span>
- <span data-ttu-id="df689-162">"Has Teams License" (Есть лицензия на Teams);</span><span class="sxs-lookup"><span data-stu-id="df689-162">Has Teams License</span></span>
- <span data-ttu-id="df689-163">"Exchange Last Activity Date" (Дата последнего действия в Exchange);</span><span class="sxs-lookup"><span data-stu-id="df689-163">Exchange Last Activity Date</span></span>
- <span data-ttu-id="df689-164">"OneDrive Last Activity Date" (Дата последнего действия в OneDrive);</span><span class="sxs-lookup"><span data-stu-id="df689-164">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="df689-165">"SharePoint Last Activity Date" (Дата последнего действия в SharePoint);</span><span class="sxs-lookup"><span data-stu-id="df689-165">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="df689-166">"Skype For Business Last Activity Date" (Дата последнего действия в Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="df689-166">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="df689-167">"Yammer Last Activity Date" (Дата последнего действия в Yammer);</span><span class="sxs-lookup"><span data-stu-id="df689-167">Yammer Last Activity Date</span></span>
- <span data-ttu-id="df689-168">"Teams Last Activity Date" (Дата последнего действия в Teams);</span><span class="sxs-lookup"><span data-stu-id="df689-168">Teams Last Activity Date</span></span>
- <span data-ttu-id="df689-169">"Exchange License Assign Date" (Дата назначения лицензии на Exchange);</span><span class="sxs-lookup"><span data-stu-id="df689-169">Exchange License Assign Date</span></span>
- <span data-ttu-id="df689-170">"OneDrive License Assign Date" (Дата назначения лицензии на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="df689-170">OneDrive License Assign Date</span></span>
- <span data-ttu-id="df689-171">"SharePoint License Assign Date" (Дата назначения лицензии на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="df689-171">SharePoint License Assign Date</span></span>
- <span data-ttu-id="df689-172">"Skype For Business License Assign Date" (Дата назначения лицензии на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="df689-172">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="df689-173">"Yammer License Assign Date" (Дата назначения лицензии на Yammer);</span><span class="sxs-lookup"><span data-stu-id="df689-173">Yammer License Assign Date</span></span>
- <span data-ttu-id="df689-174">"Teams License Assign Date" (Дата назначения лицензии на Teams);</span><span class="sxs-lookup"><span data-stu-id="df689-174">Teams License Assign Date</span></span>
- <span data-ttu-id="df689-175">"Assigned Products" (Назначенные продукты).</span><span class="sxs-lookup"><span data-stu-id="df689-175">Assigned Products</span></span>

<span data-ttu-id="df689-176">Следующие столбцы не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="df689-176">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="df689-177">"Has Yammer License" (Есть лицензия на Yammer);</span><span class="sxs-lookup"><span data-stu-id="df689-177">Has Yammer License</span></span>
- <span data-ttu-id="df689-178">"Has Teams License" (Есть лицензия на Teams);</span><span class="sxs-lookup"><span data-stu-id="df689-178">Has Teams License</span></span>
- <span data-ttu-id="df689-179">"Yammer Last Activity Date" (Дата последнего действия в Yammer);</span><span class="sxs-lookup"><span data-stu-id="df689-179">Yammer Last Activity Date</span></span>
- <span data-ttu-id="df689-180">"Teams Last Activity Date" (Дата последнего действия в Teams);</span><span class="sxs-lookup"><span data-stu-id="df689-180">Teams Last Activity Date</span></span>
- <span data-ttu-id="df689-181">"Yammer License Assign Date" (Дата назначения лицензии на Yammer);</span><span class="sxs-lookup"><span data-stu-id="df689-181">Yammer License Assign Date</span></span>
- <span data-ttu-id="df689-182">"Teams License Assign Date" (Дата назначения лицензии на Teams);</span><span class="sxs-lookup"><span data-stu-id="df689-182">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="df689-183">JSON</span><span class="sxs-lookup"><span data-stu-id="df689-183">JSON</span></span>

<span data-ttu-id="df689-184">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="df689-184">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="df689-185">Следующие свойства в объекте **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21vianet:</span><span class="sxs-lookup"><span data-stu-id="df689-185">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="df689-186">хасяммерлиценсе</span><span class="sxs-lookup"><span data-stu-id="df689-186">hasYammerLicense</span></span>
- <span data-ttu-id="df689-187">хастеамслиценсе</span><span class="sxs-lookup"><span data-stu-id="df689-187">hasTeamsLicense</span></span>
- <span data-ttu-id="df689-188">яммерластактивитидате</span><span class="sxs-lookup"><span data-stu-id="df689-188">yammerLastActivityDate</span></span>
- <span data-ttu-id="df689-189">теамсластактивитидате</span><span class="sxs-lookup"><span data-stu-id="df689-189">teamsLastActivityDate</span></span>
- <span data-ttu-id="df689-190">яммерлиценсеассигндате</span><span class="sxs-lookup"><span data-stu-id="df689-190">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="df689-191">теамслиценсеассигндате</span><span class="sxs-lookup"><span data-stu-id="df689-191">teamsLicenseAssignDate</span></span>

<span data-ttu-id="df689-192">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="df689-192">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="df689-193">Пример</span><span class="sxs-lookup"><span data-stu-id="df689-193">Example</span></span>

### <a name="csv"></a><span data-ttu-id="df689-194">CSV</span><span class="sxs-lookup"><span data-stu-id="df689-194">CSV</span></span>

<span data-ttu-id="df689-195">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="df689-195">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="df689-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="df689-196">Request</span></span>

<span data-ttu-id="df689-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df689-197">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="df689-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="df689-198">Response</span></span>

<span data-ttu-id="df689-199">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="df689-199">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="df689-200">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="df689-200">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="df689-201">JSON</span><span class="sxs-lookup"><span data-stu-id="df689-201">JSON</span></span>

<span data-ttu-id="df689-202">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="df689-202">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="df689-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="df689-203">Request</span></span>

<span data-ttu-id="df689-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df689-204">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="df689-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="df689-205">Response</span></span>

<span data-ttu-id="df689-206">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="df689-206">The following is an example of the response.</span></span>

> <span data-ttu-id="df689-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df689-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
