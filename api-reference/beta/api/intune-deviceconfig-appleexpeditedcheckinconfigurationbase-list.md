---
title: Список Аппликспедитедчеккинконфигуратионбасес
description: Список свойств и связей объектов Аппликспедитедчеккинконфигуратионбасе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1ef6636df3acae0f1dae5dd4ef40d2ab88852d22
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722734"
---
# <a name="list-appleexpeditedcheckinconfigurationbases"></a><span data-ttu-id="eef69-103">Список Аппликспедитедчеккинконфигуратионбасес</span><span class="sxs-lookup"><span data-stu-id="eef69-103">List appleExpeditedCheckinConfigurationBases</span></span>

<span data-ttu-id="eef69-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eef69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eef69-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eef69-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eef69-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eef69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eef69-107">Список свойств и связей объектов [аппликспедитедчеккинконфигуратионбасе](../resources/intune-deviceconfig-appleexpeditedcheckinconfigurationbase.md) .</span><span class="sxs-lookup"><span data-stu-id="eef69-107">List properties and relationships of the [appleExpeditedCheckinConfigurationBase](../resources/intune-deviceconfig-appleexpeditedcheckinconfigurationbase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eef69-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eef69-108">Prerequisites</span></span>
<span data-ttu-id="eef69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eef69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eef69-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eef69-111">Permission type</span></span>|<span data-ttu-id="eef69-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eef69-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eef69-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eef69-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eef69-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef69-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eef69-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eef69-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eef69-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eef69-116">Not supported.</span></span>|
|<span data-ttu-id="eef69-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eef69-117">Application</span></span>|<span data-ttu-id="eef69-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef69-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eef69-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eef69-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="eef69-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eef69-120">Request headers</span></span>
|<span data-ttu-id="eef69-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eef69-121">Header</span></span>|<span data-ttu-id="eef69-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eef69-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eef69-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eef69-123">Authorization</span></span>|<span data-ttu-id="eef69-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eef69-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eef69-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eef69-125">Accept</span></span>|<span data-ttu-id="eef69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eef69-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eef69-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eef69-127">Request body</span></span>
<span data-ttu-id="eef69-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eef69-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eef69-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="eef69-129">Response</span></span>
<span data-ttu-id="eef69-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аппликспедитедчеккинконфигуратионбасе](../resources/intune-deviceconfig-appleexpeditedcheckinconfigurationbase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eef69-130">If successful, this method returns a `200 OK` response code and a collection of [appleExpeditedCheckinConfigurationBase](../resources/intune-deviceconfig-appleexpeditedcheckinconfigurationbase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eef69-131">Пример</span><span class="sxs-lookup"><span data-stu-id="eef69-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="eef69-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="eef69-132">Request</span></span>
<span data-ttu-id="eef69-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eef69-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="eef69-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="eef69-134">Response</span></span>
<span data-ttu-id="eef69-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eef69-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1413

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleExpeditedCheckinConfigurationBase",
      "id": "5fdd79cd-79cd-5fdd-cd79-dd5fcd79dd5f",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "enableExpeditedCheckin": true
    }
  ]
}
```





