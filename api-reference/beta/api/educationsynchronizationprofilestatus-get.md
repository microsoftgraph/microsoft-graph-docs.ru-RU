---
title: Получить сведения о состоянии educationSynchronizationProfile
description: Получите сведения о состоянии определенного школа данных синхронизации профиля в клиентов. Ответ будет указывают состояние синхронизации.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3b235ca243e6ee0f2ebb442d53a7425fa979d778
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965455"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="91851-104">Получить сведения о состоянии educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="91851-104">Get the status of an educationSynchronizationProfile</span></span>

> <span data-ttu-id="91851-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91851-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91851-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91851-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91851-107">Получите сведения о состоянии данных конкретного школа [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="91851-107">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="91851-108">Ответ будет указывают состояние синхронизации.</span><span class="sxs-lookup"><span data-stu-id="91851-108">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="91851-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91851-109">Permissions</span></span>
<span data-ttu-id="91851-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91851-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91851-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91851-112">Permission type</span></span> | <span data-ttu-id="91851-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91851-113">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="91851-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91851-114">Delegated (work or school account)</span></span> | <span data-ttu-id="91851-115">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91851-115">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="91851-116">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="91851-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="91851-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91851-117">Not supported.</span></span>|
|<span data-ttu-id="91851-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91851-118">Application</span></span>| <span data-ttu-id="91851-119">EduAdministration.Read.All EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91851-119">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91851-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91851-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="91851-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91851-121">Request headers</span></span>
| <span data-ttu-id="91851-122">Имя</span><span class="sxs-lookup"><span data-stu-id="91851-122">Name</span></span>       | <span data-ttu-id="91851-123">Тип</span><span class="sxs-lookup"><span data-stu-id="91851-123">Type</span></span> | <span data-ttu-id="91851-124">Описание</span><span class="sxs-lookup"><span data-stu-id="91851-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="91851-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="91851-125">Authorization</span></span>  | <span data-ttu-id="91851-126">string</span><span class="sxs-lookup"><span data-stu-id="91851-126">string</span></span>  | <span data-ttu-id="91851-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91851-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91851-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91851-129">Request body</span></span>
<span data-ttu-id="91851-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91851-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="91851-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="91851-131">Response</span></span>
<span data-ttu-id="91851-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="91851-132">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91851-133">Пример</span><span class="sxs-lookup"><span data-stu-id="91851-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91851-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="91851-134">Request</span></span>
<span data-ttu-id="91851-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91851-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a><span data-ttu-id="91851-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="91851-136">Response</span></span>
<span data-ttu-id="91851-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="91851-137">The following is an example of the response.</span></span> 

><span data-ttu-id="91851-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91851-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus",
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
