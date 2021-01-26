---
title: 'reportRoot: getM365AppUserDetail'
description: Получите отчет с подробными сведениями о том, какие приложения и платформы использовали пользователи.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: cd0974fd22dc3e7f8ea71f86acdae4585d231dc4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983792"
---
# <a name="reportroot-getm365appuserdetail"></a><span data-ttu-id="cda1e-103">reportRoot: getM365AppUserDetail</span><span class="sxs-lookup"><span data-stu-id="cda1e-103">reportRoot: getM365AppUserDetail</span></span>

<span data-ttu-id="cda1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cda1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cda1e-105">Получите отчет с подробными сведениями о том, какие приложения и платформы использовали пользователи.</span><span class="sxs-lookup"><span data-stu-id="cda1e-105">Get a report that provides the details about which apps and platforms users have used.</span></span>

> <span data-ttu-id="cda1e-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 об использовании приложений Microsoft 365.](/microsoft-365/admin/activity-reports/microsoft365-apps-usage)</span><span class="sxs-lookup"><span data-stu-id="cda1e-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 Apps usage](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span></span>

## <a name="permissions"></a><span data-ttu-id="cda1e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cda1e-107">Permissions</span></span>

<span data-ttu-id="cda1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cda1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cda1e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cda1e-110">Permission type</span></span>                        | <span data-ttu-id="cda1e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cda1e-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="cda1e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cda1e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cda1e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cda1e-113">Reports.Read.All</span></span>                            |
| <span data-ttu-id="cda1e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cda1e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cda1e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cda1e-115">Not supported.</span></span>                              |
| <span data-ttu-id="cda1e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cda1e-116">Application</span></span>                            | <span data-ttu-id="cda1e-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cda1e-117">Reports.Read.All</span></span>                            |

> <span data-ttu-id="cda1e-118">**Примечание.** Чтобы делегировать разрешения, позволяющие приложениям читать отчеты об использовании служб от имени пользователя, администратор клиента должен на назначенную пользователю роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cda1e-118">**Note:** For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="cda1e-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="cda1e-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="cda1e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cda1e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getM365AppUserDetail(period='{period_value}')
GET /reports/getM365AppUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="cda1e-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="cda1e-121">Function parameters</span></span>

<span data-ttu-id="cda1e-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="cda1e-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cda1e-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="cda1e-123">Parameter</span></span> | <span data-ttu-id="cda1e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="cda1e-124">Type</span></span>   | <span data-ttu-id="cda1e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="cda1e-125">Description</span></span>                                                                                                                                                                                                                                             |
| :-------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="cda1e-126">period</span><span class="sxs-lookup"><span data-stu-id="cda1e-126">period</span></span>    | <span data-ttu-id="cda1e-127">string</span><span class="sxs-lookup"><span data-stu-id="cda1e-127">string</span></span> | <span data-ttu-id="cda1e-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="cda1e-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cda1e-129">Поддерживаемые значения для {period_value}: `D7` , `D30` , и `D90` `D180` .</span><span class="sxs-lookup"><span data-stu-id="cda1e-129">The supported values for {period_value} are: `D7`, `D30`, `D90`, and `D180`.</span></span> <span data-ttu-id="cda1e-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="cda1e-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="cda1e-131">date</span><span class="sxs-lookup"><span data-stu-id="cda1e-131">date</span></span>      | <span data-ttu-id="cda1e-132">Date</span><span class="sxs-lookup"><span data-stu-id="cda1e-132">Date</span></span>   | <span data-ttu-id="cda1e-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="cda1e-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="cda1e-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="cda1e-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="cda1e-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="cda1e-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span>          |

> <span data-ttu-id="cda1e-136">**Примечание.** Необходимо установить `period` url-адрес `date` или его url-адрес.</span><span class="sxs-lookup"><span data-stu-id="cda1e-136">**Note:** You need to set either `period` or `date` in the URL.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="cda1e-137">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cda1e-137">Optional query parameters</span></span>

<span data-ttu-id="cda1e-138">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cda1e-138">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cda1e-139">Тип выходных данных по умолчанию — text/csv.</span><span class="sxs-lookup"><span data-stu-id="cda1e-139">The default output type is text/csv.</span></span> <span data-ttu-id="cda1e-140">Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData, чтобы задать для выходных данных по умолчанию значение `$format` text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="cda1e-140">However, if you want to specify the output type, you can use the OData `$format` query parameter to set the default output to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cda1e-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cda1e-141">Request headers</span></span>

| <span data-ttu-id="cda1e-142">Имя</span><span class="sxs-lookup"><span data-stu-id="cda1e-142">Name</span></span>          | <span data-ttu-id="cda1e-143">Описание</span><span class="sxs-lookup"><span data-stu-id="cda1e-143">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cda1e-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cda1e-144">Authorization</span></span> | <span data-ttu-id="cda1e-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cda1e-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cda1e-147">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cda1e-147">Request body</span></span>

<span data-ttu-id="cda1e-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cda1e-148">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="cda1e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="cda1e-149">Response</span></span>

<span data-ttu-id="cda1e-150">В случае успеха этот метод возвращает код отклика и `200 OK` объект [отчета](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cda1e-150">If successful, this method returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) object in the response body.</span></span> <span data-ttu-id="cda1e-151">Данные отчета содержатся в свойстве **контента** объекта **report.**</span><span class="sxs-lookup"><span data-stu-id="cda1e-151">Report data is contained in the **content** property of the **report** object.</span></span>

### <a name="csv"></a><span data-ttu-id="cda1e-152">CSV</span><span class="sxs-lookup"><span data-stu-id="cda1e-152">CSV</span></span>

<span data-ttu-id="cda1e-153">В случае успешного запроса свойства **контента** возвращается ответ, который перенаправляет на URL-адрес предварительной загрузки для `302 Found` отчета.</span><span class="sxs-lookup"><span data-stu-id="cda1e-153">If successful, requesting the **content** property returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cda1e-154">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="cda1e-154">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cda1e-155">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cda1e-155">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cda1e-156">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="cda1e-156">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="cda1e-157">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="cda1e-157">Report Refresh Date</span></span>
- <span data-ttu-id="cda1e-158">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="cda1e-158">User Principal Name</span></span>
- <span data-ttu-id="cda1e-159">Дата последней активации</span><span class="sxs-lookup"><span data-stu-id="cda1e-159">Last Activation Date</span></span>
- <span data-ttu-id="cda1e-160">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="cda1e-160">Last Activity Date</span></span>
- <span data-ttu-id="cda1e-161">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="cda1e-161">Report Period</span></span>
- <span data-ttu-id="cda1e-162">Windows</span><span class="sxs-lookup"><span data-stu-id="cda1e-162">Windows</span></span>
- <span data-ttu-id="cda1e-163">Mac</span><span class="sxs-lookup"><span data-stu-id="cda1e-163">Mac</span></span>
- <span data-ttu-id="cda1e-164">Для мобильных устройств</span><span class="sxs-lookup"><span data-stu-id="cda1e-164">Mobile</span></span>
- <span data-ttu-id="cda1e-165">Web</span><span class="sxs-lookup"><span data-stu-id="cda1e-165">Web</span></span>
- <span data-ttu-id="cda1e-166">Outlook</span><span class="sxs-lookup"><span data-stu-id="cda1e-166">Outlook</span></span>
- <span data-ttu-id="cda1e-167">Word</span><span class="sxs-lookup"><span data-stu-id="cda1e-167">Word</span></span>
- <span data-ttu-id="cda1e-168">Excel</span><span class="sxs-lookup"><span data-stu-id="cda1e-168">Excel</span></span>
- <span data-ttu-id="cda1e-169">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="cda1e-169">PowerPoint</span></span>
- <span data-ttu-id="cda1e-170">OneNote</span><span class="sxs-lookup"><span data-stu-id="cda1e-170">OneNote</span></span>
- <span data-ttu-id="cda1e-171">Teams</span><span class="sxs-lookup"><span data-stu-id="cda1e-171">Teams</span></span>
- <span data-ttu-id="cda1e-172">Outlook (Windows)</span><span class="sxs-lookup"><span data-stu-id="cda1e-172">Outlook (Windows)</span></span>
- <span data-ttu-id="cda1e-173">Word (Windows)</span><span class="sxs-lookup"><span data-stu-id="cda1e-173">Word (Windows)</span></span>
- <span data-ttu-id="cda1e-174">Excel (Windows)</span><span class="sxs-lookup"><span data-stu-id="cda1e-174">Excel (Windows)</span></span>
- <span data-ttu-id="cda1e-175">PowerPoint (Windows)</span><span class="sxs-lookup"><span data-stu-id="cda1e-175">PowerPoint (Windows)</span></span>
- <span data-ttu-id="cda1e-176">OneNote (Windows)</span><span class="sxs-lookup"><span data-stu-id="cda1e-176">OneNote (Windows)</span></span>
- <span data-ttu-id="cda1e-177">Teams (Windows)</span><span class="sxs-lookup"><span data-stu-id="cda1e-177">Teams (Windows)</span></span>
- <span data-ttu-id="cda1e-178">Outlook (Mac)</span><span class="sxs-lookup"><span data-stu-id="cda1e-178">Outlook (Mac)</span></span>
- <span data-ttu-id="cda1e-179">Word (Mac)</span><span class="sxs-lookup"><span data-stu-id="cda1e-179">Word (Mac)</span></span>
- <span data-ttu-id="cda1e-180">Excel (Mac)</span><span class="sxs-lookup"><span data-stu-id="cda1e-180">Excel (Mac)</span></span>
- <span data-ttu-id="cda1e-181">PowerPoint (Mac)</span><span class="sxs-lookup"><span data-stu-id="cda1e-181">PowerPoint (Mac)</span></span>
- <span data-ttu-id="cda1e-182">OneNote (Mac)</span><span class="sxs-lookup"><span data-stu-id="cda1e-182">OneNote (Mac)</span></span>
- <span data-ttu-id="cda1e-183">Teams (Mac)</span><span class="sxs-lookup"><span data-stu-id="cda1e-183">Teams (Mac)</span></span>
- <span data-ttu-id="cda1e-184">Outlook (Mobile)</span><span class="sxs-lookup"><span data-stu-id="cda1e-184">Outlook (Mobile)</span></span>
- <span data-ttu-id="cda1e-185">Word (Mobile)</span><span class="sxs-lookup"><span data-stu-id="cda1e-185">Word (Mobile)</span></span>
- <span data-ttu-id="cda1e-186">Excel (мобильные устройства)</span><span class="sxs-lookup"><span data-stu-id="cda1e-186">Excel (Mobile)</span></span>
- <span data-ttu-id="cda1e-187">PowerPoint (Mobile)</span><span class="sxs-lookup"><span data-stu-id="cda1e-187">PowerPoint (Mobile)</span></span>
- <span data-ttu-id="cda1e-188">OneNote (Mobile)</span><span class="sxs-lookup"><span data-stu-id="cda1e-188">OneNote (Mobile)</span></span>
- <span data-ttu-id="cda1e-189">Teams (мобильные устройства)</span><span class="sxs-lookup"><span data-stu-id="cda1e-189">Teams (Mobile)</span></span>
- <span data-ttu-id="cda1e-190">Outlook (Web)</span><span class="sxs-lookup"><span data-stu-id="cda1e-190">Outlook (Web)</span></span>
- <span data-ttu-id="cda1e-191">Word (Интернет)</span><span class="sxs-lookup"><span data-stu-id="cda1e-191">Word (Web)</span></span>
- <span data-ttu-id="cda1e-192">Excel (Интернет)</span><span class="sxs-lookup"><span data-stu-id="cda1e-192">Excel (Web)</span></span>
- <span data-ttu-id="cda1e-193">PowerPoint (Web)</span><span class="sxs-lookup"><span data-stu-id="cda1e-193">PowerPoint (Web)</span></span>
- <span data-ttu-id="cda1e-194">OneNote (Web)</span><span class="sxs-lookup"><span data-stu-id="cda1e-194">OneNote (Web)</span></span>
- <span data-ttu-id="cda1e-195">Teams (Интернет)</span><span class="sxs-lookup"><span data-stu-id="cda1e-195">Teams (Web)</span></span>

### <a name="json"></a><span data-ttu-id="cda1e-196">JSON</span><span class="sxs-lookup"><span data-stu-id="cda1e-196">JSON</span></span>

<span data-ttu-id="cda1e-197">В случае успеха запрос свойства **контента** возвращает код отклика и `200 OK` объект JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cda1e-197">If successful, requesting the **content** property returns a `200 OK` response code and a JSON object in response body.</span></span>

<span data-ttu-id="cda1e-198">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="cda1e-198">The default page size for this request is 200 items.</span></span>

## <a name="examples"></a><span data-ttu-id="cda1e-199">Примеры</span><span class="sxs-lookup"><span data-stu-id="cda1e-199">Examples</span></span>

### <a name="example-1-csv-output"></a><span data-ttu-id="cda1e-200">Пример 1. Выходные данные CSV</span><span class="sxs-lookup"><span data-stu-id="cda1e-200">Example 1: CSV output</span></span>

<span data-ttu-id="cda1e-201">Ниже приводится пример вывода CSV-данных.</span><span class="sxs-lookup"><span data-stu-id="cda1e-201">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cda1e-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="cda1e-202">Request</span></span>

<span data-ttu-id="cda1e-203">Ниже приводится пример запроса на получения **свойства контента.**</span><span class="sxs-lookup"><span data-stu-id="cda1e-203">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="cda1e-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="cda1e-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCounDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="cda1e-205">C#</span><span class="sxs-lookup"><span data-stu-id="cda1e-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercoundetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cda1e-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cda1e-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercoundetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cda1e-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cda1e-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercoundetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cda1e-208">Java</span><span class="sxs-lookup"><span data-stu-id="cda1e-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercoundetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="cda1e-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="cda1e-209">Response</span></span>

<span data-ttu-id="cda1e-210">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cda1e-210">The following is an example of the response.</span></span>

<!-- { "blockType": "response" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cda1e-211">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="cda1e-211">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activation Date,Last Activity Date,Report Period,Windows,Mac,Mobile,Web,Outlook,Word,Excel,PowerPoint,OneNote,Teams,Outlook (Windows),Word (Windows),Excel (Windows),PowerPoint (Windows),OneNote (Windows),Teams (Windows),Outlook (Mac),Word (Mac),Excel (Mac),PowerPoint (Mac),OneNote (Mac),Teams (Mac),Outlook (Mobile),Word (Mobile),Excel (Mobile),PowerPoint (Mobile),OneNote (Mobile),Teams (Mobile),Outlook (Web),Word (Web),Excel (Web),PowerPoint (Web),OneNote (Web),Teams (Web)
```

### <a name="example-2-json-output"></a><span data-ttu-id="cda1e-212">Пример 2. Выходные данные JSON</span><span class="sxs-lookup"><span data-stu-id="cda1e-212">Example 2: JSON output</span></span>

<span data-ttu-id="cda1e-213">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="cda1e-213">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cda1e-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="cda1e-214">Request</span></span>

<span data-ttu-id="cda1e-215">Ниже приводится пример запроса на получения **свойства контента.**</span><span class="sxs-lookup"><span data-stu-id="cda1e-215">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="cda1e-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="cda1e-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCountDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="cda1e-217">C#</span><span class="sxs-lookup"><span data-stu-id="cda1e-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercountdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cda1e-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cda1e-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercountdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cda1e-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cda1e-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercountdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cda1e-220">Java</span><span class="sxs-lookup"><span data-stu-id="cda1e-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercountdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="cda1e-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="cda1e-221">Response</span></span>

<span data-ttu-id="cda1e-222">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cda1e-222">The following is an example of the response.</span></span>

> <span data-ttu-id="cda1e-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cda1e-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 951

{
  "@odata.nextLink": "https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=application/json&$skiptoken=AAAAA",
  "value": [
    {
      "reportRefreshDate": "2020-06-30",
      "userPrincipalName": "admin@contoso.com",
      "lastActivationDate": "2020-05-22",
      "lastActivityDate": "2020-06-30",
      "details": [
        {
          "reportPeriod": 7,
          "windows": true,
          "mac": false,
          "mobile": true,
          "web": false,
          "outlook": false,
          "word": false,
          "excel": false,
          "powerPoint": false,
          "oneNote": false,
          "teams": true,
          "outlookWindows": false,
          "wordWindows": false,
          "excelWindows": false,
          "powerPointWindows": false,
          "oneNoteWindows": false,
          "teamsWindows": true,
          "outlookMac": false,
          "wordMac": false,
          "excelMac": false,
          "powerPointMac": false,
          "oneNoteMac": false,
          "teamsMac": false,
          "outlookMobile": false,
          "wordMobile": false,
          "excelMobile": false,
          "powerPointMobile": false,
          "oneNoteMobile": false,
          "teamsMobile": true,
          "outlookWeb": false,
          "wordWeb": false,
          "excelWeb": false,
          "powerPointWeb": false,
          "oneNoteWeb": false,
          "teamsWeb": true
        }
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
