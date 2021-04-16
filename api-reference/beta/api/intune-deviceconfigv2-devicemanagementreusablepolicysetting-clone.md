---
title: действие клона
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1170cb9aa5854b1f4548b69c38252793fc05324b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869049"
---
# <a name="clone-action"></a><span data-ttu-id="b3ac1-103">действие клона</span><span class="sxs-lookup"><span data-stu-id="b3ac1-103">clone action</span></span>

<span data-ttu-id="b3ac1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3ac1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3ac1-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3ac1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3ac1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3ac1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3ac1-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b3ac1-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3ac1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b3ac1-108">Prerequisites</span></span>
<span data-ttu-id="b3ac1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3ac1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3ac1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3ac1-111">Permission type</span></span>|<span data-ttu-id="b3ac1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3ac1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3ac1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3ac1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3ac1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3ac1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3ac1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3ac1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3ac1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3ac1-116">Not supported.</span></span>|
|<span data-ttu-id="b3ac1-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b3ac1-117">Application</span></span>|<span data-ttu-id="b3ac1-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3ac1-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3ac1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3ac1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/clone
```

## <a name="request-headers"></a><span data-ttu-id="b3ac1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b3ac1-120">Request headers</span></span>
|<span data-ttu-id="b3ac1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3ac1-121">Header</span></span>|<span data-ttu-id="b3ac1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b3ac1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3ac1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3ac1-123">Authorization</span></span>|<span data-ttu-id="b3ac1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3ac1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3ac1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3ac1-125">Accept</span></span>|<span data-ttu-id="b3ac1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3ac1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3ac1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3ac1-127">Request body</span></span>
<span data-ttu-id="b3ac1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3ac1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3ac1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3ac1-129">Response</span></span>
<span data-ttu-id="b3ac1-130">В случае успешного выполнения это действие возвращает код отклика и `200 OK` [устройствоManagementReusablePolicySetting в](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b3ac1-130">If successful, this action returns a `200 OK` response code and a [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3ac1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b3ac1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3ac1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3ac1-132">Request</span></span>
<span data-ttu-id="b3ac1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3ac1-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/clone
```

### <a name="response"></a><span data-ttu-id="b3ac1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3ac1-134">Response</span></span>
<span data-ttu-id="b3ac1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3ac1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8302

{
  "value": {
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
                                                                  "settingDefinitionId": null,
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
}
```




