---
title: Перечисление объектов managedDeviceMobileAppConfiguration
description: Перечисление свойств и связей объектов managedDeviceMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dd1a0f4e4f3be63bc79e6fa30f858c962c2a45ee
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699515"
---
# <a name="list-manageddevicemobileappconfigurations"></a><span data-ttu-id="d4397-103">Перечисление объектов managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4397-103">List managedDeviceMobileAppConfigurations</span></span>

<span data-ttu-id="d4397-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4397-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4397-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4397-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4397-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4397-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4397-107">Перечисление свойств и связей объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4397-107">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4397-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d4397-108">Prerequisites</span></span>
<span data-ttu-id="d4397-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4397-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4397-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4397-111">Permission type</span></span>|<span data-ttu-id="d4397-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4397-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4397-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4397-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4397-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4397-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d4397-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4397-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4397-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4397-116">Not supported.</span></span>|
|<span data-ttu-id="d4397-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4397-117">Application</span></span>|<span data-ttu-id="d4397-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4397-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4397-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4397-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d4397-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d4397-120">Request headers</span></span>
|<span data-ttu-id="d4397-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4397-121">Header</span></span>|<span data-ttu-id="d4397-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d4397-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4397-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4397-123">Authorization</span></span>|<span data-ttu-id="d4397-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4397-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4397-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4397-125">Accept</span></span>|<span data-ttu-id="d4397-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4397-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4397-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d4397-127">Request body</span></span>
<span data-ttu-id="d4397-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4397-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4397-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4397-129">Response</span></span>
<span data-ttu-id="d4397-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4397-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4397-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d4397-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4397-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4397-132">Request</span></span>
<span data-ttu-id="d4397-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4397-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="d4397-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4397-134">Response</span></span>
<span data-ttu-id="d4397-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4397-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





