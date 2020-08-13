---
title: 'Reportroot.: getM365AppUserDetail'
description: Получите отчет, содержащий сведения о том, какие приложения и платформы используются пользователями.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 6abdd6334d5a96dc740ce80ad119f3f8d6efb1b0
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2020
ms.locfileid: "46658092"
---
# <a name="reportroot-getm365appuserdetail"></a><span data-ttu-id="a2eb3-103">Reportroot.: getM365AppUserDetail</span><span class="sxs-lookup"><span data-stu-id="a2eb3-103">reportRoot: getM365AppUserDetail</span></span>

<span data-ttu-id="a2eb3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2eb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2eb3-105">Получите отчет, содержащий сведения о том, какие приложения и платформы используются пользователями.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-105">Get a report that provides the details about which apps and platforms users have used.</span></span>

> <span data-ttu-id="a2eb3-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье microsoft 365 Reports — использование приложений microsoft 365](https://docs.microsoft.com/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span><span class="sxs-lookup"><span data-stu-id="a2eb3-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 Apps usage](https://docs.microsoft.com/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span></span>

## <a name="permissions"></a><span data-ttu-id="a2eb3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2eb3-107">Permissions</span></span>

<span data-ttu-id="a2eb3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2eb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2eb3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2eb3-110">Permission type</span></span>                        | <span data-ttu-id="a2eb3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a2eb3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2eb3-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2eb3-113">Reports.Read.All</span></span>                            |
| <span data-ttu-id="a2eb3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2eb3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-115">Not supported.</span></span>                              |
| <span data-ttu-id="a2eb3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2eb3-116">Application</span></span>                            | <span data-ttu-id="a2eb3-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2eb3-117">Reports.Read.All</span></span>                            |

> <span data-ttu-id="a2eb3-118">**Примечание:** Для делегированных разрешений, позволяющих приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-118">**Note:** For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a2eb3-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a2eb3-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a2eb3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2eb3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getM365AppUserDetail(period='{period_value}')
GET /reports/getM365AppUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="a2eb3-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="a2eb3-121">Function parameters</span></span>

<span data-ttu-id="a2eb3-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a2eb3-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="a2eb3-123">Parameter</span></span> | <span data-ttu-id="a2eb3-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a2eb3-124">Type</span></span>   | <span data-ttu-id="a2eb3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a2eb3-125">Description</span></span>                                                                                                                                                                                                                                             |
| :-------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="a2eb3-126">period</span><span class="sxs-lookup"><span data-stu-id="a2eb3-126">period</span></span>    | <span data-ttu-id="a2eb3-127">string</span><span class="sxs-lookup"><span data-stu-id="a2eb3-127">string</span></span> | <span data-ttu-id="a2eb3-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a2eb3-129">Для {period_value} поддерживаются следующие значения: `D7` , `D30` , `D90` и `D180` .</span><span class="sxs-lookup"><span data-stu-id="a2eb3-129">The supported values for {period_value} are: `D7`, `D30`, `D90`, and `D180`.</span></span> <span data-ttu-id="a2eb3-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a2eb3-131">date</span><span class="sxs-lookup"><span data-stu-id="a2eb3-131">date</span></span>      | <span data-ttu-id="a2eb3-132">Date</span><span class="sxs-lookup"><span data-stu-id="a2eb3-132">Date</span></span>   | <span data-ttu-id="a2eb3-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a2eb3-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a2eb3-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span>          |

> <span data-ttu-id="a2eb3-136">**Примечание:** Необходимо задать один `period` или `date` в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-136">**Note:** You need to set either `period` or `date` in the URL.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="a2eb3-137">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a2eb3-137">Optional query parameters</span></span>

<span data-ttu-id="a2eb3-138">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-138">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a2eb3-139">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-139">The default output type is text/csv.</span></span> <span data-ttu-id="a2eb3-140">Тем не менее, если вы хотите указать тип выходных данных, можно использовать `$format` параметр запроса OData для установки выходных данных по умолчанию в Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-140">However, if you want to specify the output type, you can use the OData `$format` query parameter to set the default output to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2eb3-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2eb3-141">Request headers</span></span>

| <span data-ttu-id="a2eb3-142">Имя</span><span class="sxs-lookup"><span data-stu-id="a2eb3-142">Name</span></span>          | <span data-ttu-id="a2eb3-143">Описание</span><span class="sxs-lookup"><span data-stu-id="a2eb3-143">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a2eb3-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2eb3-144">Authorization</span></span> | <span data-ttu-id="a2eb3-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2eb3-147">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2eb3-147">Request body</span></span>

<span data-ttu-id="a2eb3-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-148">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2eb3-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2eb3-149">Response</span></span>

<span data-ttu-id="a2eb3-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-150">If successful, this method returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) object in the response body.</span></span> <span data-ttu-id="a2eb3-151">Данные отчета хранятся в свойстве **Content** объекта **Report** .</span><span class="sxs-lookup"><span data-stu-id="a2eb3-151">Report data is contained in the **content** property of the **report** object.</span></span>

