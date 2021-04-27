---
title: 'reportRoot: getM365AppUserDetail'
description: Получите отчет, который содержит сведения о том, какие приложения и платформы использовали пользователи.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 196e8747254d2fdc1cdb0e97a53eb2fe8c6b78d1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050936"
---
# <a name="reportroot-getm365appuserdetail"></a><span data-ttu-id="2bda0-103">reportRoot: getM365AppUserDetail</span><span class="sxs-lookup"><span data-stu-id="2bda0-103">reportRoot: getM365AppUserDetail</span></span>

<span data-ttu-id="2bda0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bda0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bda0-105">Получите отчет, который содержит сведения о том, какие приложения и платформы использовали пользователи.</span><span class="sxs-lookup"><span data-stu-id="2bda0-105">Get a report that provides the details about which apps and platforms users have used.</span></span>

> <span data-ttu-id="2bda0-106">**Примечание:** Сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов - Приложения Microsoft 365 использования.](/microsoft-365/admin/activity-reports/microsoft365-apps-usage)</span><span class="sxs-lookup"><span data-stu-id="2bda0-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 Apps usage](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span></span>

## <a name="permissions"></a><span data-ttu-id="2bda0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2bda0-107">Permissions</span></span>

<span data-ttu-id="2bda0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bda0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2bda0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bda0-110">Permission type</span></span>                        | <span data-ttu-id="2bda0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bda0-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2bda0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bda0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2bda0-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bda0-113">Reports.Read.All</span></span>                            |
| <span data-ttu-id="2bda0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bda0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bda0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bda0-115">Not supported.</span></span>                              |
| <span data-ttu-id="2bda0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2bda0-116">Application</span></span>                            | <span data-ttu-id="2bda0-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bda0-117">Reports.Read.All</span></span>                            |

> <span data-ttu-id="2bda0-118">**Примечание:** Для делегирования разрешений, позволяющих приложениям читать отчеты об использовании служб от имени пользователя, администратор клиента должен присвоить пользователю соответствующую роль администратора Azure AD с ограниченной ответственностью.</span><span class="sxs-lookup"><span data-stu-id="2bda0-118">**Note:** For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="2bda0-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="2bda0-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="2bda0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bda0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getM365AppUserDetail(period='{period_value}')
GET /reports/getM365AppUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="2bda0-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="2bda0-121">Function parameters</span></span>

<span data-ttu-id="2bda0-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="2bda0-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2bda0-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="2bda0-123">Parameter</span></span> | <span data-ttu-id="2bda0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="2bda0-124">Type</span></span>   | <span data-ttu-id="2bda0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="2bda0-125">Description</span></span>                                                                                                                                                                                                                                             |
| :-------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="2bda0-126">period</span><span class="sxs-lookup"><span data-stu-id="2bda0-126">period</span></span>    | <span data-ttu-id="2bda0-127">string</span><span class="sxs-lookup"><span data-stu-id="2bda0-127">string</span></span> | <span data-ttu-id="2bda0-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="2bda0-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2bda0-129">Поддерживаемые значения {period_value} : `D7` , `D30` , и `D90` `D180` .</span><span class="sxs-lookup"><span data-stu-id="2bda0-129">The supported values for {period_value} are: `D7`, `D30`, `D90`, and `D180`.</span></span> <span data-ttu-id="2bda0-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="2bda0-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="2bda0-131">date</span><span class="sxs-lookup"><span data-stu-id="2bda0-131">date</span></span>      | <span data-ttu-id="2bda0-132">Date</span><span class="sxs-lookup"><span data-stu-id="2bda0-132">Date</span></span>   | <span data-ttu-id="2bda0-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="2bda0-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="2bda0-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="2bda0-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="2bda0-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="2bda0-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span>          |

