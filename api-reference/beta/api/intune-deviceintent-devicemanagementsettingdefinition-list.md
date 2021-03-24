---
title: Список deviceManagementSettingDefinitions
description: Список свойств и связей объектов deviceManagementSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 991ced33cc07d03dd6921b4034647918a6838331
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146582"
---
# <a name="list-devicemanagementsettingdefinitions"></a><span data-ttu-id="90680-103">Список deviceManagementSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="90680-103">List deviceManagementSettingDefinitions</span></span>

<span data-ttu-id="90680-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90680-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90680-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90680-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90680-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90680-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90680-107">Список свойств и связей [объектов deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="90680-107">List properties and relationships of the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90680-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="90680-108">Prerequisites</span></span>
<span data-ttu-id="90680-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90680-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90680-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90680-111">Permission type</span></span>|<span data-ttu-id="90680-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90680-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90680-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90680-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90680-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90680-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90680-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90680-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90680-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90680-116">Not supported.</span></span>|
|<span data-ttu-id="90680-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="90680-117">Application</span></span>|<span data-ttu-id="90680-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90680-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90680-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90680-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="90680-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="90680-120">Request headers</span></span>
|<span data-ttu-id="90680-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90680-121">Header</span></span>|<span data-ttu-id="90680-122">Значение</span><span class="sxs-lookup"><span data-stu-id="90680-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90680-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90680-123">Authorization</span></span>|<span data-ttu-id="90680-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90680-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90680-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90680-125">Accept</span></span>|<span data-ttu-id="90680-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90680-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90680-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90680-127">Request body</span></span>
<span data-ttu-id="90680-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90680-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90680-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="90680-129">Response</span></span>
<span data-ttu-id="90680-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="90680-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90680-131">Пример</span><span class="sxs-lookup"><span data-stu-id="90680-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="90680-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="90680-132">Request</span></span>
<span data-ttu-id="90680-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90680-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="90680-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="90680-134">Response</span></span>
<span data-ttu-id="90680-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90680-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1236

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
      "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
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
      ]
    }
  ]
}
```




