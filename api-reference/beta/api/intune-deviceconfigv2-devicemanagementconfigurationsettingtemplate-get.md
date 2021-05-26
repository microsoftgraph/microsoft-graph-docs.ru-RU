---
title: Get deviceManagementConfigurationSettingTemplate
description: Чтение свойств и связей объекта deviceManagementConfigurationSettingTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0ffa4a5fdaf5c1821f0a34d80e17314725dfeaa6
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666083"
---
# <a name="get-devicemanagementconfigurationsettingtemplate"></a><span data-ttu-id="1b9e6-103">Get deviceManagementConfigurationSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="1b9e6-103">Get deviceManagementConfigurationSettingTemplate</span></span>

<span data-ttu-id="1b9e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b9e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b9e6-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b9e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b9e6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b9e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b9e6-107">Чтение свойств и связей [объекта deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="1b9e6-107">Read properties and relationships of the [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b9e6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1b9e6-108">Prerequisites</span></span>
<span data-ttu-id="1b9e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b9e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b9e6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b9e6-111">Permission type</span></span>|<span data-ttu-id="1b9e6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b9e6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b9e6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b9e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b9e6-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b9e6-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b9e6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b9e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b9e6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b9e6-116">Not supported.</span></span>|
|<span data-ttu-id="1b9e6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1b9e6-117">Application</span></span>|<span data-ttu-id="1b9e6-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b9e6-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b9e6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b9e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templateSettings/{deviceManagementConfigurationSettingTemplateId}
GET /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b9e6-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1b9e6-120">Optional query parameters</span></span>
<span data-ttu-id="1b9e6-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1b9e6-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b9e6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b9e6-122">Request headers</span></span>
|<span data-ttu-id="1b9e6-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b9e6-123">Header</span></span>|<span data-ttu-id="1b9e6-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1b9e6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b9e6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b9e6-125">Authorization</span></span>|<span data-ttu-id="1b9e6-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b9e6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b9e6-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1b9e6-127">Accept</span></span>|<span data-ttu-id="1b9e6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1b9e6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b9e6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b9e6-129">Request body</span></span>
<span data-ttu-id="1b9e6-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b9e6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b9e6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b9e6-131">Response</span></span>
<span data-ttu-id="1b9e6-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b9e6-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b9e6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1b9e6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b9e6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b9e6-134">Request</span></span>
<span data-ttu-id="1b9e6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b9e6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templateSettings/{deviceManagementConfigurationSettingTemplateId}
```

### <a name="response"></a><span data-ttu-id="1b9e6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b9e6-136">Response</span></span>
<span data-ttu-id="1b9e6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b9e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 884

{
  "value": {
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
}
```