> <span data-ttu-id="2bda0-136">**Примечание:** Необходимо установить либо `period` `date` URL-адрес, либо его url-адрес.</span><span class="sxs-lookup"><span data-stu-id="2bda0-136">**Note:** You need to set either `period` or `date` in the URL.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2bda0-137">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2bda0-137">Optional query parameters</span></span>

<span data-ttu-id="2bda0-138">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2bda0-138">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2bda0-139">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="2bda0-139">The default output type is text/csv.</span></span> <span data-ttu-id="2bda0-140">Однако если требуется указать тип вывода, можно использовать параметр запроса OData, чтобы задать выход по умолчанию `$format` тексту/csv или приложению/json.</span><span class="sxs-lookup"><span data-stu-id="2bda0-140">However, if you want to specify the output type, you can use the OData `$format` query parameter to set the default output to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bda0-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2bda0-141">Request headers</span></span>

| <span data-ttu-id="2bda0-142">Имя</span><span class="sxs-lookup"><span data-stu-id="2bda0-142">Name</span></span>          | <span data-ttu-id="2bda0-143">Описание</span><span class="sxs-lookup"><span data-stu-id="2bda0-143">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2bda0-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2bda0-144">Authorization</span></span> | <span data-ttu-id="2bda0-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2bda0-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2bda0-147">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2bda0-147">Request body</span></span>

<span data-ttu-id="2bda0-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2bda0-148">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bda0-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bda0-149">Response</span></span>

