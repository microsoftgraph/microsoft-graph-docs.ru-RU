---
title: Создание deviceManagementReusablePolicySetting
description: Создание нового объекта deviceManagementReusablePolicySetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 146dfbe24f2380f639ec7715c9ab7cb3278191da
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869161"
---
# <a name="create-devicemanagementreusablepolicysetting"></a><span data-ttu-id="657da-103">Создание deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="657da-103">Create deviceManagementReusablePolicySetting</span></span>

<span data-ttu-id="657da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="657da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="657da-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="657da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="657da-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="657da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="657da-107">Создание нового [объекта deviceManagementReusablePolicySetting.](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)</span><span class="sxs-lookup"><span data-stu-id="657da-107">Create a new [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="657da-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="657da-108">Prerequisites</span></span>
<span data-ttu-id="657da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="657da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="657da-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="657da-111">Permission type</span></span>|<span data-ttu-id="657da-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="657da-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="657da-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="657da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="657da-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="657da-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="657da-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="657da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="657da-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="657da-116">Not supported.</span></span>|
|<span data-ttu-id="657da-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="657da-117">Application</span></span>|<span data-ttu-id="657da-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="657da-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="657da-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="657da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusablePolicySettings
```

## <a name="request-headers"></a><span data-ttu-id="657da-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="657da-120">Request headers</span></span>
|<span data-ttu-id="657da-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="657da-121">Header</span></span>|<span data-ttu-id="657da-122">Значение</span><span class="sxs-lookup"><span data-stu-id="657da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="657da-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="657da-123">Authorization</span></span>|<span data-ttu-id="657da-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="657da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="657da-125">Accept</span><span class="sxs-lookup"><span data-stu-id="657da-125">Accept</span></span>|<span data-ttu-id="657da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="657da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="657da-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="657da-127">Request body</span></span>
<span data-ttu-id="657da-128">В теле запроса поставляем представление JSON для объекта deviceManagementReusablePolicySetting.</span><span class="sxs-lookup"><span data-stu-id="657da-128">In the request body, supply a JSON representation for the deviceManagementReusablePolicySetting object.</span></span>

<span data-ttu-id="657da-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementReusablePolicySetting.</span><span class="sxs-lookup"><span data-stu-id="657da-129">The following table shows the properties that are required when you create the deviceManagementReusablePolicySetting.</span></span>

|<span data-ttu-id="657da-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="657da-130">Property</span></span>|<span data-ttu-id="657da-131">Тип</span><span class="sxs-lookup"><span data-stu-id="657da-131">Type</span></span>|<span data-ttu-id="657da-132">Описание</span><span class="sxs-lookup"><span data-stu-id="657da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="657da-133">id</span><span class="sxs-lookup"><span data-stu-id="657da-133">id</span></span>|<span data-ttu-id="657da-134">String</span><span class="sxs-lookup"><span data-stu-id="657da-134">String</span></span>|<span data-ttu-id="657da-135">система, генерируемая многоярусным и настраиваемым id.</span><span class="sxs-lookup"><span data-stu-id="657da-135">system generated reusable setting id.</span></span>|
|<span data-ttu-id="657da-136">displayName</span><span class="sxs-lookup"><span data-stu-id="657da-136">displayName</span></span>|<span data-ttu-id="657da-137">String</span><span class="sxs-lookup"><span data-stu-id="657da-137">String</span></span>|<span data-ttu-id="657da-138">имя отображения для повторного параметров, предоставленное пользователем.</span><span class="sxs-lookup"><span data-stu-id="657da-138">reusable setting display name supplied by user.</span></span>|
|<span data-ttu-id="657da-139">description</span><span class="sxs-lookup"><span data-stu-id="657da-139">description</span></span>|<span data-ttu-id="657da-140">String</span><span class="sxs-lookup"><span data-stu-id="657da-140">String</span></span>|<span data-ttu-id="657da-141">повторное описание параметра, предоставленное пользователем.</span><span class="sxs-lookup"><span data-stu-id="657da-141">reusable setting description supplied by user.</span></span>|
|<span data-ttu-id="657da-142">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="657da-142">settingDefinitionId</span></span>|<span data-ttu-id="657da-143">String</span><span class="sxs-lookup"><span data-stu-id="657da-143">String</span></span>|<span data-ttu-id="657da-144">параметр определения, связанный с этим многопользоваемым параметром.</span><span class="sxs-lookup"><span data-stu-id="657da-144">setting definition id associated with this reusable setting.</span></span>|
|<span data-ttu-id="657da-145">settingInstance</span><span class="sxs-lookup"><span data-stu-id="657da-145">settingInstance</span></span>|[<span data-ttu-id="657da-146">deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="657da-146">deviceManagementConfigurationSettingInstance</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|<span data-ttu-id="657da-147">экземпляр конфигурации повторного параметров</span><span class="sxs-lookup"><span data-stu-id="657da-147">reusable setting configuration instance</span></span>|
|<span data-ttu-id="657da-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="657da-148">createdDateTime</span></span>|<span data-ttu-id="657da-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="657da-149">DateTimeOffset</span></span>|<span data-ttu-id="657da-150">дата и время создания параметров повторного параметров.</span><span class="sxs-lookup"><span data-stu-id="657da-150">reusable setting creation date and time.</span></span> <span data-ttu-id="657da-151">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="657da-151">This property is read-only.</span></span>|
|<span data-ttu-id="657da-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="657da-152">lastModifiedDateTime</span></span>|<span data-ttu-id="657da-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="657da-153">DateTimeOffset</span></span>|<span data-ttu-id="657da-154">дата и время последнего изменения параметра повторного параметров.</span><span class="sxs-lookup"><span data-stu-id="657da-154">date and time when reusable setting was last modified.</span></span> <span data-ttu-id="657da-155">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="657da-155">This property is read-only.</span></span>|
|<span data-ttu-id="657da-156">version</span><span class="sxs-lookup"><span data-stu-id="657da-156">version</span></span>|<span data-ttu-id="657da-157">Int32</span><span class="sxs-lookup"><span data-stu-id="657da-157">Int32</span></span>|<span data-ttu-id="657da-158">номер версии для повторного параметров.</span><span class="sxs-lookup"><span data-stu-id="657da-158">version number for reusable setting.</span></span> <span data-ttu-id="657da-159">Допустимые значения от 0 до 2147483647.</span><span class="sxs-lookup"><span data-stu-id="657da-159">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="657da-160">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="657da-160">This property is read-only.</span></span>|
|<span data-ttu-id="657da-161">referencingConfigurationPolicyCount</span><span class="sxs-lookup"><span data-stu-id="657da-161">referencingConfigurationPolicyCount</span></span>|<span data-ttu-id="657da-162">Int32</span><span class="sxs-lookup"><span data-stu-id="657da-162">Int32</span></span>|<span data-ttu-id="657da-163">количество политик конфигурации, ссылающихся на текущий параметр повторного параметров.</span><span class="sxs-lookup"><span data-stu-id="657da-163">count of configuration policies referencing the current reusable setting.</span></span> <span data-ttu-id="657da-164">Допустимые значения от 0 до 2147483647.</span><span class="sxs-lookup"><span data-stu-id="657da-164">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="657da-165">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="657da-165">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="657da-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="657da-166">Response</span></span>
<span data-ttu-id="657da-167">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="657da-167">If successful, this method returns a `201 Created` response code and a [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="657da-168">Пример</span><span class="sxs-lookup"><span data-stu-id="657da-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="657da-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="657da-169">Request</span></span>
<span data-ttu-id="657da-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="657da-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusablePolicySettings
Content-type: application/json
Content-length: 7888

{
  "@odata.type": "#microsoft.graph.deviceManagementReusablePolicySetting",
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
  "version": 7,
  "referencingConfigurationPolicyCount": 3
}
```

### <a name="response"></a><span data-ttu-id="657da-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="657da-171">Response</span></span>
<span data-ttu-id="657da-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="657da-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 8060

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
```




