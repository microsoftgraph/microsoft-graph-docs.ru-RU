---
title: Перечисление объектов managedDeviceMobileAppConfigurationAssignment
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7db781fd33984f3abe270c30c03d5ee6bdf401ec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446288"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="34bec-103">Перечисление объектов managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="34bec-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

<span data-ttu-id="34bec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34bec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34bec-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34bec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34bec-106">Список свойств и связей объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="34bec-106">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34bec-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="34bec-107">Prerequisites</span></span>
<span data-ttu-id="34bec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34bec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34bec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34bec-110">Permission type</span></span>|<span data-ttu-id="34bec-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34bec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34bec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34bec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34bec-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="34bec-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="34bec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34bec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34bec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34bec-115">Not supported.</span></span>|
|<span data-ttu-id="34bec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34bec-116">Application</span></span>|<span data-ttu-id="34bec-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34bec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34bec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34bec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="34bec-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="34bec-119">Request headers</span></span>
|<span data-ttu-id="34bec-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34bec-120">Header</span></span>|<span data-ttu-id="34bec-121">Значение</span><span class="sxs-lookup"><span data-stu-id="34bec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34bec-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34bec-122">Authorization</span></span>|<span data-ttu-id="34bec-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34bec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34bec-124">Accept</span><span class="sxs-lookup"><span data-stu-id="34bec-124">Accept</span></span>|<span data-ttu-id="34bec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34bec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34bec-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="34bec-126">Request body</span></span>
<span data-ttu-id="34bec-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34bec-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34bec-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="34bec-128">Response</span></span>
<span data-ttu-id="34bec-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34bec-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34bec-130">Пример</span><span class="sxs-lookup"><span data-stu-id="34bec-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="34bec-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="34bec-131">Request</span></span>
<span data-ttu-id="34bec-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34bec-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="34bec-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="34bec-133">Response</span></span>
<span data-ttu-id="34bec-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34bec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```