### <a name="csv"></a><span data-ttu-id="a2eb3-152">CSV</span><span class="sxs-lookup"><span data-stu-id="a2eb3-152">CSV</span></span>

<span data-ttu-id="a2eb3-153">При успешном выполнении запрос свойства **Content** возвращает `302 Found` ответ, который перенаправляет на URL-адрес скачивания, прошедший проверку подлинности для отчета.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-153">If successful, requesting the **content** property returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a2eb3-154">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-154">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a2eb3-155">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-155">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a2eb3-156">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="a2eb3-156">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="a2eb3-157">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="a2eb3-157">Report Refresh Date</span></span>
- <span data-ttu-id="a2eb3-158">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="a2eb3-158">User Principal Name</span></span>
- <span data-ttu-id="a2eb3-159">Дата последней активации</span><span class="sxs-lookup"><span data-stu-id="a2eb3-159">Last Activation Date</span></span>
- <span data-ttu-id="a2eb3-160">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-160">Last Activity Date</span></span>
- <span data-ttu-id="a2eb3-161">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="a2eb3-161">Report Period</span></span>
- <span data-ttu-id="a2eb3-162">Windows</span><span class="sxs-lookup"><span data-stu-id="a2eb3-162">Windows</span></span>
- <span data-ttu-id="a2eb3-163">Mac</span><span class="sxs-lookup"><span data-stu-id="a2eb3-163">Mac</span></span>
- <span data-ttu-id="a2eb3-164">Мобильные устройства</span><span class="sxs-lookup"><span data-stu-id="a2eb3-164">Mobile</span></span>
- <span data-ttu-id="a2eb3-165">Web</span><span class="sxs-lookup"><span data-stu-id="a2eb3-165">Web</span></span>
- <span data-ttu-id="a2eb3-166">Outlook</span><span class="sxs-lookup"><span data-stu-id="a2eb3-166">Outlook</span></span>
- <span data-ttu-id="a2eb3-167">Word</span><span class="sxs-lookup"><span data-stu-id="a2eb3-167">Word</span></span>
- <span data-ttu-id="a2eb3-168">Excel</span><span class="sxs-lookup"><span data-stu-id="a2eb3-168">Excel</span></span>
- <span data-ttu-id="a2eb3-169">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="a2eb3-169">PowerPoint</span></span>
- <span data-ttu-id="a2eb3-170">OneNote</span><span class="sxs-lookup"><span data-stu-id="a2eb3-170">OneNote</span></span>
- <span data-ttu-id="a2eb3-171">Teams</span><span class="sxs-lookup"><span data-stu-id="a2eb3-171">Teams</span></span>
- <span data-ttu-id="a2eb3-172">Outlook (Windows)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-172">Outlook (Windows)</span></span>
- <span data-ttu-id="a2eb3-173">Word (Windows)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-173">Word (Windows)</span></span>
- <span data-ttu-id="a2eb3-174">Excel (Windows)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-174">Excel (Windows)</span></span>
- <span data-ttu-id="a2eb3-175">PowerPoint (Windows)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-175">PowerPoint (Windows)</span></span>
- <span data-ttu-id="a2eb3-176">OneNote (Windows)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-176">OneNote (Windows)</span></span>
- <span data-ttu-id="a2eb3-177">Teams (Windows)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-177">Teams (Windows)</span></span>
- <span data-ttu-id="a2eb3-178">Outlook (Mac)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-178">Outlook (Mac)</span></span>
- <span data-ttu-id="a2eb3-179">Word (Mac)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-179">Word (Mac)</span></span>
- <span data-ttu-id="a2eb3-180">Excel (Mac)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-180">Excel (Mac)</span></span>
- <span data-ttu-id="a2eb3-181">PowerPoint (Mac)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-181">PowerPoint (Mac)</span></span>
- <span data-ttu-id="a2eb3-182">OneNote (Mac)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-182">OneNote (Mac)</span></span>
- <span data-ttu-id="a2eb3-183">Teams (Mac)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-183">Teams (Mac)</span></span>
- <span data-ttu-id="a2eb3-184">Outlook (Mobile)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-184">Outlook (Mobile)</span></span>
- <span data-ttu-id="a2eb3-185">Word (для мобильных устройств)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-185">Word (Mobile)</span></span>
- <span data-ttu-id="a2eb3-186">Excel (Mobile)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-186">Excel (Mobile)</span></span>
- <span data-ttu-id="a2eb3-187">PowerPoint (Mobile)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-187">PowerPoint (Mobile)</span></span>
- <span data-ttu-id="a2eb3-188">OneNote (Mobile)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-188">OneNote (Mobile)</span></span>
- <span data-ttu-id="a2eb3-189">Teams (Mobile)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-189">Teams (Mobile)</span></span>
- <span data-ttu-id="a2eb3-190">Outlook (веб)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-190">Outlook (Web)</span></span>
- <span data-ttu-id="a2eb3-191">Word (веб)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-191">Word (Web)</span></span>
- <span data-ttu-id="a2eb3-192">Excel (веб)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-192">Excel (Web)</span></span>
- <span data-ttu-id="a2eb3-193">PowerPoint (веб)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-193">PowerPoint (Web)</span></span>
- <span data-ttu-id="a2eb3-194">OneNote (Интернет)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-194">OneNote (Web)</span></span>
- <span data-ttu-id="a2eb3-195">Teams (веб)</span><span class="sxs-lookup"><span data-stu-id="a2eb3-195">Teams (Web)</span></span>

