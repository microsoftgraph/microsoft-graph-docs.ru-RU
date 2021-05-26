---
title: Обновление deviceManagementConfigurationSettingTemplate
description: Обновление свойств объекта deviceManagementConfigurationSettingTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 98cd26899ec0b2661635dc0758997ecb876cf7d3
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664885"
---
# <a name="update-devicemanagementconfigurationsettingtemplate"></a><span data-ttu-id="b491f-103">Обновление deviceManagementConfigurationSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="b491f-103">Update deviceManagementConfigurationSettingTemplate</span></span>

<span data-ttu-id="b491f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b491f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b491f-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b491f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b491f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b491f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b491f-107">Обновление свойств объекта [deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="b491f-107">Update the properties of a [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b491f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b491f-108">Prerequisites</span></span>
<span data-ttu-id="b491f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b491f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b491f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b491f-111">Permission type</span></span>|<span data-ttu-id="b491f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b491f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b491f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b491f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b491f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b491f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b491f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b491f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b491f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b491f-116">Not supported.</span></span>|
|<span data-ttu-id="b491f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b491f-117">Application</span></span>|<span data-ttu-id="b491f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b491f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b491f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b491f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templateSettings/{deviceManagementConfigurationSettingTemplateId}
PATCH /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="b491f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b491f-120">Request headers</span></span>
|<span data-ttu-id="b491f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b491f-121">Header</span></span>|<span data-ttu-id="b491f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b491f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b491f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b491f-123">Authorization</span></span>|<span data-ttu-id="b491f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b491f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b491f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b491f-125">Accept</span></span>|<span data-ttu-id="b491f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b491f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b491f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b491f-127">Request body</span></span>
<span data-ttu-id="b491f-128">В теле запроса поставляем представление JSON для [объекта deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="b491f-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object.</span></span>

<span data-ttu-id="b491f-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="b491f-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md).</span></span>

|<span data-ttu-id="b491f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b491f-130">Property</span></span>|<span data-ttu-id="b491f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b491f-131">Type</span></span>|<span data-ttu-id="b491f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b491f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b491f-133">id</span><span class="sxs-lookup"><span data-stu-id="b491f-133">id</span></span>|<span data-ttu-id="b491f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b491f-134">String</span></span>|<span data-ttu-id="b491f-135">Ключ этого шаблона параметра в шаблоне политики, который содержит его.</span><span class="sxs-lookup"><span data-stu-id="b491f-135">Key of this setting template within the policy template which contains it.</span></span> <span data-ttu-id="b491f-136">Автоматически созданный.</span><span class="sxs-lookup"><span data-stu-id="b491f-136">Automatically generated.</span></span>|
|<span data-ttu-id="b491f-137">settingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="b491f-137">settingInstanceTemplate</span></span>|[<span data-ttu-id="b491f-138">deviceManagementConfigurationSettingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="b491f-138">deviceManagementConfigurationSettingInstanceTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|<span data-ttu-id="b491f-139">Настройка шаблона экземпляра</span><span class="sxs-lookup"><span data-stu-id="b491f-139">Setting Instance Template</span></span>|



## <a name="response"></a><span data-ttu-id="b491f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b491f-140">Response</span></span>
<span data-ttu-id="b491f-141">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b491f-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b491f-142">Пример</span><span class="sxs-lookup"><span data-stu-id="b491f-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="b491f-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="b491f-143">Request</span></span>
<span data-ttu-id="b491f-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b491f-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templateSettings/{deviceManagementConfigurationSettingTemplateId}
Content-type: application/json
Content-length: 784

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingTemplate",
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
```

### <a name="response"></a><span data-ttu-id="b491f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b491f-145">Response</span></span>
<span data-ttu-id="b491f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b491f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 833

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
```




