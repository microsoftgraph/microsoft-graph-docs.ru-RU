---
title: Создание deviceManagementConfigurationSettingTemplate
description: Создайте новый объект deviceManagementConfigurationSettingTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75e4f8bdb6cfa6761daf29695cb64d2b04425840
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666091"
---
# <a name="create-devicemanagementconfigurationsettingtemplate"></a><span data-ttu-id="14b81-103">Создание deviceManagementConfigurationSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="14b81-103">Create deviceManagementConfigurationSettingTemplate</span></span>

<span data-ttu-id="14b81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14b81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14b81-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14b81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14b81-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14b81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14b81-107">Создайте новый [объект deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="14b81-107">Create a new [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14b81-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="14b81-108">Prerequisites</span></span>
<span data-ttu-id="14b81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14b81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14b81-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14b81-111">Permission type</span></span>|<span data-ttu-id="14b81-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14b81-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14b81-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14b81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14b81-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b81-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14b81-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14b81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14b81-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14b81-116">Not supported.</span></span>|
|<span data-ttu-id="14b81-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="14b81-117">Application</span></span>|<span data-ttu-id="14b81-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b81-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14b81-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14b81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templateSettings
POST /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates
```

## <a name="request-headers"></a><span data-ttu-id="14b81-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="14b81-120">Request headers</span></span>
|<span data-ttu-id="14b81-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14b81-121">Header</span></span>|<span data-ttu-id="14b81-122">Значение</span><span class="sxs-lookup"><span data-stu-id="14b81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14b81-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14b81-123">Authorization</span></span>|<span data-ttu-id="14b81-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14b81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14b81-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14b81-125">Accept</span></span>|<span data-ttu-id="14b81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14b81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14b81-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14b81-127">Request body</span></span>
<span data-ttu-id="14b81-128">В теле запроса поставляем представление JSON для объекта deviceManagementConfigurationSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="14b81-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingTemplate object.</span></span>

<span data-ttu-id="14b81-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementConfigurationSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="14b81-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingTemplate.</span></span>

|<span data-ttu-id="14b81-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="14b81-130">Property</span></span>|<span data-ttu-id="14b81-131">Тип</span><span class="sxs-lookup"><span data-stu-id="14b81-131">Type</span></span>|<span data-ttu-id="14b81-132">Описание</span><span class="sxs-lookup"><span data-stu-id="14b81-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14b81-133">id</span><span class="sxs-lookup"><span data-stu-id="14b81-133">id</span></span>|<span data-ttu-id="14b81-134">Строка</span><span class="sxs-lookup"><span data-stu-id="14b81-134">String</span></span>|<span data-ttu-id="14b81-135">Ключ этого шаблона параметра в шаблоне политики, который содержит его.</span><span class="sxs-lookup"><span data-stu-id="14b81-135">Key of this setting template within the policy template which contains it.</span></span> <span data-ttu-id="14b81-136">Автоматически созданный.</span><span class="sxs-lookup"><span data-stu-id="14b81-136">Automatically generated.</span></span>|
|<span data-ttu-id="14b81-137">settingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="14b81-137">settingInstanceTemplate</span></span>|[<span data-ttu-id="14b81-138">deviceManagementConfigurationSettingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="14b81-138">deviceManagementConfigurationSettingInstanceTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|<span data-ttu-id="14b81-139">Настройка шаблона экземпляра</span><span class="sxs-lookup"><span data-stu-id="14b81-139">Setting Instance Template</span></span>|



## <a name="response"></a><span data-ttu-id="14b81-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="14b81-140">Response</span></span>
<span data-ttu-id="14b81-141">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="14b81-141">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14b81-142">Пример</span><span class="sxs-lookup"><span data-stu-id="14b81-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="14b81-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="14b81-143">Request</span></span>
<span data-ttu-id="14b81-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14b81-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templateSettings
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

### <a name="response"></a><span data-ttu-id="14b81-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="14b81-145">Response</span></span>
<span data-ttu-id="14b81-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14b81-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




