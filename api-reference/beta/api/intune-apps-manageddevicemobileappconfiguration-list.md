---
title: Перечисление объектов managedDeviceMobileAppConfiguration
description: Перечисление свойств и связей объектов managedDeviceMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e2c6fc5afc8f302e309584773fd4f9c49a9982e6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406113"
---
# <a name="list-manageddevicemobileappconfigurations"></a><span data-ttu-id="e9c29-103">Перечисление объектов managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9c29-103">List managedDeviceMobileAppConfigurations</span></span>

<span data-ttu-id="e9c29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9c29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9c29-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9c29-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9c29-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9c29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9c29-107">Перечисление свойств и связей объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9c29-107">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9c29-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e9c29-108">Prerequisites</span></span>
<span data-ttu-id="e9c29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9c29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9c29-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9c29-111">Permission type</span></span>|<span data-ttu-id="e9c29-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9c29-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9c29-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9c29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9c29-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9c29-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e9c29-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9c29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9c29-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9c29-116">Not supported.</span></span>|
|<span data-ttu-id="e9c29-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e9c29-117">Application</span></span>|<span data-ttu-id="e9c29-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9c29-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9c29-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9c29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e9c29-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e9c29-120">Request headers</span></span>
|<span data-ttu-id="e9c29-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9c29-121">Header</span></span>|<span data-ttu-id="e9c29-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e9c29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9c29-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9c29-123">Authorization</span></span>|<span data-ttu-id="e9c29-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9c29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9c29-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9c29-125">Accept</span></span>|<span data-ttu-id="e9c29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9c29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9c29-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9c29-127">Request body</span></span>
<span data-ttu-id="e9c29-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9c29-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9c29-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9c29-129">Response</span></span>
<span data-ttu-id="e9c29-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e9c29-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9c29-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e9c29-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9c29-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9c29-132">Request</span></span>
<span data-ttu-id="e9c29-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9c29-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="e9c29-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9c29-134">Response</span></span>
<span data-ttu-id="e9c29-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9c29-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 559

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
      "id": "c60e7591-7591-c60e-9175-0ec691750ec6",
      "targetedMobileApps": [
        "Targeted Mobile Apps value"
      ],
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```



