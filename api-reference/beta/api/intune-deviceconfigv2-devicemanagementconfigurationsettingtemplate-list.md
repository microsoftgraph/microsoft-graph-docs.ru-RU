---
title: Список deviceManagementConfigurationSettingTemplates
description: Список свойств и связей объектов deviceManagementConfigurationSettingTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 99591f65be18681cdd02cd9b8f4f77557cd374a5
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664886"
---
# <a name="list-devicemanagementconfigurationsettingtemplates"></a><span data-ttu-id="87062-103">Список deviceManagementConfigurationSettingTemplates</span><span class="sxs-lookup"><span data-stu-id="87062-103">List deviceManagementConfigurationSettingTemplates</span></span>

<span data-ttu-id="87062-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87062-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87062-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87062-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87062-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87062-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87062-107">Список свойств и связей [объектов deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="87062-107">List properties and relationships of the [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87062-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="87062-108">Prerequisites</span></span>
<span data-ttu-id="87062-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87062-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87062-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87062-111">Permission type</span></span>|<span data-ttu-id="87062-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87062-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87062-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87062-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87062-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87062-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87062-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87062-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87062-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87062-116">Not supported.</span></span>|
|<span data-ttu-id="87062-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="87062-117">Application</span></span>|<span data-ttu-id="87062-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87062-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87062-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87062-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templateSettings
GET /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates
```

## <a name="request-headers"></a><span data-ttu-id="87062-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="87062-120">Request headers</span></span>
|<span data-ttu-id="87062-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87062-121">Header</span></span>|<span data-ttu-id="87062-122">Значение</span><span class="sxs-lookup"><span data-stu-id="87062-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87062-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87062-123">Authorization</span></span>|<span data-ttu-id="87062-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87062-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87062-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87062-125">Accept</span></span>|<span data-ttu-id="87062-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87062-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87062-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87062-127">Request body</span></span>
<span data-ttu-id="87062-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87062-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87062-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="87062-129">Response</span></span>
<span data-ttu-id="87062-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию `200 OK` [объектов deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="87062-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87062-131">Пример</span><span class="sxs-lookup"><span data-stu-id="87062-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="87062-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="87062-132">Request</span></span>
<span data-ttu-id="87062-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87062-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templateSettings
```

### <a name="response"></a><span data-ttu-id="87062-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="87062-134">Response</span></span>
<span data-ttu-id="87062-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87062-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 930

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingTemplate",
      "id": "203fd028-d028-203f-28d0-3f2028d03f20",
      "settingInstanceTemplate": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
        "settingInstanceTemplateId": "Setting Instance Template Id value",
        "settingDefinitionId": "Setting Definition Id value",
        "isRequired": true,
        "simpleSettingValueTemplate": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
          "settingValueTemplateId": "Setting Value Template Id value",
          "defaultValue": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
            "constantValue": "Constant Value value"
          }
        }
      }
    }
  ]
}
```




