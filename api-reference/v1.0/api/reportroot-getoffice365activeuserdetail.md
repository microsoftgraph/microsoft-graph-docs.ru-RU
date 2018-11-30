---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Получение сведений об активных пользователях Office 365.
ms.openlocfilehash: d14ef5dfab0bde7264fbaa6f82007bdfa2300da8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027319"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="31ba6-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="31ba6-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="31ba6-104">Получение сведений об активных пользователях Office 365.</span><span class="sxs-lookup"><span data-stu-id="31ba6-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="31ba6-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="31ba6-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="31ba6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31ba6-106">Permissions</span></span>

<span data-ttu-id="31ba6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31ba6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31ba6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31ba6-109">Permission type</span></span>                        | <span data-ttu-id="31ba6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31ba6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="31ba6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31ba6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="31ba6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="31ba6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="31ba6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31ba6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31ba6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31ba6-114">Not supported.</span></span>                           |
| <span data-ttu-id="31ba6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31ba6-115">Application</span></span>                            | <span data-ttu-id="31ba6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="31ba6-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="31ba6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31ba6-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="31ba6-118">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="31ba6-118">Function parameters</span></span>

<span data-ttu-id="31ba6-119">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="31ba6-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="31ba6-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="31ba6-120">Parameter</span></span> | <span data-ttu-id="31ba6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="31ba6-121">Type</span></span>   | <span data-ttu-id="31ba6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="31ba6-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="31ba6-123">period</span><span class="sxs-lookup"><span data-stu-id="31ba6-123">period</span></span>    | <span data-ttu-id="31ba6-124">строка</span><span class="sxs-lookup"><span data-stu-id="31ba6-124">string</span></span> | <span data-ttu-id="31ba6-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="31ba6-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="31ba6-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="31ba6-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="31ba6-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="31ba6-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="31ba6-128">date</span><span class="sxs-lookup"><span data-stu-id="31ba6-128">date</span></span>      | <span data-ttu-id="31ba6-129">Date</span><span class="sxs-lookup"><span data-stu-id="31ba6-129">Date</span></span>   | <span data-ttu-id="31ba6-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="31ba6-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="31ba6-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="31ba6-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="31ba6-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="31ba6-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="31ba6-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="31ba6-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31ba6-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31ba6-134">Request headers</span></span>

| <span data-ttu-id="31ba6-135">Имя</span><span class="sxs-lookup"><span data-stu-id="31ba6-135">Name</span></span>          | <span data-ttu-id="31ba6-136">Описание</span><span class="sxs-lookup"><span data-stu-id="31ba6-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="31ba6-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31ba6-137">Authorization</span></span> | <span data-ttu-id="31ba6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31ba6-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="31ba6-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="31ba6-140">If-None-Match</span></span> | <span data-ttu-id="31ba6-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="31ba6-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="31ba6-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="31ba6-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="31ba6-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="31ba6-143">Response</span></span>

<span data-ttu-id="31ba6-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="31ba6-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="31ba6-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="31ba6-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="31ba6-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="31ba6-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="31ba6-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="31ba6-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="31ba6-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="31ba6-148">Report Refresh Date</span></span>
- <span data-ttu-id="31ba6-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="31ba6-149">User Principal Name</span></span>
- <span data-ttu-id="31ba6-150">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="31ba6-150">Display Name</span></span>
- <span data-ttu-id="31ba6-151">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="31ba6-151">Is Deleted</span></span>
- <span data-ttu-id="31ba6-152">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="31ba6-152">Deleted Date</span></span>
- <span data-ttu-id="31ba6-153">"Has Exchange License" (Есть лицензия на Exchange);</span><span class="sxs-lookup"><span data-stu-id="31ba6-153">Has Exchange License</span></span>
- <span data-ttu-id="31ba6-154">"Has OneDrive License" (Есть лицензия на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="31ba6-154">Has OneDrive License</span></span>
- <span data-ttu-id="31ba6-155">"Has SharePoint License" (Есть лицензия на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="31ba6-155">Has SharePoint License</span></span>
- <span data-ttu-id="31ba6-156">"Has Skype For Business License" (Есть лицензия на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="31ba6-156">Has Skype For Business License</span></span>
- <span data-ttu-id="31ba6-157">"Has Yammer License" (Есть лицензия на Yammer);</span><span class="sxs-lookup"><span data-stu-id="31ba6-157">Has Yammer License</span></span>
- <span data-ttu-id="31ba6-158">"Has Teams License" (Есть лицензия на Teams);</span><span class="sxs-lookup"><span data-stu-id="31ba6-158">Has Teams License</span></span>
- <span data-ttu-id="31ba6-159">"Exchange Last Activity Date" (Дата последнего действия в Exchange);</span><span class="sxs-lookup"><span data-stu-id="31ba6-159">Exchange Last Activity Date</span></span>
- <span data-ttu-id="31ba6-160">"OneDrive Last Activity Date" (Дата последнего действия в OneDrive);</span><span class="sxs-lookup"><span data-stu-id="31ba6-160">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="31ba6-161">"SharePoint Last Activity Date" (Дата последнего действия в SharePoint);</span><span class="sxs-lookup"><span data-stu-id="31ba6-161">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="31ba6-162">"Skype For Business Last Activity Date" (Дата последнего действия в Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="31ba6-162">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="31ba6-163">"Yammer Last Activity Date" (Дата последнего действия в Yammer);</span><span class="sxs-lookup"><span data-stu-id="31ba6-163">Yammer Last Activity Date</span></span>
- <span data-ttu-id="31ba6-164">"Teams Last Activity Date" (Дата последнего действия в Teams);</span><span class="sxs-lookup"><span data-stu-id="31ba6-164">Teams Last Activity Date</span></span>
- <span data-ttu-id="31ba6-165">"Exchange License Assign Date" (Дата назначения лицензии на Exchange);</span><span class="sxs-lookup"><span data-stu-id="31ba6-165">Exchange License Assign Date</span></span>
- <span data-ttu-id="31ba6-166">"OneDrive License Assign Date" (Дата назначения лицензии на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="31ba6-166">OneDrive License Assign Date</span></span>
- <span data-ttu-id="31ba6-167">"SharePoint License Assign Date" (Дата назначения лицензии на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="31ba6-167">SharePoint License Assign Date</span></span>
- <span data-ttu-id="31ba6-168">"Skype For Business License Assign Date" (Дата назначения лицензии на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="31ba6-168">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="31ba6-169">"Yammer License Assign Date" (Дата назначения лицензии на Yammer);</span><span class="sxs-lookup"><span data-stu-id="31ba6-169">Yammer License Assign Date</span></span>
- <span data-ttu-id="31ba6-170">"Teams License Assign Date" (Дата назначения лицензии на Teams);</span><span class="sxs-lookup"><span data-stu-id="31ba6-170">Teams License Assign Date</span></span>
- <span data-ttu-id="31ba6-171">"Assigned Products" (Назначенные продукты).</span><span class="sxs-lookup"><span data-stu-id="31ba6-171">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="31ba6-172">Пример</span><span class="sxs-lookup"><span data-stu-id="31ba6-172">Example</span></span>

#### <a name="request"></a><span data-ttu-id="31ba6-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="31ba6-173">Request</span></span>

<span data-ttu-id="31ba6-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31ba6-174">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="31ba6-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="31ba6-175">Response</span></span>

<span data-ttu-id="31ba6-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="31ba6-176">The following is an example of the response.</span></span>

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

<span data-ttu-id="31ba6-177">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="31ba6-177">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
```
