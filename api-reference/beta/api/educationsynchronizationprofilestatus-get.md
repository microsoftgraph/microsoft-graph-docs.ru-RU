---
title: Получить сведения о состоянии educationSynchronizationProfile
description: Получите сведения о состоянии определенного школа данных синхронизации профиля в клиентов. Ответ будет указывают состояние синхронизации.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6a2d3dffd715d78bb96794808da39255db0164b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510199"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="53ca5-104">Получить сведения о состоянии educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="53ca5-104">Get the status of an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53ca5-105">Получите сведения о состоянии данных конкретного школа [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="53ca5-105">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="53ca5-106">Ответ будет указывают состояние синхронизации.</span><span class="sxs-lookup"><span data-stu-id="53ca5-106">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="53ca5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53ca5-107">Permissions</span></span>
<span data-ttu-id="53ca5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53ca5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53ca5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53ca5-110">Permission type</span></span> | <span data-ttu-id="53ca5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53ca5-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="53ca5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53ca5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="53ca5-113">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53ca5-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="53ca5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53ca5-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="53ca5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53ca5-115">Not supported.</span></span>|
|<span data-ttu-id="53ca5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53ca5-116">Application</span></span>| <span data-ttu-id="53ca5-117">EduAdministration.Read.All EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53ca5-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53ca5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53ca5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="53ca5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53ca5-119">Request headers</span></span>
| <span data-ttu-id="53ca5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="53ca5-120">Name</span></span>       | <span data-ttu-id="53ca5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="53ca5-121">Type</span></span> | <span data-ttu-id="53ca5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="53ca5-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="53ca5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53ca5-123">Authorization</span></span>  | <span data-ttu-id="53ca5-124">string</span><span class="sxs-lookup"><span data-stu-id="53ca5-124">string</span></span>  | <span data-ttu-id="53ca5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53ca5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53ca5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53ca5-127">Request body</span></span>
<span data-ttu-id="53ca5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53ca5-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="53ca5-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="53ca5-129">Response</span></span>
<span data-ttu-id="53ca5-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="53ca5-130">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53ca5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="53ca5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53ca5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="53ca5-132">Request</span></span>
<span data-ttu-id="53ca5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53ca5-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a><span data-ttu-id="53ca5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="53ca5-134">Response</span></span>
<span data-ttu-id="53ca5-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53ca5-135">The following is an example of the response.</span></span> 

><span data-ttu-id="53ca5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53ca5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofilestatus-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
