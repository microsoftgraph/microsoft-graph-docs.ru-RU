---
title: Список deviceManagementConfigurationSimpleSettingCollectionDefinitions
description: Список свойств и связей объектов deviceManagementConfigurationSimpleSettingCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b401869a2e9370199d19ffe7be78e33643e2bd8
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867891"
---
# <a name="list-devicemanagementconfigurationsimplesettingcollectiondefinitions"></a><span data-ttu-id="82b38-103">Список deviceManagementConfigurationSimpleSettingCollectionDefinitions</span><span class="sxs-lookup"><span data-stu-id="82b38-103">List deviceManagementConfigurationSimpleSettingCollectionDefinitions</span></span>

<span data-ttu-id="82b38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82b38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82b38-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82b38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82b38-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82b38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82b38-107">Список свойств и связей [объектов deviceManagementConfigurationSimpleSettingCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="82b38-107">List properties and relationships of the [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82b38-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="82b38-108">Prerequisites</span></span>
<span data-ttu-id="82b38-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82b38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82b38-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82b38-111">Permission type</span></span>|<span data-ttu-id="82b38-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82b38-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82b38-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82b38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82b38-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82b38-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82b38-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82b38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82b38-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82b38-116">Not supported.</span></span>|
|<span data-ttu-id="82b38-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="82b38-117">Application</span></span>|<span data-ttu-id="82b38-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82b38-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82b38-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82b38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reusableSettings
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="82b38-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="82b38-120">Request headers</span></span>
|<span data-ttu-id="82b38-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82b38-121">Header</span></span>|<span data-ttu-id="82b38-122">Значение</span><span class="sxs-lookup"><span data-stu-id="82b38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82b38-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82b38-123">Authorization</span></span>|<span data-ttu-id="82b38-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82b38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82b38-125">Accept</span><span class="sxs-lookup"><span data-stu-id="82b38-125">Accept</span></span>|<span data-ttu-id="82b38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82b38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82b38-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82b38-127">Request body</span></span>
<span data-ttu-id="82b38-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82b38-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82b38-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="82b38-129">Response</span></span>
<span data-ttu-id="82b38-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию `200 OK` [объектов deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="82b38-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82b38-131">Пример</span><span class="sxs-lookup"><span data-stu-id="82b38-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="82b38-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="82b38-132">Request</span></span>
<span data-ttu-id="82b38-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82b38-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reusableSettings
```

### <a name="response"></a><span data-ttu-id="82b38-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="82b38-134">Response</span></span>
<span data-ttu-id="82b38-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82b38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10234

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionDefinition",
      "applicability": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
        "description": "Description value",
        "platform": "macOS",
        "deviceMode": "kiosk",
        "technologies": "mdm"
      },
      "accessTypes": "add",
      "keywords": [
        "Keywords value"
      ],
      "infoUrls": [
        "Info Urls value"
      ],
      "occurrence": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
        "minDeviceOccurrence": 3,
        "maxDeviceOccurrence": 3
      },
      "baseUri": "Base Uri value",
      "offsetUri": "Offset Uri value",
      "rootDefinitionId": "Root Definition Id value",
      "categoryId": "Category Id value",
      "settingUsage": "configuration",
      "uxBehavior": "dropdown",
      "visibility": "settingsCatalog",
      "referredSettingInformationList": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
          "settingDefinitionId": "Setting Definition Id value"
        }
      ],
      "id": "cb4abda1-bda1-cb4a-a1bd-4acba1bd4acb",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value",
      "version": "Version value",
      "valueDefinition": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueDefinition"
      },
      "defaultValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
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
                                                                        "settingDefinitionId": "Setting Definition Id value",
                                                                        "choiceSettingValue": {
                                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                          "value": "Value value",
                                                                          "children": null
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
        ]
      },
      "dependentOn": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
          "dependentOn": "Dependent On value",
          "parentSettingId": "Parent Setting Id value"
        }
      ],
      "dependedOnBy": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
          "dependedOnBy": "Depended On By value",
          "required": true
        }
      ],
      "maximumCount": 12,
      "minimumCount": 12
    }
  ]
}
```




