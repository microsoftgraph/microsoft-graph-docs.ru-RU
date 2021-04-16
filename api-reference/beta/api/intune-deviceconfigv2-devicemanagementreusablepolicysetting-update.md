---
title: Обновление deviceManagementReusablePolicySetting
description: Обновление свойств объекта deviceManagementReusablePolicySetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3332732f8d52b90582e320939ff395ee98b3712f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869145"
---
# <a name="update-devicemanagementreusablepolicysetting"></a><span data-ttu-id="64031-103">Обновление deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="64031-103">Update deviceManagementReusablePolicySetting</span></span>

<span data-ttu-id="64031-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64031-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64031-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64031-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64031-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64031-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64031-107">Обновление свойств объекта [deviceManagementReusablePolicySetting.](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)</span><span class="sxs-lookup"><span data-stu-id="64031-107">Update the properties of a [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64031-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="64031-108">Prerequisites</span></span>
<span data-ttu-id="64031-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64031-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64031-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64031-111">Permission type</span></span>|<span data-ttu-id="64031-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64031-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64031-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64031-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64031-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64031-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64031-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64031-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64031-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64031-116">Not supported.</span></span>|
|<span data-ttu-id="64031-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="64031-117">Application</span></span>|<span data-ttu-id="64031-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64031-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64031-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64031-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}
```

## <a name="request-headers"></a><span data-ttu-id="64031-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="64031-120">Request headers</span></span>
|<span data-ttu-id="64031-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64031-121">Header</span></span>|<span data-ttu-id="64031-122">Значение</span><span class="sxs-lookup"><span data-stu-id="64031-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64031-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64031-123">Authorization</span></span>|<span data-ttu-id="64031-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64031-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64031-125">Accept</span><span class="sxs-lookup"><span data-stu-id="64031-125">Accept</span></span>|<span data-ttu-id="64031-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64031-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64031-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64031-127">Request body</span></span>
<span data-ttu-id="64031-128">В теле запроса поставляем представление JSON для [объекта deviceManagementReusablePolicySetting.](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)</span><span class="sxs-lookup"><span data-stu-id="64031-128">In the request body, supply a JSON representation for the [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object.</span></span>

<span data-ttu-id="64031-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementReusablePolicySetting.](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)</span><span class="sxs-lookup"><span data-stu-id="64031-129">The following table shows the properties that are required when you create the [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md).</span></span>

|<span data-ttu-id="64031-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="64031-130">Property</span></span>|<span data-ttu-id="64031-131">Тип</span><span class="sxs-lookup"><span data-stu-id="64031-131">Type</span></span>|<span data-ttu-id="64031-132">Описание</span><span class="sxs-lookup"><span data-stu-id="64031-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64031-133">id</span><span class="sxs-lookup"><span data-stu-id="64031-133">id</span></span>|<span data-ttu-id="64031-134">String</span><span class="sxs-lookup"><span data-stu-id="64031-134">String</span></span>|<span data-ttu-id="64031-135">система, генерируемая многоярусным и настраиваемым id.</span><span class="sxs-lookup"><span data-stu-id="64031-135">system generated reusable setting id.</span></span>|
|<span data-ttu-id="64031-136">displayName</span><span class="sxs-lookup"><span data-stu-id="64031-136">displayName</span></span>|<span data-ttu-id="64031-137">String</span><span class="sxs-lookup"><span data-stu-id="64031-137">String</span></span>|<span data-ttu-id="64031-138">имя отображения для повторного параметров, предоставленное пользователем.</span><span class="sxs-lookup"><span data-stu-id="64031-138">reusable setting display name supplied by user.</span></span>|
|<span data-ttu-id="64031-139">description</span><span class="sxs-lookup"><span data-stu-id="64031-139">description</span></span>|<span data-ttu-id="64031-140">String</span><span class="sxs-lookup"><span data-stu-id="64031-140">String</span></span>|<span data-ttu-id="64031-141">повторное описание параметра, предоставленное пользователем.</span><span class="sxs-lookup"><span data-stu-id="64031-141">reusable setting description supplied by user.</span></span>|
|<span data-ttu-id="64031-142">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="64031-142">settingDefinitionId</span></span>|<span data-ttu-id="64031-143">String</span><span class="sxs-lookup"><span data-stu-id="64031-143">String</span></span>|<span data-ttu-id="64031-144">параметр определения, связанный с этим многопользоваемым параметром.</span><span class="sxs-lookup"><span data-stu-id="64031-144">setting definition id associated with this reusable setting.</span></span>|
|<span data-ttu-id="64031-145">settingInstance</span><span class="sxs-lookup"><span data-stu-id="64031-145">settingInstance</span></span>|[<span data-ttu-id="64031-146">deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="64031-146">deviceManagementConfigurationSettingInstance</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|<span data-ttu-id="64031-147">экземпляр конфигурации повторного параметров</span><span class="sxs-lookup"><span data-stu-id="64031-147">reusable setting configuration instance</span></span>|
|<span data-ttu-id="64031-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64031-148">createdDateTime</span></span>|<span data-ttu-id="64031-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64031-149">DateTimeOffset</span></span>|<span data-ttu-id="64031-150">дата и время создания параметров повторного параметров.</span><span class="sxs-lookup"><span data-stu-id="64031-150">reusable setting creation date and time.</span></span> <span data-ttu-id="64031-151">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64031-151">This property is read-only.</span></span>|
|<span data-ttu-id="64031-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64031-152">lastModifiedDateTime</span></span>|<span data-ttu-id="64031-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64031-153">DateTimeOffset</span></span>|<span data-ttu-id="64031-154">дата и время последнего изменения параметра повторного параметров.</span><span class="sxs-lookup"><span data-stu-id="64031-154">date and time when reusable setting was last modified.</span></span> <span data-ttu-id="64031-155">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64031-155">This property is read-only.</span></span>|
|<span data-ttu-id="64031-156">version</span><span class="sxs-lookup"><span data-stu-id="64031-156">version</span></span>|<span data-ttu-id="64031-157">Int32</span><span class="sxs-lookup"><span data-stu-id="64031-157">Int32</span></span>|<span data-ttu-id="64031-158">номер версии для повторного параметров.</span><span class="sxs-lookup"><span data-stu-id="64031-158">version number for reusable setting.</span></span> <span data-ttu-id="64031-159">Допустимые значения от 0 до 2147483647.</span><span class="sxs-lookup"><span data-stu-id="64031-159">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="64031-160">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64031-160">This property is read-only.</span></span>|
|<span data-ttu-id="64031-161">referencingConfigurationPolicyCount</span><span class="sxs-lookup"><span data-stu-id="64031-161">referencingConfigurationPolicyCount</span></span>|<span data-ttu-id="64031-162">Int32</span><span class="sxs-lookup"><span data-stu-id="64031-162">Int32</span></span>|<span data-ttu-id="64031-163">количество политик конфигурации, ссылающихся на текущий параметр повторного параметров.</span><span class="sxs-lookup"><span data-stu-id="64031-163">count of configuration policies referencing the current reusable setting.</span></span> <span data-ttu-id="64031-164">Допустимые значения от 0 до 2147483647.</span><span class="sxs-lookup"><span data-stu-id="64031-164">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="64031-165">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64031-165">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="64031-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="64031-166">Response</span></span>
<span data-ttu-id="64031-167">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="64031-167">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64031-168">Пример</span><span class="sxs-lookup"><span data-stu-id="64031-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="64031-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="64031-169">Request</span></span>
<span data-ttu-id="64031-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64031-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}
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

### <a name="response"></a><span data-ttu-id="64031-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="64031-171">Response</span></span>
<span data-ttu-id="64031-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64031-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




