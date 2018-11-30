---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Получение сведения о действиях отдельных пользователей Microsoft Teams.
ms.openlocfilehash: 6905f9a18627a9ebf3c63ca92c111d1518564a3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026378"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="c6d08-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="c6d08-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="c6d08-104">Получение сведения о действиях отдельных пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c6d08-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6d08-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6d08-105">Permissions</span></span>

<span data-ttu-id="c6d08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6d08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6d08-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6d08-108">Permission type</span></span>                        | <span data-ttu-id="c6d08-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6d08-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c6d08-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6d08-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6d08-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6d08-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c6d08-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6d08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6d08-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6d08-113">Not supported.</span></span>                           |
| <span data-ttu-id="c6d08-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6d08-114">Application</span></span>                            | <span data-ttu-id="c6d08-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6d08-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c6d08-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6d08-116">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="c6d08-117">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="c6d08-117">Function parameters</span></span>

<span data-ttu-id="c6d08-118">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c6d08-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c6d08-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="c6d08-119">Parameter</span></span> | <span data-ttu-id="c6d08-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c6d08-120">Type</span></span>   | <span data-ttu-id="c6d08-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c6d08-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c6d08-122">period</span><span class="sxs-lookup"><span data-stu-id="c6d08-122">period</span></span>    | <span data-ttu-id="c6d08-123">строка</span><span class="sxs-lookup"><span data-stu-id="c6d08-123">string</span></span> | <span data-ttu-id="c6d08-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c6d08-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c6d08-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c6d08-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c6d08-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c6d08-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c6d08-127">date</span><span class="sxs-lookup"><span data-stu-id="c6d08-127">date</span></span>      | <span data-ttu-id="c6d08-128">Date</span><span class="sxs-lookup"><span data-stu-id="c6d08-128">Date</span></span>   | <span data-ttu-id="c6d08-129">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="c6d08-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c6d08-130">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="c6d08-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c6d08-131">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="c6d08-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c6d08-132">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="c6d08-132">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6d08-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6d08-133">Request headers</span></span>

| <span data-ttu-id="c6d08-134">Имя</span><span class="sxs-lookup"><span data-stu-id="c6d08-134">Name</span></span>          | <span data-ttu-id="c6d08-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c6d08-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c6d08-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6d08-136">Authorization</span></span> | <span data-ttu-id="c6d08-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6d08-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c6d08-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6d08-139">Response</span></span>

<span data-ttu-id="c6d08-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c6d08-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c6d08-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c6d08-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c6d08-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c6d08-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c6d08-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c6d08-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="c6d08-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c6d08-144">Report Refresh Date</span></span>
- <span data-ttu-id="c6d08-145">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="c6d08-145">User Principal Name</span></span>
- <span data-ttu-id="c6d08-146">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="c6d08-146">Last Activity Date</span></span>
- <span data-ttu-id="c6d08-147">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="c6d08-147">Is Deleted</span></span>
- <span data-ttu-id="c6d08-148">Deleted Date (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="c6d08-148">Deleted Date</span></span>
- <span data-ttu-id="c6d08-149">Assigned Products (Назначенные продукты);</span><span class="sxs-lookup"><span data-stu-id="c6d08-149">Assigned Products</span></span>
- <span data-ttu-id="c6d08-150">Team Chat Messages Count (Количество сообщений в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="c6d08-150">Team Chat Message Count</span></span>
- <span data-ttu-id="c6d08-151">Private Chat Message Count (Количество сообщений в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="c6d08-151">Private Chat Message Count</span></span>
- <span data-ttu-id="c6d08-152">Call Count (Количество звонков);</span><span class="sxs-lookup"><span data-stu-id="c6d08-152">Call Count</span></span>
- <span data-ttu-id="c6d08-153">Meeting Count (Количество собраний);</span><span class="sxs-lookup"><span data-stu-id="c6d08-153">Meeting Count</span></span>
- <span data-ttu-id="c6d08-154">Has Other Action (Есть другое действие);</span><span class="sxs-lookup"><span data-stu-id="c6d08-154">Has Other Action</span></span>
- <span data-ttu-id="c6d08-155">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="c6d08-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c6d08-156">Пример</span><span class="sxs-lookup"><span data-stu-id="c6d08-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c6d08-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6d08-157">Request</span></span>

<span data-ttu-id="c6d08-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6d08-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="c6d08-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6d08-159">Response</span></span>

<span data-ttu-id="c6d08-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c6d08-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="c6d08-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c6d08-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```
