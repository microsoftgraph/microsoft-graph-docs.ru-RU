---
title: Получение состояния Едукатионсинчронизатионпрофиле
description: Получение состояния определенного профиля синхронизации данных School в клиенте. Ответ будет указывать на состояние синхронизации.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6a2d3dffd715d78bb96794808da39255db0164b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457475"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="8f952-104">Получение состояния Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="8f952-104">Get the status of an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f952-105">Получение состояния определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="8f952-105">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="8f952-106">Ответ будет указывать на состояние синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8f952-106">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f952-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f952-107">Permissions</span></span>
<span data-ttu-id="8f952-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f952-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f952-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f952-110">Permission type</span></span> | <span data-ttu-id="8f952-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f952-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="8f952-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f952-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8f952-113">Едуадминистратион. Read, Едуадминистратион. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f952-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="8f952-114">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f952-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="8f952-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f952-115">Not supported.</span></span>|
|<span data-ttu-id="8f952-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f952-116">Application</span></span>| <span data-ttu-id="8f952-117">Едуадминистратион. Read. ALL, Едуадминистратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8f952-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f952-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f952-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="8f952-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f952-119">Request headers</span></span>
| <span data-ttu-id="8f952-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8f952-120">Name</span></span>       | <span data-ttu-id="8f952-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8f952-121">Type</span></span> | <span data-ttu-id="8f952-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8f952-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8f952-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f952-123">Authorization</span></span>  | <span data-ttu-id="8f952-124">string</span><span class="sxs-lookup"><span data-stu-id="8f952-124">string</span></span>  | <span data-ttu-id="8f952-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f952-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8f952-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f952-127">Request body</span></span>
<span data-ttu-id="8f952-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f952-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8f952-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f952-129">Response</span></span>
<span data-ttu-id="8f952-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [едукатионсинчронизатионпрофилестатус](../resources/educationsynchronizationprofilestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f952-130">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f952-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8f952-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f952-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f952-132">Request</span></span>
<span data-ttu-id="8f952-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f952-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a><span data-ttu-id="8f952-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f952-134">Response</span></span>
<span data-ttu-id="8f952-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8f952-135">The following is an example of the response.</span></span> 

><span data-ttu-id="8f952-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f952-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
