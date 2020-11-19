---
title: Список Девицеманажементконфигуратионполициассигнментс
description: Список свойств и связей объектов Девицеманажементконфигуратионполициассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76298793f4cfb31321cf28bab3860be5236d34c9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302167"
---
# <a name="list-devicemanagementconfigurationpolicyassignments"></a><span data-ttu-id="83554-103">Список Девицеманажементконфигуратионполициассигнментс</span><span class="sxs-lookup"><span data-stu-id="83554-103">List deviceManagementConfigurationPolicyAssignments</span></span>

<span data-ttu-id="83554-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83554-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83554-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83554-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83554-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83554-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83554-107">Список свойств и связей объектов [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="83554-107">List properties and relationships of the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83554-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="83554-108">Prerequisites</span></span>
<span data-ttu-id="83554-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83554-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83554-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83554-111">Permission type</span></span>|<span data-ttu-id="83554-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83554-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83554-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83554-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83554-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="83554-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="83554-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83554-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83554-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83554-116">Not supported.</span></span>|
|<span data-ttu-id="83554-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83554-117">Application</span></span>|<span data-ttu-id="83554-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="83554-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83554-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83554-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="83554-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="83554-120">Request headers</span></span>
|<span data-ttu-id="83554-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83554-121">Header</span></span>|<span data-ttu-id="83554-122">Значение</span><span class="sxs-lookup"><span data-stu-id="83554-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83554-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83554-123">Authorization</span></span>|<span data-ttu-id="83554-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83554-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83554-125">Accept</span><span class="sxs-lookup"><span data-stu-id="83554-125">Accept</span></span>|<span data-ttu-id="83554-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83554-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83554-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83554-127">Request body</span></span>
<span data-ttu-id="83554-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="83554-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83554-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="83554-129">Response</span></span>
<span data-ttu-id="83554-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83554-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83554-131">Пример</span><span class="sxs-lookup"><span data-stu-id="83554-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="83554-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="83554-132">Request</span></span>
<span data-ttu-id="83554-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83554-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="83554-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="83554-134">Response</span></span>
<span data-ttu-id="83554-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83554-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
      "id": "1f069921-9921-1f06-2199-061f2199061f",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```




