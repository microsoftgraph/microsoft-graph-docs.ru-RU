---
title: Получение Девицеманажементколлектионсеттингдефинитион
description: Чтение свойств и связей объекта Девицеманажементколлектионсеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: edcbbe098f3ac72e6d405f4ce18cef92f8c117ea
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49290289"
---
# <a name="get-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="226aa-103">Получение Девицеманажементколлектионсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="226aa-103">Get deviceManagementCollectionSettingDefinition</span></span>

<span data-ttu-id="226aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="226aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="226aa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="226aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="226aa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="226aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="226aa-107">Чтение свойств и связей объекта [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="226aa-107">Read properties and relationships of the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="226aa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="226aa-108">Prerequisites</span></span>
<span data-ttu-id="226aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="226aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="226aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="226aa-111">Permission type</span></span>|<span data-ttu-id="226aa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="226aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="226aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="226aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="226aa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="226aa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="226aa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="226aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="226aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="226aa-116">Not supported.</span></span>|
|<span data-ttu-id="226aa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="226aa-117">Application</span></span>|<span data-ttu-id="226aa-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="226aa-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="226aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="226aa-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="226aa-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="226aa-120">Optional query parameters</span></span>
<span data-ttu-id="226aa-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="226aa-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="226aa-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="226aa-122">Request headers</span></span>
|<span data-ttu-id="226aa-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="226aa-123">Header</span></span>|<span data-ttu-id="226aa-124">Значение</span><span class="sxs-lookup"><span data-stu-id="226aa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="226aa-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="226aa-125">Authorization</span></span>|<span data-ttu-id="226aa-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="226aa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="226aa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="226aa-127">Accept</span></span>|<span data-ttu-id="226aa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="226aa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="226aa-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="226aa-129">Request body</span></span>
<span data-ttu-id="226aa-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="226aa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="226aa-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="226aa-131">Response</span></span>
<span data-ttu-id="226aa-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="226aa-132">If successful, this method returns a `200 OK` response code and [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="226aa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="226aa-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="226aa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="226aa-134">Request</span></span>
<span data-ttu-id="226aa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="226aa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="226aa-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="226aa-136">Response</span></span>
<span data-ttu-id="226aa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="226aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1221

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
    "elementDefinitionId": "Element Definition Id value"
  }
}
```




