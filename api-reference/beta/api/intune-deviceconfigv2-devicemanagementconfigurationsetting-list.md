---
title: Список deviceManagementConfigurationSettings
description: Список свойств и связей объектов deviceManagementConfigurationSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db37ba69e5dc541543258b06a332b9fe139b6599
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146974"
---
# <a name="list-devicemanagementconfigurationsettings"></a><span data-ttu-id="496a9-103">Список deviceManagementConfigurationSettings</span><span class="sxs-lookup"><span data-stu-id="496a9-103">List deviceManagementConfigurationSettings</span></span>

<span data-ttu-id="496a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="496a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="496a9-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="496a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="496a9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="496a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="496a9-107">Список свойств и связей [объектов deviceManagementConfigurationSetting.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)</span><span class="sxs-lookup"><span data-stu-id="496a9-107">List properties and relationships of the [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="496a9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="496a9-108">Prerequisites</span></span>
<span data-ttu-id="496a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="496a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="496a9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="496a9-111">Permission type</span></span>|<span data-ttu-id="496a9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="496a9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="496a9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="496a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="496a9-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="496a9-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="496a9-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="496a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="496a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="496a9-116">Not supported.</span></span>|
|<span data-ttu-id="496a9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="496a9-117">Application</span></span>|<span data-ttu-id="496a9-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="496a9-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="496a9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="496a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings
```

## <a name="request-headers"></a><span data-ttu-id="496a9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="496a9-120">Request headers</span></span>
|<span data-ttu-id="496a9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="496a9-121">Header</span></span>|<span data-ttu-id="496a9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="496a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="496a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="496a9-123">Authorization</span></span>|<span data-ttu-id="496a9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="496a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="496a9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="496a9-125">Accept</span></span>|<span data-ttu-id="496a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="496a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="496a9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="496a9-127">Request body</span></span>
<span data-ttu-id="496a9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="496a9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="496a9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="496a9-129">Response</span></span>
<span data-ttu-id="496a9-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию `200 OK` [объектов deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="496a9-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="496a9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="496a9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="496a9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="496a9-132">Request</span></span>
<span data-ttu-id="496a9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="496a9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings
```

### <a name="response"></a><span data-ttu-id="496a9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="496a9-134">Response</span></span>
<span data-ttu-id="496a9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="496a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8239

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationSetting",
      "id": "9acf977e-977e-9acf-7e97-cf9a7e97cf9a",
      "settingInstance": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
        "settingDefinitionId": "Setting Definition Id value",
        "choiceSettingValue": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
          "value": "Value value",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
              "settingDefinitionId": "Setting Definition Id value",
              "choiceSettingValue": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                "value": "Value value",
                "children": [
                  {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                    "settingDefinitionId": "Setting Definition Id value",
                    "choiceSettingValue": {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                      "value": "Value value",
                      "children": [
                        {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                          "settingDefinitionId": "Setting Definition Id value",
                          "choiceSettingValue": {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                            "value": "Value value",
                            "children": [
                              {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                "settingDefinitionId": "Setting Definition Id value",
                                "choiceSettingValue": {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                  "value": "Value value",
                                  "children": [
                                    {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                      "settingDefinitionId": "Setting Definition Id value",
                                      "choiceSettingValue": {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                        "value": "Value value",
                                        "children": [
                                          {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                            "settingDefinitionId": "Setting Definition Id value",
                                            "choiceSettingValue": {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                              "value": "Value value",
                                              "children": [
                                                {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                  "settingDefinitionId": "Setting Definition Id value",
                                                  "choiceSettingValue": {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                    "value": "Value value",
                                                    "children": [
                                                      {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                        "settingDefinitionId": "Setting Definition Id value",
                                                        "choiceSettingValue": {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                          "value": "Value value",
                                                          "children": [
                                                            {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                              "settingDefinitionId": "Setting Definition Id value",
                                                              "choiceSettingValue": {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                "value": "Value value",
                                                                "children": [
                                                                  {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                    "settingDefinitionId": "Setting Definition Id value",
                                                                    "choiceSettingValue": {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                      "value": "Value value",
                                                                      "children": [
                                                                        {
                                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                          "settingDefinitionId": null,
                                                                          "choiceSettingValue": null
                                                                        }
                                                                      ]
                                                                    }
                                                                  }
                                                                ]
                                                              }
                                                            }
                                                          ]
                                                        }
                                                      }
                                                    ]
                                                  }
                                                }
                                              ]
                                            }
                                          }
                                        ]
                                      }
                                    }
                                  ]
                                }
                              }
                            ]
                          }
                        }
                      ]
                    }
                  }
                ]
              }
            }
          ]
        }
      }
    }
  ]
}
```




