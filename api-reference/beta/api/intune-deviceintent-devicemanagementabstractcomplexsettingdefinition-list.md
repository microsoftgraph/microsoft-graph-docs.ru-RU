---
title: Список deviceManagementAbstractComplexSettingDefinitions
description: Список свойств и связей объектов deviceManagementAbstractComplexSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 044ff8d7e13b5965d9ff3b85e15b656fb75c57be
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129064"
---
# <a name="list-devicemanagementabstractcomplexsettingdefinitions"></a><span data-ttu-id="057dc-103">Список deviceManagementAbstractComplexSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="057dc-103">List deviceManagementAbstractComplexSettingDefinitions</span></span>

<span data-ttu-id="057dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="057dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="057dc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="057dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="057dc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="057dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="057dc-107">Список свойств и связей [объектов deviceManagementAbstractComplexSettingDefinition.](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="057dc-107">List properties and relationships of the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="057dc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="057dc-108">Prerequisites</span></span>
<span data-ttu-id="057dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="057dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="057dc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="057dc-111">Permission type</span></span>|<span data-ttu-id="057dc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="057dc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="057dc-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="057dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="057dc-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="057dc-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="057dc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="057dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="057dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="057dc-116">Not supported.</span></span>|
|<span data-ttu-id="057dc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="057dc-117">Application</span></span>|<span data-ttu-id="057dc-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="057dc-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="057dc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="057dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/settingDefinitions
GET /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="057dc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="057dc-120">Request headers</span></span>
|<span data-ttu-id="057dc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="057dc-121">Header</span></span>|<span data-ttu-id="057dc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="057dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="057dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="057dc-123">Authorization</span></span>|<span data-ttu-id="057dc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="057dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="057dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="057dc-125">Accept</span></span>|<span data-ttu-id="057dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="057dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="057dc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="057dc-127">Request body</span></span>
<span data-ttu-id="057dc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="057dc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="057dc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="057dc-129">Response</span></span>
<span data-ttu-id="057dc-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="057dc-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="057dc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="057dc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="057dc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="057dc-132">Request</span></span>
<span data-ttu-id="057dc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="057dc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="057dc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="057dc-134">Response</span></span>
<span data-ttu-id="057dc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="057dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1322

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
      "id": "1b703309-3309-1b70-0933-701b0933701b",
      "valueType": "boolean",
      "displayName": "Display Name value",
      "isTopLevel": true,
      "description": "Description value",
      "placeholderText": "Placeholder Text value",
      "documentationUrl": "https://example.com/documentationUrl/",
      "headerTitle": "Header Title value",
      "headerSubtitle": "Header Subtitle value",
      "keywords": [
        "Keywords value"
      ],
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
          "supportedTypes": [
            "Supported Types value"
          ]
        }
      ],
      "dependencies": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
          "definitionId": "Definition Id value",
          "constraints": [
            {
              "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
              "supportedTypes": [
                "Supported Types value"
              ]
            }
          ]
        }
      ],
      "implementations": [
        "Implementations value"
      ]
    }
  ]
}
```




