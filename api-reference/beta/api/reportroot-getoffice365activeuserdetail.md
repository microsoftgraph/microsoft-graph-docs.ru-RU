---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Получение сведений об активных пользователях Office 365.
ms.openlocfilehash: 340428bba0bbba8c333cde98e7ad38f28186e662
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076433"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="de7f1-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="de7f1-103">reportRoot: getOffice365ActiveUserDetail</span></span>

> <span data-ttu-id="de7f1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="de7f1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de7f1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de7f1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de7f1-106">Получение сведений об активных пользователях Office 365.</span><span class="sxs-lookup"><span data-stu-id="de7f1-106">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="de7f1-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="de7f1-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="de7f1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de7f1-108">Permissions</span></span>

<span data-ttu-id="de7f1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de7f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de7f1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de7f1-111">Permission type</span></span>                        | <span data-ttu-id="de7f1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de7f1-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="de7f1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de7f1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="de7f1-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="de7f1-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="de7f1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de7f1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de7f1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de7f1-116">Not supported.</span></span>                           |
| <span data-ttu-id="de7f1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de7f1-117">Application</span></span>                            | <span data-ttu-id="de7f1-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="de7f1-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="de7f1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de7f1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="de7f1-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="de7f1-120">Function parameters</span></span>

<span data-ttu-id="de7f1-121">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="de7f1-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="de7f1-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="de7f1-122">Parameter</span></span> | <span data-ttu-id="de7f1-123">Тип</span><span class="sxs-lookup"><span data-stu-id="de7f1-123">Type</span></span>   | <span data-ttu-id="de7f1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="de7f1-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="de7f1-125">period</span><span class="sxs-lookup"><span data-stu-id="de7f1-125">period</span></span>    | <span data-ttu-id="de7f1-126">строка</span><span class="sxs-lookup"><span data-stu-id="de7f1-126">string</span></span> | <span data-ttu-id="de7f1-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="de7f1-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="de7f1-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="de7f1-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="de7f1-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="de7f1-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="de7f1-130">date</span><span class="sxs-lookup"><span data-stu-id="de7f1-130">date</span></span>      | <span data-ttu-id="de7f1-131">Date</span><span class="sxs-lookup"><span data-stu-id="de7f1-131">Date</span></span>   | <span data-ttu-id="de7f1-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="de7f1-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="de7f1-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="de7f1-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="de7f1-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="de7f1-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="de7f1-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="de7f1-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="de7f1-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="de7f1-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="de7f1-137">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="de7f1-137">The default output type is text/csv.</span></span> <span data-ttu-id="de7f1-138">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="de7f1-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de7f1-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de7f1-139">Request headers</span></span>

| <span data-ttu-id="de7f1-140">Имя</span><span class="sxs-lookup"><span data-stu-id="de7f1-140">Name</span></span>          | <span data-ttu-id="de7f1-141">Описание</span><span class="sxs-lookup"><span data-stu-id="de7f1-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="de7f1-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de7f1-142">Authorization</span></span> | <span data-ttu-id="de7f1-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de7f1-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="de7f1-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="de7f1-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="de7f1-146">CSV</span><span class="sxs-lookup"><span data-stu-id="de7f1-146">CSV</span></span>

