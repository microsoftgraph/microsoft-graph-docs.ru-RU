---
title: Список deviceManagementScriptAssignments
description: Список свойств и связей объектов deviceManagementScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 58ea2dc537a444f05d717f98814bc10aeb8d715b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156450"
---
# <a name="list-devicemanagementscriptassignments"></a><span data-ttu-id="e2859-103">Список deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="e2859-103">List deviceManagementScriptAssignments</span></span>

<span data-ttu-id="e2859-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2859-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2859-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2859-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2859-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2859-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2859-107">Список свойств и связей объектов [deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e2859-107">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2859-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e2859-108">Prerequisites</span></span>
<span data-ttu-id="e2859-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2859-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2859-111">Permission type</span></span>|<span data-ttu-id="e2859-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2859-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2859-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2859-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2859-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2859-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e2859-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2859-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2859-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2859-116">Not supported.</span></span>|
|<span data-ttu-id="e2859-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2859-117">Application</span></span>|<span data-ttu-id="e2859-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2859-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2859-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2859-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
GET /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e2859-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e2859-120">Request headers</span></span>
|<span data-ttu-id="e2859-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2859-121">Header</span></span>|<span data-ttu-id="e2859-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e2859-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2859-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2859-123">Authorization</span></span>|<span data-ttu-id="e2859-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2859-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2859-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e2859-125">Accept</span></span>|<span data-ttu-id="e2859-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2859-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2859-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2859-127">Request body</span></span>
<span data-ttu-id="e2859-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2859-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2859-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2859-129">Response</span></span>
<span data-ttu-id="e2859-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2859-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2859-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e2859-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2859-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2859-132">Request</span></span>
<span data-ttu-id="e2859-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2859-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
```

### <a name="response"></a><span data-ttu-id="e2859-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2859-134">Response</span></span>
<span data-ttu-id="e2859-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2859-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 505

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
      "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




