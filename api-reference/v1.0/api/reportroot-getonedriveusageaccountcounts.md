---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса. Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e25fc9d099b8eabd866725b7b3a41796f2a4a615
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591399"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="b39bd-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="b39bd-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="b39bd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b39bd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b39bd-106">Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b39bd-106">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="b39bd-107">Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.</span><span class="sxs-lookup"><span data-stu-id="b39bd-107">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="b39bd-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="b39bd-108">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="b39bd-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b39bd-109">Permissions</span></span>

<span data-ttu-id="b39bd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b39bd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b39bd-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b39bd-112">Permission type</span></span>                        | <span data-ttu-id="b39bd-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b39bd-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b39bd-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b39bd-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="b39bd-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b39bd-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b39bd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b39bd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b39bd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b39bd-117">Not supported.</span></span>                           |
| <span data-ttu-id="b39bd-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b39bd-118">Application</span></span>                            | <span data-ttu-id="b39bd-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b39bd-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="b39bd-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b39bd-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="b39bd-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="b39bd-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="b39bd-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b39bd-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b39bd-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b39bd-123">Function parameters</span></span>

<span data-ttu-id="b39bd-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="b39bd-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b39bd-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="b39bd-125">Parameter</span></span> | <span data-ttu-id="b39bd-126">Тип</span><span class="sxs-lookup"><span data-stu-id="b39bd-126">Type</span></span>   | <span data-ttu-id="b39bd-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b39bd-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b39bd-128">period</span><span class="sxs-lookup"><span data-stu-id="b39bd-128">period</span></span>    | <span data-ttu-id="b39bd-129">string</span><span class="sxs-lookup"><span data-stu-id="b39bd-129">string</span></span> | <span data-ttu-id="b39bd-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="b39bd-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b39bd-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="b39bd-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b39bd-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="b39bd-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b39bd-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b39bd-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b39bd-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b39bd-134">Request headers</span></span>

| <span data-ttu-id="b39bd-135">Имя</span><span class="sxs-lookup"><span data-stu-id="b39bd-135">Name</span></span>          | <span data-ttu-id="b39bd-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b39bd-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b39bd-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b39bd-137">Authorization</span></span> | <span data-ttu-id="b39bd-p106">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b39bd-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b39bd-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b39bd-140">If-None-Match</span></span> | <span data-ttu-id="b39bd-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="b39bd-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b39bd-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b39bd-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b39bd-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b39bd-143">Response</span></span>

<span data-ttu-id="b39bd-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b39bd-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b39bd-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b39bd-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b39bd-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b39bd-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b39bd-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="b39bd-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b39bd-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="b39bd-148">Report Refresh Date</span></span>
- <span data-ttu-id="b39bd-149">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="b39bd-149">Site Type</span></span>
- <span data-ttu-id="b39bd-150">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="b39bd-150">Total</span></span>
- <span data-ttu-id="b39bd-151">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="b39bd-151">Active</span></span>
- <span data-ttu-id="b39bd-152">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="b39bd-152">Report Date</span></span>
- <span data-ttu-id="b39bd-153">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="b39bd-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b39bd-154">Пример</span><span class="sxs-lookup"><span data-stu-id="b39bd-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b39bd-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="b39bd-155">Request</span></span>

<span data-ttu-id="b39bd-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b39bd-156">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getonedriveusageaccountcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="b39bd-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="b39bd-157">Response</span></span>

<span data-ttu-id="b39bd-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b39bd-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="b39bd-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b39bd-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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
