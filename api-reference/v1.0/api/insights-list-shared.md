---
title: Список "Общие"
description: Расчетные данные, возвращающие список файлов, которыми вы поделились с пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 0b799be314ce9f2519d7174c84f9349b09bbd5c3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050425"
---
# <a name="list-shared"></a><span data-ttu-id="a8dda-103">Список "Общие"</span><span class="sxs-lookup"><span data-stu-id="a8dda-103">List shared</span></span>

<span data-ttu-id="a8dda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8dda-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8dda-105">Вычисляемая информация, которая включает список документов, общих пользователю.</span><span class="sxs-lookup"><span data-stu-id="a8dda-105">Calculated insight that includes the list of documents shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8dda-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8dda-106">Permissions</span></span>
<span data-ttu-id="a8dda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8dda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8dda-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8dda-109">Permission type</span></span>      | <span data-ttu-id="a8dda-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8dda-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8dda-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8dda-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a8dda-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8dda-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a8dda-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8dda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8dda-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8dda-114">Not supported.</span></span>    |
|<span data-ttu-id="a8dda-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8dda-115">Application</span></span> | <span data-ttu-id="a8dda-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8dda-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8dda-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8dda-117">HTTP request</span></span>
<span data-ttu-id="a8dda-118">Получите список документов, общих пользователю, вписав его.</span><span class="sxs-lookup"><span data-stu-id="a8dda-118">Get a list of documents shared with the signed-in user.</span></span>

><span data-ttu-id="a8dda-119">**Примечание.** Только пользователь может делать запросы с помощью id или основного имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="a8dda-119">**Note**: Only the user can make requests using the user's id or principal name.</span></span>

```http
GET /me/insights/shared
GET /users/{id | userPrincipalName}/insights/shared
```

<span data-ttu-id="a8dda-120">Расширение ресурса, на который ссылается общая **информация:**</span><span class="sxs-lookup"><span data-stu-id="a8dda-120">Expand the resource referenced by a **shared** insight:</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8dda-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a8dda-121">Optional query parameters</span></span>
<span data-ttu-id="a8dda-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a8dda-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="a8dda-123">Параметр запроса можно `$filter` использовать для фильтрации общих элементов.</span><span class="sxs-lookup"><span data-stu-id="a8dda-123">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="a8dda-124">Например, в зависимости от **типа:**</span><span class="sxs-lookup"><span data-stu-id="a8dda-124">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="a8dda-125">В [resourceVisualization](../resources/insights-resourcevisualization.md)см. доступные типы и типы контейнеров, которые можно фильтровать.</span><span class="sxs-lookup"><span data-stu-id="a8dda-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="a8dda-126">Вы также можете получить файлы, общие для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a8dda-126">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="a8dda-127">Например, укажите `lastshared/sharedby/address` свойство:</span><span class="sxs-lookup"><span data-stu-id="a8dda-127">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="a8dda-128">См. [сложный тип sharingDetail.](../resources/insights-sharingdetail.md)</span><span class="sxs-lookup"><span data-stu-id="a8dda-128">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="a8dda-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8dda-129">Request headers</span></span>
| <span data-ttu-id="a8dda-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8dda-130">Header</span></span>       |  <span data-ttu-id="a8dda-131">Значение</span><span class="sxs-lookup"><span data-stu-id="a8dda-131">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="a8dda-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8dda-132">Authorization</span></span>  | <span data-ttu-id="a8dda-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8dda-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="a8dda-135">Accept</span><span class="sxs-lookup"><span data-stu-id="a8dda-135">Accept</span></span>  | <span data-ttu-id="a8dda-136">application/json</span><span class="sxs-lookup"><span data-stu-id="a8dda-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8dda-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8dda-137">Request body</span></span>
<span data-ttu-id="a8dda-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8dda-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8dda-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8dda-139">Response</span></span>

<span data-ttu-id="a8dda-140">В случае успешной работы этот метод возвращает код ответа и список общих элементов `200 OK` в тексте [](../resources/insights-shared.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="a8dda-140">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a8dda-141">Пример</span><span class="sxs-lookup"><span data-stu-id="a8dda-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a8dda-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8dda-142">Request</span></span>

<span data-ttu-id="a8dda-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8dda-143">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="a8dda-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8dda-144">Response</span></span>

<span data-ttu-id="a8dda-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a8dda-145">Here is an example of the response.</span></span> <span data-ttu-id="a8dda-146">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a8dda-146">Note: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "AWb0Qy4TEA1KhLW-k1L5mSjtxZAcxDFkTKiTNA-2kZDTXzrMX_4FhECOU0bKZVj1uReivYoYYoJNqTeuC-x1Agtm9EMuExANSoS1vpNS-ZkoBA",
            "lastShared": {
                "sharedDateTime": "2021-03-23T08:41:05Z",
                "sharingType": "Direct",
                "sharedBy": {
                    "displayName": "Megan Bowen",
                    "address": "MeganB@contoso.com",
                    "id": "3e0c9f05-b9b8-4cf5-9b35-a4e11b24b5b7"
                },
                "sharingReference": {}
            },
            "resourceVisualization": {
                "title": "CE Annual Report",
                "type": "Word",
                "mediaType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
                "previewImageUrl": "https://contoso-my.sharepoint.com/_api/v2.0/drives/b!ZvRDLhMQDUqEtb6TUvmZKO3FkBzEMWRMqJM0D7aRkNNfOsxf_gWEQI5TRsplWPW5/items/01K6ZMU4QXUK6YUGDCQJG2SN5OBPWHKAQL/thumbnails/0/small/thumbnailContent",
                "previewText": "Contoso Annual Report Anne Wallace Sales Contoso today announced financial results for its most recent fi",
                "containerWebUrl": "https://contoso-my.sharepoint.com/personal/meganb_m365x841051_onmicrosoft_com/Documents/Forms/All.aspx",
                "containerDisplayName": "Megan Bowen",
                "containerType": "OneDriveBusiness"
            },
            "resourceReference": {
                "webUrl": "https://contoso-my.sharepoint.com/personal/meganb_m365x841051_onmicrosoft_com/_layouts/15/Doc.aspx?sourcedoc=%7B8ABDA217-6218-4D82-A937-AE0BEC75020B%7D&file=CE%20Annual%20Report.docx&action=default&mobileredirect=true&DefaultItemOpen=1",
                "id": "drives/b!ZvRDLhMQDUqEtb6TUvmZKO3FkBzEMWRMqJM0D7aRkNNfOsxf_gWEQI5TRsplWPW5/items/01K6ZMU4QXUK6YUGDCQJG2SN5OBPWHKAQL",
                "type": "microsoft.graph.driveItem"
            }
        }
    ]
}
```
