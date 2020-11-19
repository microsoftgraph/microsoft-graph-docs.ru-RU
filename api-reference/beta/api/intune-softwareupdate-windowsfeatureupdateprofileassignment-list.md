---
title: Список Виндовсфеатуреупдатепрофилеассигнментс
description: Список свойств и связей объектов Виндовсфеатуреупдатепрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1dc58e50c53951d05ba2196e9e9d081a1ec0c751
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223663"
---
# <a name="list-windowsfeatureupdateprofileassignments"></a><span data-ttu-id="8ebb9-103">Список Виндовсфеатуреупдатепрофилеассигнментс</span><span class="sxs-lookup"><span data-stu-id="8ebb9-103">List windowsFeatureUpdateProfileAssignments</span></span>

<span data-ttu-id="8ebb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ebb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ebb9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ebb9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ebb9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ebb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ebb9-107">Список свойств и связей объектов [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8ebb9-107">List properties and relationships of the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ebb9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8ebb9-108">Prerequisites</span></span>
<span data-ttu-id="8ebb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ebb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ebb9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ebb9-111">Permission type</span></span>|<span data-ttu-id="8ebb9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ebb9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ebb9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ebb9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ebb9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ebb9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8ebb9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ebb9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ebb9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ebb9-116">Not supported.</span></span>|
|<span data-ttu-id="8ebb9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8ebb9-117">Application</span></span>|<span data-ttu-id="8ebb9-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ebb9-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ebb9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ebb9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8ebb9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8ebb9-120">Request headers</span></span>
|<span data-ttu-id="8ebb9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ebb9-121">Header</span></span>|<span data-ttu-id="8ebb9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8ebb9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ebb9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ebb9-123">Authorization</span></span>|<span data-ttu-id="8ebb9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ebb9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ebb9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ebb9-125">Accept</span></span>|<span data-ttu-id="8ebb9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ebb9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ebb9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ebb9-127">Request body</span></span>
<span data-ttu-id="8ebb9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ebb9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ebb9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ebb9-129">Response</span></span>
<span data-ttu-id="8ebb9-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ebb9-130">If successful, this method returns a `200 OK` response code and a collection of [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ebb9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8ebb9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ebb9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ebb9-132">Request</span></span>
<span data-ttu-id="8ebb9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ebb9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="8ebb9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ebb9-134">Response</span></span>
<span data-ttu-id="8ebb9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ebb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 454

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
      "id": "567a744f-744f-567a-4f74-7a564f747a56",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```




