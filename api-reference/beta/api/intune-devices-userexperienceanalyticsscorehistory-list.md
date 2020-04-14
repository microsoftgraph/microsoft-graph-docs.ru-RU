---
title: Список Усерекспериенцеаналитиксскорехисториес
description: Список свойств и связей объектов Усерекспериенцеаналитиксскорехистори.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6398d9d8950fedca2951fae6a223120240ff8ce
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43378939"
---
# <a name="list-userexperienceanalyticsscorehistories"></a><span data-ttu-id="4b616-103">Список Усерекспериенцеаналитиксскорехисториес</span><span class="sxs-lookup"><span data-stu-id="4b616-103">List userExperienceAnalyticsScoreHistories</span></span>

<span data-ttu-id="4b616-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b616-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b616-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b616-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b616-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b616-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b616-107">Список свойств и связей объектов [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="4b616-107">List properties and relationships of the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b616-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b616-108">Prerequisites</span></span>
<span data-ttu-id="4b616-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b616-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b616-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b616-111">Permission type</span></span>|<span data-ttu-id="4b616-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b616-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b616-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b616-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b616-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b616-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4b616-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b616-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b616-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b616-116">Not supported.</span></span>|
|<span data-ttu-id="4b616-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4b616-117">Application</span></span>|<span data-ttu-id="4b616-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b616-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b616-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b616-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="4b616-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b616-120">Request headers</span></span>
|<span data-ttu-id="4b616-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b616-121">Header</span></span>|<span data-ttu-id="4b616-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b616-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b616-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b616-123">Authorization</span></span>|<span data-ttu-id="4b616-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b616-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b616-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b616-125">Accept</span></span>|<span data-ttu-id="4b616-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b616-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b616-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b616-127">Request body</span></span>
<span data-ttu-id="4b616-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b616-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b616-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b616-129">Response</span></span>
<span data-ttu-id="4b616-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b616-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b616-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4b616-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b616-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b616-132">Request</span></span>
<span data-ttu-id="4b616-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b616-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory
```

### <a name="response"></a><span data-ttu-id="4b616-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b616-134">Response</span></span>
<span data-ttu-id="4b616-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b616-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 353

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
      "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
      "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
      "startupScore": 12,
      "coreBootScore": 13,
      "coreSigninScore": 15,
      "recommendedSoftwareScore": 8
    }
  ]
}
```



