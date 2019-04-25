---
title: Перечисление объектов settingStateDeviceSummary
description: Список свойств и связей объектов settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89fc1df7d1951650e36df2f8e2a367654a6c96d0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572593"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="7c29e-103">Перечисление объектов settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="7c29e-103">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="7c29e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c29e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c29e-105">Список свойств и связей объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7c29e-105">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c29e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7c29e-106">Prerequisites</span></span>
<span data-ttu-id="7c29e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c29e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c29e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c29e-109">Permission type</span></span>|<span data-ttu-id="7c29e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c29e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c29e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c29e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7c29e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c29e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7c29e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c29e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c29e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c29e-114">Not supported.</span></span>|
|<span data-ttu-id="7c29e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c29e-115">Application</span></span>|<span data-ttu-id="7c29e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c29e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c29e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c29e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="7c29e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c29e-118">Request headers</span></span>
|<span data-ttu-id="7c29e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c29e-119">Header</span></span>|<span data-ttu-id="7c29e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7c29e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c29e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c29e-121">Authorization</span></span>|<span data-ttu-id="7c29e-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c29e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c29e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7c29e-123">Accept</span></span>|<span data-ttu-id="7c29e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7c29e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c29e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c29e-125">Request body</span></span>
<span data-ttu-id="7c29e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c29e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c29e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c29e-127">Response</span></span>
<span data-ttu-id="7c29e-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c29e-128">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c29e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7c29e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c29e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c29e-130">Request</span></span>
<span data-ttu-id="7c29e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c29e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="7c29e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c29e-132">Response</span></span>
<span data-ttu-id="7c29e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c29e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
      "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
      "settingName": "Setting Name value",
      "instancePath": "Instance Path value",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```



