---
title: Список Девицеманажементконфигуратионсеттингс
description: Список свойств и связей объектов Девицеманажементконфигуратионсеттинг.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa45febac14a96fcb2b8c77564da7d34dcbf9b15
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242595"
---
# <a name="list-devicemanagementconfigurationsettings"></a><span data-ttu-id="b7edd-103">Список Девицеманажементконфигуратионсеттингс</span><span class="sxs-lookup"><span data-stu-id="b7edd-103">List deviceManagementConfigurationSettings</span></span>

<span data-ttu-id="b7edd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7edd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7edd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7edd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7edd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7edd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7edd-107">Список свойств и связей объектов [девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="b7edd-107">List properties and relationships of the [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7edd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b7edd-108">Prerequisites</span></span>
<span data-ttu-id="b7edd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7edd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7edd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7edd-111">Permission type</span></span>|<span data-ttu-id="b7edd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7edd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7edd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7edd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7edd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7edd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b7edd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7edd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7edd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7edd-116">Not supported.</span></span>|
|<span data-ttu-id="b7edd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b7edd-117">Application</span></span>|<span data-ttu-id="b7edd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7edd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7edd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7edd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings
```

## <a name="request-headers"></a><span data-ttu-id="b7edd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b7edd-120">Request headers</span></span>
|<span data-ttu-id="b7edd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7edd-121">Header</span></span>|<span data-ttu-id="b7edd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b7edd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7edd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7edd-123">Authorization</span></span>|<span data-ttu-id="b7edd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7edd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7edd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b7edd-125">Accept</span></span>|<span data-ttu-id="b7edd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7edd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7edd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7edd-127">Request body</span></span>
<span data-ttu-id="b7edd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7edd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7edd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7edd-129">Response</span></span>
<span data-ttu-id="b7edd-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7edd-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7edd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b7edd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7edd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7edd-132">Request</span></span>
<span data-ttu-id="b7edd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7edd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings
```

### <a name="response"></a><span data-ttu-id="b7edd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7edd-134">Response</span></span>
<span data-ttu-id="b7edd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7edd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




