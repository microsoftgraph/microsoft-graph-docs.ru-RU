---
title: Получение Девицеманажементколлектионсеттингдефинитион
description: Чтение свойств и связей объекта Девицеманажементколлектионсеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 06b90c882d2e2c163dfdf8cb35231c1de71c08ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054492"
---
# <a name="get-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="63226-103">Получение Девицеманажементколлектионсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="63226-103">Get deviceManagementCollectionSettingDefinition</span></span>

<span data-ttu-id="63226-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63226-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63226-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63226-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63226-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63226-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63226-107">Чтение свойств и связей объекта [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="63226-107">Read properties and relationships of the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63226-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="63226-108">Prerequisites</span></span>
<span data-ttu-id="63226-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63226-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63226-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63226-111">Permission type</span></span>|<span data-ttu-id="63226-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63226-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63226-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63226-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63226-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63226-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="63226-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63226-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63226-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63226-116">Not supported.</span></span>|
|<span data-ttu-id="63226-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63226-117">Application</span></span>|<span data-ttu-id="63226-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63226-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63226-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63226-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
GET /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63226-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="63226-120">Optional query parameters</span></span>
<span data-ttu-id="63226-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="63226-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63226-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63226-122">Request headers</span></span>
|<span data-ttu-id="63226-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63226-123">Header</span></span>|<span data-ttu-id="63226-124">Значение</span><span class="sxs-lookup"><span data-stu-id="63226-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63226-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63226-125">Authorization</span></span>|<span data-ttu-id="63226-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63226-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63226-127">Accept</span><span class="sxs-lookup"><span data-stu-id="63226-127">Accept</span></span>|<span data-ttu-id="63226-128">application/json</span><span class="sxs-lookup"><span data-stu-id="63226-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63226-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63226-129">Request body</span></span>
<span data-ttu-id="63226-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63226-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63226-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="63226-131">Response</span></span>
<span data-ttu-id="63226-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63226-132">If successful, this method returns a `200 OK` response code and [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63226-133">Пример</span><span class="sxs-lookup"><span data-stu-id="63226-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="63226-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="63226-134">Request</span></span>
<span data-ttu-id="63226-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63226-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="63226-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="63226-136">Response</span></span>
<span data-ttu-id="63226-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63226-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1131

{
  "value": {
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
}
```