### <a name="json"></a><span data-ttu-id="a2eb3-196">JSON</span><span class="sxs-lookup"><span data-stu-id="a2eb3-196">JSON</span></span>

<span data-ttu-id="a2eb3-197">В случае успешного выполнения запрос свойства **Content** возвращает `200 OK` код отклика и объект JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-197">If successful, requesting the **content** property returns a `200 OK` response code and a JSON object in response body.</span></span>

<span data-ttu-id="a2eb3-198">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-198">The default page size for this request is 200 items.</span></span>

## <a name="examples"></a><span data-ttu-id="a2eb3-199">Примеры</span><span class="sxs-lookup"><span data-stu-id="a2eb3-199">Examples</span></span>

### <a name="example-1-csv-output"></a><span data-ttu-id="a2eb3-200">Пример 1: вывод в формате CSV</span><span class="sxs-lookup"><span data-stu-id="a2eb3-200">Example 1: CSV output</span></span>

<span data-ttu-id="a2eb3-201">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-201">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a2eb3-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2eb3-202">Request</span></span>

<span data-ttu-id="a2eb3-203">Ниже приведен пример запроса на получение свойства **содержимого** .</span><span class="sxs-lookup"><span data-stu-id="a2eb3-203">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="a2eb3-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2eb3-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCounDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="a2eb3-205">C#</span><span class="sxs-lookup"><span data-stu-id="a2eb3-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercoundetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2eb3-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2eb3-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercoundetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2eb3-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2eb3-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercoundetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="a2eb3-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2eb3-208">Response</span></span>

<span data-ttu-id="a2eb3-209">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-209">The following is an example of the response.</span></span>

<!-- { "blockType": "response" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a2eb3-210">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-210">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="example-2-json-output"></a><span data-ttu-id="a2eb3-211">Пример 2: выходные данные JSON</span><span class="sxs-lookup"><span data-stu-id="a2eb3-211">Example 2: JSON output</span></span>

<span data-ttu-id="a2eb3-212">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-212">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a2eb3-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2eb3-213">Request</span></span>

<span data-ttu-id="a2eb3-214">Ниже приведен пример запроса на получение свойства **содержимого** .</span><span class="sxs-lookup"><span data-stu-id="a2eb3-214">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="a2eb3-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2eb3-215">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCountDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="a2eb3-216">C#</span><span class="sxs-lookup"><span data-stu-id="a2eb3-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercountdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2eb3-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2eb3-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercountdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2eb3-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2eb3-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercountdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="a2eb3-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2eb3-219">Response</span></span>

<span data-ttu-id="a2eb3-220">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-220">The following is an example of the response.</span></span>

> <span data-ttu-id="a2eb3-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2eb3-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
