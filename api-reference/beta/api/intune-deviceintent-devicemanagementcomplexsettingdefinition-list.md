---
title: Список Девицеманажементкомплекссеттингдефинитионс
description: Список свойств и связей объектов Девицеманажементкомплекссеттингдефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a40d19a1589f131dad9c1349f57e2438b8518c8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42472046"
---
# <a name="list-devicemanagementcomplexsettingdefinitions"></a><span data-ttu-id="f8ae7-103">Список Девицеманажементкомплекссеттингдефинитионс</span><span class="sxs-lookup"><span data-stu-id="f8ae7-103">List deviceManagementComplexSettingDefinitions</span></span>

<span data-ttu-id="f8ae7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f8ae7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8ae7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8ae7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8ae7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8ae7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8ae7-107">Список свойств и связей объектов [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="f8ae7-107">List properties and relationships of the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8ae7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f8ae7-108">Prerequisites</span></span>
<span data-ttu-id="f8ae7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8ae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8ae7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8ae7-111">Permission type</span></span>|<span data-ttu-id="f8ae7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8ae7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8ae7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8ae7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8ae7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8ae7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f8ae7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8ae7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8ae7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8ae7-116">Not supported.</span></span>|
|<span data-ttu-id="f8ae7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8ae7-117">Application</span></span>|<span data-ttu-id="f8ae7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8ae7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8ae7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8ae7-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f8ae7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f8ae7-120">Request headers</span></span>
|<span data-ttu-id="f8ae7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8ae7-121">Header</span></span>|<span data-ttu-id="f8ae7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f8ae7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8ae7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8ae7-123">Authorization</span></span>|<span data-ttu-id="f8ae7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8ae7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8ae7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8ae7-125">Accept</span></span>|<span data-ttu-id="f8ae7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8ae7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8ae7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8ae7-127">Request body</span></span>
<span data-ttu-id="f8ae7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8ae7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8ae7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8ae7-129">Response</span></span>
<span data-ttu-id="f8ae7-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8ae7-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8ae7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f8ae7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8ae7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8ae7-132">Request</span></span>
<span data-ttu-id="f8ae7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8ae7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="f8ae7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8ae7-134">Response</span></span>
<span data-ttu-id="f8ae7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8ae7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1234

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
      "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
      "valueType": "boolean",
      "displayName": "Display Name value",
      "isTopLevel": true,
      "description": "Description value",
      "placeholderText": "Placeholder Text value",
      "documentationUrl": "https://example.com/documentationUrl/",
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
      "propertyDefinitionIds": [
        "Property Definition Ids value"
      ]
    }
  ]
}
```





