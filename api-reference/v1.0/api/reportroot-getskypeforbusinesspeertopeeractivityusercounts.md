---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts'
description: Отследите динамику использования по количеству уникальных пользователей и типу проведенных в организации одноранговых сеансов. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов в одноранговых сеансах).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 98eadcbee3d2465446c3fe6b581da004f0c54ed4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554711"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="0932d-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="0932d-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

<span data-ttu-id="0932d-105">Отследите динамику использования по количеству уникальных пользователей и типу проведенных в организации одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="0932d-105">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="0932d-106">Такие типы включают обмен мгновенными сообщениями, предоставление общего доступа к приложениям, аудио, видео, а также передачу файлов в одноранговых сеансах.</span><span class="sxs-lookup"><span data-stu-id="0932d-106">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="0932d-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в одноранговых сеансах Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="0932d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="0932d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0932d-108">Permissions</span></span>

<span data-ttu-id="0932d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0932d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0932d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0932d-111">Permission type</span></span>                        | <span data-ttu-id="0932d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0932d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0932d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0932d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0932d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0932d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0932d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0932d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0932d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0932d-116">Not supported.</span></span>                           |
| <span data-ttu-id="0932d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0932d-117">Application</span></span>                            | <span data-ttu-id="0932d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0932d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0932d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0932d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0932d-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="0932d-120">Function parameters</span></span>

<span data-ttu-id="0932d-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="0932d-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0932d-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="0932d-122">Parameter</span></span> | <span data-ttu-id="0932d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0932d-123">Type</span></span>   | <span data-ttu-id="0932d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0932d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0932d-125">period</span><span class="sxs-lookup"><span data-stu-id="0932d-125">period</span></span>    | <span data-ttu-id="0932d-126">string</span><span class="sxs-lookup"><span data-stu-id="0932d-126">string</span></span> | <span data-ttu-id="0932d-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="0932d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0932d-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="0932d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0932d-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="0932d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0932d-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0932d-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0932d-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0932d-131">Request headers</span></span>

| <span data-ttu-id="0932d-132">Имя</span><span class="sxs-lookup"><span data-stu-id="0932d-132">Name</span></span>          | <span data-ttu-id="0932d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0932d-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0932d-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0932d-134">Authorization</span></span> | <span data-ttu-id="0932d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0932d-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0932d-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0932d-137">If-None-Match</span></span> | <span data-ttu-id="0932d-138">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="0932d-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0932d-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="0932d-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0932d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0932d-140">Response</span></span>

<span data-ttu-id="0932d-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="0932d-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0932d-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="0932d-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0932d-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0932d-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0932d-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="0932d-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0932d-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="0932d-145">Report Refresh Date</span></span>
- <span data-ttu-id="0932d-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="0932d-146">Report Date</span></span>
- <span data-ttu-id="0932d-147">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="0932d-147">Report Period</span></span>
- <span data-ttu-id="0932d-148">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="0932d-148">IM</span></span>
- <span data-ttu-id="0932d-149">"Audio" (Аудио);</span><span class="sxs-lookup"><span data-stu-id="0932d-149">Audio</span></span>
- <span data-ttu-id="0932d-150">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="0932d-150">Video</span></span>
- <span data-ttu-id="0932d-151">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="0932d-151">App Sharing</span></span>
- <span data-ttu-id="0932d-152">"File Transfer" (Передача файлов).</span><span class="sxs-lookup"><span data-stu-id="0932d-152">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="0932d-153">Пример</span><span class="sxs-lookup"><span data-stu-id="0932d-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0932d-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="0932d-154">Request</span></span>

<span data-ttu-id="0932d-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0932d-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="0932d-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="0932d-156">Response</span></span>

<span data-ttu-id="0932d-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0932d-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="0932d-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="0932d-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```