<span data-ttu-id="de7f1-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="de7f1-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="de7f1-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="de7f1-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="de7f1-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="de7f1-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="de7f1-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="de7f1-150">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="de7f1-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="de7f1-151">Report Refresh Date</span></span>
- <span data-ttu-id="de7f1-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="de7f1-152">User Principal Name</span></span>
- <span data-ttu-id="de7f1-153">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="de7f1-153">Display Name</span></span>
- <span data-ttu-id="de7f1-154">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="de7f1-154">Is Deleted</span></span>
- <span data-ttu-id="de7f1-155">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="de7f1-155">Deleted Date</span></span>
- <span data-ttu-id="de7f1-156">"Has Exchange License" (Есть лицензия на Exchange);</span><span class="sxs-lookup"><span data-stu-id="de7f1-156">Has Exchange License</span></span>
- <span data-ttu-id="de7f1-157">"Has OneDrive License" (Есть лицензия на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="de7f1-157">Has OneDrive License</span></span>
- <span data-ttu-id="de7f1-158">"Has SharePoint License" (Есть лицензия на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="de7f1-158">Has SharePoint License</span></span>
- <span data-ttu-id="de7f1-159">"Has Skype For Business License" (Есть лицензия на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="de7f1-159">Has Skype For Business License</span></span>
- <span data-ttu-id="de7f1-160">"Has Yammer License" (Есть лицензия на Yammer);</span><span class="sxs-lookup"><span data-stu-id="de7f1-160">Has Yammer License</span></span>
- <span data-ttu-id="de7f1-161">"Has Teams License" (Есть лицензия на Teams);</span><span class="sxs-lookup"><span data-stu-id="de7f1-161">Has Teams License</span></span>
- <span data-ttu-id="de7f1-162">"Exchange Last Activity Date" (Дата последнего действия в Exchange);</span><span class="sxs-lookup"><span data-stu-id="de7f1-162">Exchange Last Activity Date</span></span>
- <span data-ttu-id="de7f1-163">"OneDrive Last Activity Date" (Дата последнего действия в OneDrive);</span><span class="sxs-lookup"><span data-stu-id="de7f1-163">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="de7f1-164">"SharePoint Last Activity Date" (Дата последнего действия в SharePoint);</span><span class="sxs-lookup"><span data-stu-id="de7f1-164">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="de7f1-165">"Skype For Business Last Activity Date" (Дата последнего действия в Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="de7f1-165">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="de7f1-166">"Yammer Last Activity Date" (Дата последнего действия в Yammer);</span><span class="sxs-lookup"><span data-stu-id="de7f1-166">Yammer Last Activity Date</span></span>
- <span data-ttu-id="de7f1-167">"Teams Last Activity Date" (Дата последнего действия в Teams);</span><span class="sxs-lookup"><span data-stu-id="de7f1-167">Teams Last Activity Date</span></span>
- <span data-ttu-id="de7f1-168">"Exchange License Assign Date" (Дата назначения лицензии на Exchange);</span><span class="sxs-lookup"><span data-stu-id="de7f1-168">Exchange License Assign Date</span></span>
- <span data-ttu-id="de7f1-169">"OneDrive License Assign Date" (Дата назначения лицензии на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="de7f1-169">OneDrive License Assign Date</span></span>
- <span data-ttu-id="de7f1-170">"SharePoint License Assign Date" (Дата назначения лицензии на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="de7f1-170">SharePoint License Assign Date</span></span>
- <span data-ttu-id="de7f1-171">"Skype For Business License Assign Date" (Дата назначения лицензии на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="de7f1-171">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="de7f1-172">"Yammer License Assign Date" (Дата назначения лицензии на Yammer);</span><span class="sxs-lookup"><span data-stu-id="de7f1-172">Yammer License Assign Date</span></span>
- <span data-ttu-id="de7f1-173">"Teams License Assign Date" (Дата назначения лицензии на Teams);</span><span class="sxs-lookup"><span data-stu-id="de7f1-173">Teams License Assign Date</span></span>
- <span data-ttu-id="de7f1-174">"Assigned Products" (Назначенные продукты).</span><span class="sxs-lookup"><span data-stu-id="de7f1-174">Assigned Products</span></span>

<span data-ttu-id="de7f1-175">В Китае Microsoft Graph обслуживается 21Vianet не поддерживаются следующие столбцы:</span><span class="sxs-lookup"><span data-stu-id="de7f1-175">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="de7f1-176">"Has Yammer License" (Есть лицензия на Yammer);</span><span class="sxs-lookup"><span data-stu-id="de7f1-176">Has Yammer License</span></span>
- <span data-ttu-id="de7f1-177">"Has Teams License" (Есть лицензия на Teams);</span><span class="sxs-lookup"><span data-stu-id="de7f1-177">Has Teams License</span></span>
- <span data-ttu-id="de7f1-178">"Yammer Last Activity Date" (Дата последнего действия в Yammer);</span><span class="sxs-lookup"><span data-stu-id="de7f1-178">Yammer Last Activity Date</span></span>
- <span data-ttu-id="de7f1-179">"Teams Last Activity Date" (Дата последнего действия в Teams);</span><span class="sxs-lookup"><span data-stu-id="de7f1-179">Teams Last Activity Date</span></span>
- <span data-ttu-id="de7f1-180">"Yammer License Assign Date" (Дата назначения лицензии на Yammer);</span><span class="sxs-lookup"><span data-stu-id="de7f1-180">Yammer License Assign Date</span></span>
- <span data-ttu-id="de7f1-181">"Teams License Assign Date" (Дата назначения лицензии на Teams);</span><span class="sxs-lookup"><span data-stu-id="de7f1-181">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="de7f1-182">JSON</span><span class="sxs-lookup"><span data-stu-id="de7f1-182">JSON</span></span>

<span data-ttu-id="de7f1-183">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="de7f1-183">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="de7f1-184">Следующие свойства объекта **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** не поддерживаются в Китае Microsoft Graph обслуживается 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="de7f1-184">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="de7f1-185">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="de7f1-185">hasYammerLicense</span></span>
- <span data-ttu-id="de7f1-186">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="de7f1-186">hasTeamsLicense</span></span>
- <span data-ttu-id="de7f1-187">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="de7f1-187">yammerLastActivityDate</span></span>
- <span data-ttu-id="de7f1-188">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="de7f1-188">teamsLastActivityDate</span></span>
- <span data-ttu-id="de7f1-189">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="de7f1-189">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="de7f1-190">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="de7f1-190">teamsLicenseAssignDate</span></span>

<span data-ttu-id="de7f1-191">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="de7f1-191">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="de7f1-192">Пример</span><span class="sxs-lookup"><span data-stu-id="de7f1-192">Example</span></span>

### <a name="csv"></a><span data-ttu-id="de7f1-193">CSV</span><span class="sxs-lookup"><span data-stu-id="de7f1-193">CSV</span></span>

<span data-ttu-id="de7f1-194">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="de7f1-194">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="de7f1-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="de7f1-195">Request</span></span>

<span data-ttu-id="de7f1-196">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de7f1-196">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="de7f1-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="de7f1-197">Response</span></span>

<span data-ttu-id="de7f1-198">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="de7f1-198">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="de7f1-199">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="de7f1-199">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="de7f1-200">JSON</span><span class="sxs-lookup"><span data-stu-id="de7f1-200">JSON</span></span>

<span data-ttu-id="de7f1-201">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="de7f1-201">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="de7f1-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="de7f1-202">Request</span></span>

<span data-ttu-id="de7f1-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de7f1-203">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="de7f1-204">Ответ</span><span class="sxs-lookup"><span data-stu-id="de7f1-204">Response</span></span>

<span data-ttu-id="de7f1-205">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de7f1-205">The following is an example of the response.</span></span>

> <span data-ttu-id="de7f1-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de7f1-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
