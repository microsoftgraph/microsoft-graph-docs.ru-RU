---
title: Список deviceManagementReusablePolicySettings
description: Список свойств и связей объектов deviceManagementReusablePolicySetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 849283d79fb7a0cb867143e90b074131ad1d7171
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869150"
---
# <a name="list-devicemanagementreusablepolicysettings"></a><span data-ttu-id="8232f-103">Список deviceManagementReusablePolicySettings</span><span class="sxs-lookup"><span data-stu-id="8232f-103">List deviceManagementReusablePolicySettings</span></span>

<span data-ttu-id="8232f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8232f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8232f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8232f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8232f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8232f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8232f-107">Список свойств и связей [объектов deviceManagementReusablePolicySetting.](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)</span><span class="sxs-lookup"><span data-stu-id="8232f-107">List properties and relationships of the [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8232f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8232f-108">Prerequisites</span></span>
<span data-ttu-id="8232f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8232f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8232f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8232f-111">Permission type</span></span>|<span data-ttu-id="8232f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8232f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8232f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8232f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8232f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8232f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8232f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8232f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8232f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8232f-116">Not supported.</span></span>|
|<span data-ttu-id="8232f-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8232f-117">Application</span></span>|<span data-ttu-id="8232f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8232f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8232f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8232f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reusablePolicySettings
```

## <a name="request-headers"></a><span data-ttu-id="8232f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8232f-120">Request headers</span></span>
|<span data-ttu-id="8232f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8232f-121">Header</span></span>|<span data-ttu-id="8232f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8232f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8232f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8232f-123">Authorization</span></span>|<span data-ttu-id="8232f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8232f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8232f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8232f-125">Accept</span></span>|<span data-ttu-id="8232f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8232f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8232f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8232f-127">Request body</span></span>
<span data-ttu-id="8232f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8232f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8232f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8232f-129">Response</span></span>
<span data-ttu-id="8232f-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8232f-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8232f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8232f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8232f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8232f-132">Request</span></span>
<span data-ttu-id="8232f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8232f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reusablePolicySettings
```

### <a name="response"></a><span data-ttu-id="8232f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8232f-134">Response</span></span>
<span data-ttu-id="8232f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8232f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8589

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementReusablePolicySetting",
      "id": "7a4f9bd7-9bd7-7a4f-d79b-4f7ad79b4f7a",
      "displayName": "Display Name value",
      "description": "Description value",
      "settingDefinitionId": "Setting Definition Id value",
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
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "referencingConfigurationPolicyCount": 3
    }
  ]
}
```




