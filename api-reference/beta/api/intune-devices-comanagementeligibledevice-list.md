---
title: Список Команажементелигибледевицес
description: Список свойств и связей объектов Команажементелигибледевице.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c8a3d82e1daec393502019b2ca63978c607a169a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49229466"
---
# <a name="list-comanagementeligibledevices"></a><span data-ttu-id="f1cc8-103">Список Команажементелигибледевицес</span><span class="sxs-lookup"><span data-stu-id="f1cc8-103">List comanagementEligibleDevices</span></span>

<span data-ttu-id="f1cc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1cc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1cc8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1cc8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1cc8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1cc8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1cc8-107">Список свойств и связей объектов [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md) .</span><span class="sxs-lookup"><span data-stu-id="f1cc8-107">List properties and relationships of the [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1cc8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1cc8-108">Prerequisites</span></span>
<span data-ttu-id="f1cc8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1cc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1cc8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1cc8-111">Permission type</span></span>|<span data-ttu-id="f1cc8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1cc8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1cc8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1cc8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1cc8-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1cc8-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f1cc8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1cc8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1cc8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1cc8-116">Not supported.</span></span>|
|<span data-ttu-id="f1cc8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f1cc8-117">Application</span></span>|<span data-ttu-id="f1cc8-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1cc8-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1cc8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1cc8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/comanagementEligibleDevices
```

## <a name="request-headers"></a><span data-ttu-id="f1cc8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f1cc8-120">Request headers</span></span>
|<span data-ttu-id="f1cc8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1cc8-121">Header</span></span>|<span data-ttu-id="f1cc8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f1cc8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1cc8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1cc8-123">Authorization</span></span>|<span data-ttu-id="f1cc8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1cc8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1cc8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1cc8-125">Accept</span></span>|<span data-ttu-id="f1cc8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1cc8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1cc8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1cc8-127">Request body</span></span>
<span data-ttu-id="f1cc8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1cc8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1cc8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1cc8-129">Response</span></span>
<span data-ttu-id="f1cc8-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1cc8-130">If successful, this method returns a `200 OK` response code and a collection of [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1cc8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f1cc8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1cc8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1cc8-132">Request</span></span>
<span data-ttu-id="f1cc8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1cc8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleDevices
```

### <a name="response"></a><span data-ttu-id="f1cc8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1cc8-134">Response</span></span>
<span data-ttu-id="f1cc8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1cc8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




