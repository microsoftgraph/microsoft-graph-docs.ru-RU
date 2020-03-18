---
title: Список Усерекспериенцеаналитиксстартупскорехисториес
description: Список свойств и связей объектов Усерекспериенцеаналитиксстартупскорехистори.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7bba0d9f0c76ef2d4876fa6aa99d5916427f998d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813756"
---
# <a name="list-userexperienceanalyticsstartupscorehistories"></a><span data-ttu-id="45776-103">Список Усерекспериенцеаналитиксстартупскорехисториес</span><span class="sxs-lookup"><span data-stu-id="45776-103">List userExperienceAnalyticsStartupScoreHistories</span></span>

> <span data-ttu-id="45776-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45776-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45776-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45776-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45776-106">Список свойств и связей объектов [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="45776-106">List properties and relationships of the [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45776-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45776-107">Prerequisites</span></span>
<span data-ttu-id="45776-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45776-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45776-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45776-110">Permission type</span></span>|<span data-ttu-id="45776-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45776-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45776-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45776-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45776-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="45776-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="45776-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45776-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45776-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45776-115">Not supported.</span></span>|
|<span data-ttu-id="45776-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="45776-116">Application</span></span>|<span data-ttu-id="45776-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="45776-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45776-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45776-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsStartupScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="45776-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45776-119">Request headers</span></span>
|<span data-ttu-id="45776-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45776-120">Header</span></span>|<span data-ttu-id="45776-121">Значение</span><span class="sxs-lookup"><span data-stu-id="45776-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45776-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="45776-122">Authorization</span></span>|<span data-ttu-id="45776-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45776-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45776-124">Accept</span><span class="sxs-lookup"><span data-stu-id="45776-124">Accept</span></span>|<span data-ttu-id="45776-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45776-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45776-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45776-126">Request body</span></span>
<span data-ttu-id="45776-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45776-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45776-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="45776-128">Response</span></span>
<span data-ttu-id="45776-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45776-129">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45776-130">Пример</span><span class="sxs-lookup"><span data-stu-id="45776-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="45776-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="45776-131">Request</span></span>
<span data-ttu-id="45776-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45776-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsStartupScoreHistory
```

### <a name="response"></a><span data-ttu-id="45776-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="45776-133">Response</span></span>
<span data-ttu-id="45776-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45776-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 360

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
      "id": "52efee0b-ee0b-52ef-0bee-ef520beeef52",
      "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
      "startupScore": 12,
      "coreBootScore": 13,
      "coreSigninScore": 15,
      "recommendedSoftwareScore": 8
    }
  ]
}
```




