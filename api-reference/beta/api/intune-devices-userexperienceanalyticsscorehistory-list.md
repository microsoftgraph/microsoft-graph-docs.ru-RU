---
title: Список userExperienceAnalyticsScoreHistories
description: Список свойств и связей объектов userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b0dc569752e2620b33b2ca455e9e431c3529e7d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146148"
---
# <a name="list-userexperienceanalyticsscorehistories"></a><span data-ttu-id="4a89d-103">Список userExperienceAnalyticsScoreHistories</span><span class="sxs-lookup"><span data-stu-id="4a89d-103">List userExperienceAnalyticsScoreHistories</span></span>

<span data-ttu-id="4a89d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a89d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a89d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a89d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a89d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a89d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a89d-107">Список свойств и связей [объектов userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)</span><span class="sxs-lookup"><span data-stu-id="4a89d-107">List properties and relationships of the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a89d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4a89d-108">Prerequisites</span></span>
<span data-ttu-id="4a89d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a89d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a89d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a89d-111">Permission type</span></span>|<span data-ttu-id="4a89d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a89d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a89d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a89d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a89d-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a89d-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4a89d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a89d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a89d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a89d-116">Not supported.</span></span>|
|<span data-ttu-id="4a89d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4a89d-117">Application</span></span>|<span data-ttu-id="4a89d-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a89d-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a89d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a89d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="4a89d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4a89d-120">Request headers</span></span>
|<span data-ttu-id="4a89d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a89d-121">Header</span></span>|<span data-ttu-id="4a89d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4a89d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a89d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a89d-123">Authorization</span></span>|<span data-ttu-id="4a89d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a89d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a89d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4a89d-125">Accept</span></span>|<span data-ttu-id="4a89d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a89d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a89d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a89d-127">Request body</span></span>
<span data-ttu-id="4a89d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a89d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a89d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a89d-129">Response</span></span>
<span data-ttu-id="4a89d-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4a89d-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a89d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4a89d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a89d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a89d-132">Request</span></span>
<span data-ttu-id="4a89d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a89d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory
```

### <a name="response"></a><span data-ttu-id="4a89d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a89d-134">Response</span></span>
<span data-ttu-id="4a89d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a89d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
      "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
      "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
      "startupScore": 12,
      "coreBootScore": 13,
      "coreSigninScore": 15,
      "recommendedSoftwareScore": 8,
      "restartScore": 12
    }
  ]
}
```




