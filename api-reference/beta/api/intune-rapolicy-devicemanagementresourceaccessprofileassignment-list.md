---
title: Список Девицеманажементресаурцеакцесспрофилеассигнментс
description: Список свойств и связей объектов Девицеманажементресаурцеакцесспрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba45fd9dffddf0638af4160efe8d9717181e3f04
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242292"
---
# <a name="list-devicemanagementresourceaccessprofileassignments"></a><span data-ttu-id="018af-103">Список Девицеманажементресаурцеакцесспрофилеассигнментс</span><span class="sxs-lookup"><span data-stu-id="018af-103">List deviceManagementResourceAccessProfileAssignments</span></span>

<span data-ttu-id="018af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="018af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="018af-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="018af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="018af-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="018af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="018af-107">Список свойств и связей объектов [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="018af-107">List properties and relationships of the [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="018af-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="018af-108">Prerequisites</span></span>
<span data-ttu-id="018af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="018af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="018af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="018af-111">Permission type</span></span>|<span data-ttu-id="018af-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="018af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="018af-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="018af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="018af-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="018af-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="018af-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="018af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="018af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="018af-116">Not supported.</span></span>|
|<span data-ttu-id="018af-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="018af-117">Application</span></span>|<span data-ttu-id="018af-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="018af-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="018af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="018af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="018af-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="018af-120">Request headers</span></span>
|<span data-ttu-id="018af-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="018af-121">Header</span></span>|<span data-ttu-id="018af-122">Значение</span><span class="sxs-lookup"><span data-stu-id="018af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="018af-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="018af-123">Authorization</span></span>|<span data-ttu-id="018af-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="018af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="018af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="018af-125">Accept</span></span>|<span data-ttu-id="018af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="018af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="018af-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="018af-127">Request body</span></span>
<span data-ttu-id="018af-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="018af-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="018af-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="018af-129">Response</span></span>
<span data-ttu-id="018af-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="018af-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="018af-131">Пример</span><span class="sxs-lookup"><span data-stu-id="018af-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="018af-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="018af-132">Request</span></span>
<span data-ttu-id="018af-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="018af-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments
```

### <a name="response"></a><span data-ttu-id="018af-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="018af-134">Response</span></span>
<span data-ttu-id="018af-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="018af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 517

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
      "id": "4ebb8d4e-8d4e-4ebb-4e8d-bb4e4e8dbb4e",
      "intent": "remove",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "sourceId": "Source Id value"
    }
  ]
}
```




