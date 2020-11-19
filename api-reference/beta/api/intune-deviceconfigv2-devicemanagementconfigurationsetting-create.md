---
title: Создание Девицеманажементконфигуратионсеттинг
description: Создание нового объекта Девицеманажементконфигуратионсеттинг.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 981e1e22f670bcb3d703b1dd30623ad264c7a8bd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242601"
---
# <a name="create-devicemanagementconfigurationsetting"></a><span data-ttu-id="9b38b-103">Создание Девицеманажементконфигуратионсеттинг</span><span class="sxs-lookup"><span data-stu-id="9b38b-103">Create deviceManagementConfigurationSetting</span></span>

<span data-ttu-id="9b38b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b38b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b38b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b38b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b38b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b38b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b38b-107">Создание нового объекта [девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="9b38b-107">Create a new [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b38b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9b38b-108">Prerequisites</span></span>
<span data-ttu-id="9b38b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b38b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b38b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b38b-111">Permission type</span></span>|<span data-ttu-id="9b38b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b38b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b38b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b38b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b38b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b38b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b38b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b38b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b38b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b38b-116">Not supported.</span></span>|
|<span data-ttu-id="9b38b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9b38b-117">Application</span></span>|<span data-ttu-id="9b38b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b38b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b38b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b38b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings
```

## <a name="request-headers"></a><span data-ttu-id="9b38b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9b38b-120">Request headers</span></span>
|<span data-ttu-id="9b38b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b38b-121">Header</span></span>|<span data-ttu-id="9b38b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9b38b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b38b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b38b-123">Authorization</span></span>|<span data-ttu-id="9b38b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b38b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b38b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9b38b-125">Accept</span></span>|<span data-ttu-id="9b38b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b38b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b38b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b38b-127">Request body</span></span>
<span data-ttu-id="9b38b-128">В тексте запроса добавьте представление объекта Девицеманажементконфигуратионсеттинг в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b38b-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSetting object.</span></span>

<span data-ttu-id="9b38b-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементконфигуратионсеттинг.</span><span class="sxs-lookup"><span data-stu-id="9b38b-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSetting.</span></span>

|<span data-ttu-id="9b38b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b38b-130">Property</span></span>|<span data-ttu-id="9b38b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9b38b-131">Type</span></span>|<span data-ttu-id="9b38b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9b38b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b38b-133">id</span><span class="sxs-lookup"><span data-stu-id="9b38b-133">id</span></span>|<span data-ttu-id="9b38b-134">String</span><span class="sxs-lookup"><span data-stu-id="9b38b-134">String</span></span>|<span data-ttu-id="9b38b-135">Ключ этого параметра в политике, которая содержит его.</span><span class="sxs-lookup"><span data-stu-id="9b38b-135">Key of this setting within the policy which contains it.</span></span> <span data-ttu-id="9b38b-136">Создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="9b38b-136">Automatically generated.</span></span>|
|<span data-ttu-id="9b38b-137">сеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="9b38b-137">settingInstance</span></span>|[<span data-ttu-id="9b38b-138">девицеманажементконфигуратионсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="9b38b-138">deviceManagementConfigurationSettingInstance</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|<span data-ttu-id="9b38b-139">Установка экземпляра</span><span class="sxs-lookup"><span data-stu-id="9b38b-139">Setting Instance</span></span>|



## <a name="response"></a><span data-ttu-id="9b38b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b38b-140">Response</span></span>
<span data-ttu-id="9b38b-141">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b38b-141">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b38b-142">Пример</span><span class="sxs-lookup"><span data-stu-id="9b38b-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b38b-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b38b-143">Request</span></span>
<span data-ttu-id="9b38b-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b38b-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings
Content-type: application/json
Content-length: 7689

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSetting",
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
```

### <a name="response"></a><span data-ttu-id="9b38b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b38b-145">Response</span></span>
<span data-ttu-id="9b38b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b38b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7738

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
```




