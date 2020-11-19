---
title: Перечисление объектов managedDeviceMobileAppConfigurationAssignment
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 24643d6685724b466416dfb0c998dad82edaf8b1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49250305"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="75205-103">Перечисление объектов managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="75205-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

<span data-ttu-id="75205-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75205-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75205-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75205-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75205-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75205-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75205-107">Список свойств и связей объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75205-107">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75205-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="75205-108">Prerequisites</span></span>
<span data-ttu-id="75205-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75205-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75205-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75205-111">Permission type</span></span>|<span data-ttu-id="75205-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75205-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75205-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75205-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75205-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="75205-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="75205-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75205-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75205-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75205-116">Not supported.</span></span>|
|<span data-ttu-id="75205-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="75205-117">Application</span></span>|<span data-ttu-id="75205-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="75205-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75205-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75205-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="75205-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="75205-120">Request headers</span></span>
|<span data-ttu-id="75205-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75205-121">Header</span></span>|<span data-ttu-id="75205-122">Значение</span><span class="sxs-lookup"><span data-stu-id="75205-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75205-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75205-123">Authorization</span></span>|<span data-ttu-id="75205-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75205-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75205-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75205-125">Accept</span></span>|<span data-ttu-id="75205-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75205-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75205-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75205-127">Request body</span></span>
<span data-ttu-id="75205-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75205-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75205-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="75205-129">Response</span></span>
<span data-ttu-id="75205-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75205-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75205-131">Пример</span><span class="sxs-lookup"><span data-stu-id="75205-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="75205-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="75205-132">Request</span></span>
<span data-ttu-id="75205-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75205-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="75205-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="75205-134">Response</span></span>
<span data-ttu-id="75205-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75205-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 456

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```




