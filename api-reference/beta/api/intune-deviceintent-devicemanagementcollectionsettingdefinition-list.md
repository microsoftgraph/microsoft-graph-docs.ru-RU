---
title: Список Девицеманажементколлектионсеттингдефинитионс
description: Список свойств и связей объектов Девицеманажементколлектионсеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5f74d2b9ab3ae856d845b4f906b0358a14d4a32
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43329525"
---
# <a name="list-devicemanagementcollectionsettingdefinitions"></a><span data-ttu-id="2ab37-103">Список Девицеманажементколлектионсеттингдефинитионс</span><span class="sxs-lookup"><span data-stu-id="2ab37-103">List deviceManagementCollectionSettingDefinitions</span></span>

<span data-ttu-id="2ab37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ab37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ab37-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ab37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ab37-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ab37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ab37-107">Список свойств и связей объектов [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="2ab37-107">List properties and relationships of the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ab37-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2ab37-108">Prerequisites</span></span>
<span data-ttu-id="2ab37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ab37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ab37-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ab37-111">Permission type</span></span>|<span data-ttu-id="2ab37-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ab37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ab37-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ab37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ab37-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ab37-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2ab37-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ab37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ab37-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ab37-116">Not supported.</span></span>|
|<span data-ttu-id="2ab37-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ab37-117">Application</span></span>|<span data-ttu-id="2ab37-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ab37-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ab37-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ab37-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2ab37-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2ab37-120">Request headers</span></span>
|<span data-ttu-id="2ab37-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ab37-121">Header</span></span>|<span data-ttu-id="2ab37-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2ab37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ab37-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ab37-123">Authorization</span></span>|<span data-ttu-id="2ab37-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ab37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ab37-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2ab37-125">Accept</span></span>|<span data-ttu-id="2ab37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ab37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ab37-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ab37-127">Request body</span></span>
<span data-ttu-id="2ab37-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ab37-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ab37-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ab37-129">Response</span></span>
<span data-ttu-id="2ab37-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ab37-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ab37-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2ab37-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ab37-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ab37-132">Request</span></span>
<span data-ttu-id="2ab37-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ab37-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="2ab37-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ab37-134">Response</span></span>
<span data-ttu-id="2ab37-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ab37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1213

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
      "id": "0419c4a7-c4a7-0419-a7c4-1904a7c41904",
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
      "elementDefinitionId": "Element Definition Id value"
    }
  ]
}
```



