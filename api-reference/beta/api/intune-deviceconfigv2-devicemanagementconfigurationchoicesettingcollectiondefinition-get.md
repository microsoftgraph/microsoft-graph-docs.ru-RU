---
title: Get deviceManagementConfigurationChoiceSettingCollectionDefinition
description: Чтение свойств и связей объекта deviceManagementConfigurationChoiceSettingCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: beaffbca71cdfd85602cc56ee33fd544460d8d07
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136813"
---
# <a name="get-devicemanagementconfigurationchoicesettingcollectiondefinition"></a><span data-ttu-id="db5b5-103">Get deviceManagementConfigurationChoiceSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="db5b5-103">Get deviceManagementConfigurationChoiceSettingCollectionDefinition</span></span>

<span data-ttu-id="db5b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db5b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db5b5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db5b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db5b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db5b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db5b5-107">Чтение свойств и связей [объекта deviceManagementConfigurationChoiceSettingCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="db5b5-107">Read properties and relationships of the [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db5b5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="db5b5-108">Prerequisites</span></span>
<span data-ttu-id="db5b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db5b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db5b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db5b5-111">Permission type</span></span>|<span data-ttu-id="db5b5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db5b5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db5b5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db5b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db5b5-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5b5-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db5b5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db5b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db5b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db5b5-116">Not supported.</span></span>|
|<span data-ttu-id="db5b5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="db5b5-117">Application</span></span>|<span data-ttu-id="db5b5-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5b5-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db5b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db5b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db5b5-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="db5b5-120">Optional query parameters</span></span>
<span data-ttu-id="db5b5-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="db5b5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db5b5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db5b5-122">Request headers</span></span>
|<span data-ttu-id="db5b5-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db5b5-123">Header</span></span>|<span data-ttu-id="db5b5-124">Значение</span><span class="sxs-lookup"><span data-stu-id="db5b5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db5b5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="db5b5-125">Authorization</span></span>|<span data-ttu-id="db5b5-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db5b5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db5b5-127">Accept</span><span class="sxs-lookup"><span data-stu-id="db5b5-127">Accept</span></span>|<span data-ttu-id="db5b5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="db5b5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db5b5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db5b5-129">Request body</span></span>
<span data-ttu-id="db5b5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db5b5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db5b5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="db5b5-131">Response</span></span>
<span data-ttu-id="db5b5-132">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [объект deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="db5b5-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db5b5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="db5b5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="db5b5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="db5b5-134">Request</span></span>
<span data-ttu-id="db5b5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db5b5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="db5b5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="db5b5-136">Response</span></span>
<span data-ttu-id="db5b5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db5b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10414

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionDefinition",
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
    "id": "eb03fdca-fdca-eb03-cafd-03ebcafd03eb",
    "description": "Description value",
    "helpText": "Help Text value",
    "name": "Name value",
    "displayName": "Display Name value",
    "version": "Version value",
    "options": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition",
        "optionValue": {
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
        "itemId": "Item Id value",
        "description": "Description value",
        "helpText": "Help Text value",
        "name": "Name value",
        "displayName": "Display Name value"
      }
    ],
    "defaultOptionId": "Default Option Id value",
    "maximumCount": 12,
    "minimumCount": 12
  }
}
```




