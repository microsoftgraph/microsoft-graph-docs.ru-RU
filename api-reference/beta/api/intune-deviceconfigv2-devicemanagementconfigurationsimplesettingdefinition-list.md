---
title: Список Девицеманажементконфигуратионсимплесеттингдефинитионс
description: Список свойств и связей объектов Девицеманажементконфигуратионсимплесеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 047b5751f5249cacf33a034b4c9d7eb8c59e128b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242456"
---
# <a name="list-devicemanagementconfigurationsimplesettingdefinitions"></a><span data-ttu-id="c3bf0-103">Список Девицеманажементконфигуратионсимплесеттингдефинитионс</span><span class="sxs-lookup"><span data-stu-id="c3bf0-103">List deviceManagementConfigurationSimpleSettingDefinitions</span></span>

<span data-ttu-id="c3bf0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3bf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3bf0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3bf0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3bf0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3bf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3bf0-107">Список свойств и связей объектов [девицеманажементконфигуратионсимплесеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="c3bf0-107">List properties and relationships of the [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3bf0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c3bf0-108">Prerequisites</span></span>
<span data-ttu-id="c3bf0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3bf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3bf0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3bf0-111">Permission type</span></span>|<span data-ttu-id="c3bf0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3bf0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3bf0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3bf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3bf0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3bf0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c3bf0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3bf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3bf0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3bf0-116">Not supported.</span></span>|
|<span data-ttu-id="c3bf0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c3bf0-117">Application</span></span>|<span data-ttu-id="c3bf0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3bf0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3bf0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3bf0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="c3bf0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c3bf0-120">Request headers</span></span>
|<span data-ttu-id="c3bf0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3bf0-121">Header</span></span>|<span data-ttu-id="c3bf0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c3bf0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3bf0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3bf0-123">Authorization</span></span>|<span data-ttu-id="c3bf0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3bf0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3bf0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3bf0-125">Accept</span></span>|<span data-ttu-id="c3bf0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3bf0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3bf0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3bf0-127">Request body</span></span>
<span data-ttu-id="c3bf0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3bf0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3bf0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3bf0-129">Response</span></span>
<span data-ttu-id="c3bf0-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементконфигуратионсимплесеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3bf0-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3bf0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c3bf0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3bf0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3bf0-132">Request</span></span>
<span data-ttu-id="c3bf0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3bf0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationSettings
```

### <a name="response"></a><span data-ttu-id="c3bf0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3bf0-134">Response</span></span>
<span data-ttu-id="c3bf0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3bf0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9857

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingDefinition",
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
      "id": "30dc0613-0613-30dc-1306-dc301306dc30",
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
      ]
    }
  ]
}
```




