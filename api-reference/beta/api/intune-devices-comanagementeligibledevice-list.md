---
title: Список Команажементелигибледевицес
description: Список свойств и связей объектов Команажементелигибледевице.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2aba5e3294162a6584a0f7b2f133f9fa78f6e80a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792529"
---
# <a name="list-comanagementeligibledevices"></a><span data-ttu-id="d8735-103">Список Команажементелигибледевицес</span><span class="sxs-lookup"><span data-stu-id="d8735-103">List comanagementEligibleDevices</span></span>

<span data-ttu-id="d8735-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8735-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8735-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8735-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8735-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8735-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8735-107">Список свойств и связей объектов [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md) .</span><span class="sxs-lookup"><span data-stu-id="d8735-107">List properties and relationships of the [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8735-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d8735-108">Prerequisites</span></span>
<span data-ttu-id="d8735-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8735-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8735-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8735-111">Permission type</span></span>|<span data-ttu-id="d8735-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8735-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8735-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8735-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8735-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8735-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d8735-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8735-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8735-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8735-116">Not supported.</span></span>|
|<span data-ttu-id="d8735-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8735-117">Application</span></span>|<span data-ttu-id="d8735-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8735-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8735-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8735-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/comanagementEligibleDevices
```

## <a name="request-headers"></a><span data-ttu-id="d8735-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d8735-120">Request headers</span></span>
|<span data-ttu-id="d8735-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8735-121">Header</span></span>|<span data-ttu-id="d8735-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d8735-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8735-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8735-123">Authorization</span></span>|<span data-ttu-id="d8735-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8735-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8735-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d8735-125">Accept</span></span>|<span data-ttu-id="d8735-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8735-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8735-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d8735-127">Request body</span></span>
<span data-ttu-id="d8735-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8735-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8735-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8735-129">Response</span></span>
<span data-ttu-id="d8735-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8735-130">If successful, this method returns a `200 OK` response code and a collection of [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8735-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d8735-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8735-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8735-132">Request</span></span>
<span data-ttu-id="d8735-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8735-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleDevices
```

### <a name="response"></a><span data-ttu-id="d8735-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8735-134">Response</span></span>
<span data-ttu-id="d8735-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8735-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 880

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
      "id": "ac20683b-683b-ac20-3b68-20ac3b6820ac",
      "deviceName": "Device Name value",
      "deviceType": "windowsRT",
      "clientRegistrationStatus": "registered",
      "ownerType": "company",
      "managementAgents": "mdm",
      "managementState": "retirePending",
      "referenceId": "Reference Id value",
      "mdmStatus": "Mdm Status value",
      "osVersion": "Os Version value",
      "serialNumber": "Serial Number value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "osDescription": "Os Description value",
      "entitySource": 12,
      "userId": "User Id value",
      "upn": "Upn value",
      "userEmail": "User Email value",
      "userName": "User Name value",
      "status": "eligible"
    }
  ]
}
```