<span data-ttu-id="2bda0-150">В случае успешной работы этот метод возвращает код `200 OK` отклика и объект [отчета](../resources/intune-shared-report.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2bda0-150">If successful, this method returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) object in the response body.</span></span> <span data-ttu-id="2bda0-151">Данные отчета содержатся в **свойстве** контента объекта **отчета.**</span><span class="sxs-lookup"><span data-stu-id="2bda0-151">Report data is contained in the **content** property of the **report** object.</span></span>

### <a name="csv"></a><span data-ttu-id="2bda0-152">CSV</span><span class="sxs-lookup"><span data-stu-id="2bda0-152">CSV</span></span>

<span data-ttu-id="2bda0-153">В случае успешного  запроса свойства контента возвращается ответ, который перенаправляется на предварительно заранее задаваемые URL-адрес `302 Found` загрузки отчета.</span><span class="sxs-lookup"><span data-stu-id="2bda0-153">If successful, requesting the **content** property returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2bda0-154">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="2bda0-154">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2bda0-155">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2bda0-155">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2bda0-156">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="2bda0-156">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="2bda0-157">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="2bda0-157">Report Refresh Date</span></span>
- <span data-ttu-id="2bda0-158">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="2bda0-158">User Principal Name</span></span>
- <span data-ttu-id="2bda0-159">Дата последней активации</span><span class="sxs-lookup"><span data-stu-id="2bda0-159">Last Activation Date</span></span>
- <span data-ttu-id="2bda0-160">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="2bda0-160">Last Activity Date</span></span>
- <span data-ttu-id="2bda0-161">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="2bda0-161">Report Period</span></span>
- <span data-ttu-id="2bda0-162">Windows</span><span class="sxs-lookup"><span data-stu-id="2bda0-162">Windows</span></span>
- <span data-ttu-id="2bda0-163">Mac</span><span class="sxs-lookup"><span data-stu-id="2bda0-163">Mac</span></span>
- <span data-ttu-id="2bda0-164">Для мобильных устройств</span><span class="sxs-lookup"><span data-stu-id="2bda0-164">Mobile</span></span>
- <span data-ttu-id="2bda0-165">Web</span><span class="sxs-lookup"><span data-stu-id="2bda0-165">Web</span></span>
- <span data-ttu-id="2bda0-166">Outlook</span><span class="sxs-lookup"><span data-stu-id="2bda0-166">Outlook</span></span>
- <span data-ttu-id="2bda0-167">Word</span><span class="sxs-lookup"><span data-stu-id="2bda0-167">Word</span></span>
- <span data-ttu-id="2bda0-168">Excel</span><span class="sxs-lookup"><span data-stu-id="2bda0-168">Excel</span></span>
- <span data-ttu-id="2bda0-169">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="2bda0-169">PowerPoint</span></span>
- <span data-ttu-id="2bda0-170">OneNote</span><span class="sxs-lookup"><span data-stu-id="2bda0-170">OneNote</span></span>
- <span data-ttu-id="2bda0-171">Teams</span><span class="sxs-lookup"><span data-stu-id="2bda0-171">Teams</span></span>
- <span data-ttu-id="2bda0-172">Outlook (Windows)</span><span class="sxs-lookup"><span data-stu-id="2bda0-172">Outlook (Windows)</span></span>
- <span data-ttu-id="2bda0-173">Word (Windows)</span><span class="sxs-lookup"><span data-stu-id="2bda0-173">Word (Windows)</span></span>
- <span data-ttu-id="2bda0-174">Excel (Windows)</span><span class="sxs-lookup"><span data-stu-id="2bda0-174">Excel (Windows)</span></span>
- <span data-ttu-id="2bda0-175">PowerPoint (Windows)</span><span class="sxs-lookup"><span data-stu-id="2bda0-175">PowerPoint (Windows)</span></span>
- <span data-ttu-id="2bda0-176">OneNote (Windows)</span><span class="sxs-lookup"><span data-stu-id="2bda0-176">OneNote (Windows)</span></span>
- <span data-ttu-id="2bda0-177">Teams (Windows)</span><span class="sxs-lookup"><span data-stu-id="2bda0-177">Teams (Windows)</span></span>
- <span data-ttu-id="2bda0-178">Outlook (Mac)</span><span class="sxs-lookup"><span data-stu-id="2bda0-178">Outlook (Mac)</span></span>
- <span data-ttu-id="2bda0-179">Word (Mac)</span><span class="sxs-lookup"><span data-stu-id="2bda0-179">Word (Mac)</span></span>
- <span data-ttu-id="2bda0-180">Excel (Mac)</span><span class="sxs-lookup"><span data-stu-id="2bda0-180">Excel (Mac)</span></span>
- <span data-ttu-id="2bda0-181">PowerPoint (Mac)</span><span class="sxs-lookup"><span data-stu-id="2bda0-181">PowerPoint (Mac)</span></span>
- <span data-ttu-id="2bda0-182">OneNote (Mac)</span><span class="sxs-lookup"><span data-stu-id="2bda0-182">OneNote (Mac)</span></span>
- <span data-ttu-id="2bda0-183">Teams (Mac)</span><span class="sxs-lookup"><span data-stu-id="2bda0-183">Teams (Mac)</span></span>
- <span data-ttu-id="2bda0-184">Outlook (Мобильный)</span><span class="sxs-lookup"><span data-stu-id="2bda0-184">Outlook (Mobile)</span></span>
- <span data-ttu-id="2bda0-185">Word (Mobile)</span><span class="sxs-lookup"><span data-stu-id="2bda0-185">Word (Mobile)</span></span>
- <span data-ttu-id="2bda0-186">Excel (Мобильный)</span><span class="sxs-lookup"><span data-stu-id="2bda0-186">Excel (Mobile)</span></span>
- <span data-ttu-id="2bda0-187">PowerPoint (Мобильный)</span><span class="sxs-lookup"><span data-stu-id="2bda0-187">PowerPoint (Mobile)</span></span>
- <span data-ttu-id="2bda0-188">OneNote (Мобильный)</span><span class="sxs-lookup"><span data-stu-id="2bda0-188">OneNote (Mobile)</span></span>
- <span data-ttu-id="2bda0-189">Teams (Мобильный)</span><span class="sxs-lookup"><span data-stu-id="2bda0-189">Teams (Mobile)</span></span>
- <span data-ttu-id="2bda0-190">Outlook (Веб)</span><span class="sxs-lookup"><span data-stu-id="2bda0-190">Outlook (Web)</span></span>
- <span data-ttu-id="2bda0-191">Word (Web)</span><span class="sxs-lookup"><span data-stu-id="2bda0-191">Word (Web)</span></span>
- <span data-ttu-id="2bda0-192">Excel (Веб)</span><span class="sxs-lookup"><span data-stu-id="2bda0-192">Excel (Web)</span></span>
- <span data-ttu-id="2bda0-193">PowerPoint (Веб)</span><span class="sxs-lookup"><span data-stu-id="2bda0-193">PowerPoint (Web)</span></span>
- <span data-ttu-id="2bda0-194">OneNote (Веб)</span><span class="sxs-lookup"><span data-stu-id="2bda0-194">OneNote (Web)</span></span>
- <span data-ttu-id="2bda0-195">Teams (Web)</span><span class="sxs-lookup"><span data-stu-id="2bda0-195">Teams (Web)</span></span>

### <a name="json"></a><span data-ttu-id="2bda0-196">JSON</span><span class="sxs-lookup"><span data-stu-id="2bda0-196">JSON</span></span>

<span data-ttu-id="2bda0-197">В случае успешной работы запрос свойства **контента** возвращает код отклика `200 OK` и объект JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2bda0-197">If successful, requesting the **content** property returns a `200 OK` response code and a JSON object in response body.</span></span>

<span data-ttu-id="2bda0-198">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="2bda0-198">The default page size for this request is 200 items.</span></span>

## <a name="examples"></a><span data-ttu-id="2bda0-199">Примеры</span><span class="sxs-lookup"><span data-stu-id="2bda0-199">Examples</span></span>

### <a name="example-1-csv-output"></a><span data-ttu-id="2bda0-200">Пример 1. Выход CSV</span><span class="sxs-lookup"><span data-stu-id="2bda0-200">Example 1: CSV output</span></span>

<span data-ttu-id="2bda0-201">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="2bda0-201">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2bda0-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bda0-202">Request</span></span>

<span data-ttu-id="2bda0-203">Ниже приводится пример запроса на получения **свойства** контента.</span><span class="sxs-lookup"><span data-stu-id="2bda0-203">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="2bda0-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="2bda0-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCounDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="2bda0-205">C#</span><span class="sxs-lookup"><span data-stu-id="2bda0-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercoundetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2bda0-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2bda0-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercoundetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2bda0-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2bda0-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercoundetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2bda0-208">Java</span><span class="sxs-lookup"><span data-stu-id="2bda0-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercoundetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="2bda0-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bda0-209">Response</span></span>

<span data-ttu-id="2bda0-210">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2bda0-210">The following is an example of the response.</span></span>

<!-- { "blockType": "response" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2bda0-211">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="2bda0-211">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="example-2-json-output"></a><span data-ttu-id="2bda0-212">Пример 2. Вывод JSON</span><span class="sxs-lookup"><span data-stu-id="2bda0-212">Example 2: JSON output</span></span>

<span data-ttu-id="2bda0-213">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="2bda0-213">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2bda0-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bda0-214">Request</span></span>

<span data-ttu-id="2bda0-215">Ниже приводится пример запроса на получения **свойства** контента.</span><span class="sxs-lookup"><span data-stu-id="2bda0-215">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="2bda0-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="2bda0-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCountDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="2bda0-217">C#</span><span class="sxs-lookup"><span data-stu-id="2bda0-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercountdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2bda0-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2bda0-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercountdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2bda0-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2bda0-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercountdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2bda0-220">Java</span><span class="sxs-lookup"><span data-stu-id="2bda0-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercountdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="2bda0-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bda0-221">Response</span></span>

<span data-ttu-id="2bda0-222">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2bda0-222">The following is an example of the response.</span></span>

> <span data-ttu-id="2bda0-223">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2bda0-223">**Note:** The response object shown here might be shortened for readability.</span></span>

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
