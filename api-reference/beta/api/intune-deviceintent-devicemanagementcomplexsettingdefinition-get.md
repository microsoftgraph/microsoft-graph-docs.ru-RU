---
title: Получение Девицеманажементкомплекссеттингдефинитион
description: Чтение свойств и связей объекта Девицеманажементкомплекссеттингдефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dc8bf1f42c6559056ca8da04c1bb08e4543020af
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181093"
---
# <a name="get-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="ef34b-103">Получение Девицеманажементкомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="ef34b-103">Get deviceManagementComplexSettingDefinition</span></span>

> <span data-ttu-id="ef34b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef34b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef34b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef34b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef34b-106">Чтение свойств и связей объекта [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="ef34b-106">Read properties and relationships of the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef34b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ef34b-107">Prerequisites</span></span>
<span data-ttu-id="ef34b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef34b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef34b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef34b-110">Permission type</span></span>|<span data-ttu-id="ef34b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef34b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef34b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef34b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef34b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef34b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ef34b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef34b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef34b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef34b-115">Not supported.</span></span>|
|<span data-ttu-id="ef34b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef34b-116">Application</span></span>|<span data-ttu-id="ef34b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef34b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef34b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef34b-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="ef34b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ef34b-119">Optional query parameters</span></span>
<span data-ttu-id="ef34b-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ef34b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef34b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef34b-121">Request headers</span></span>
|<span data-ttu-id="ef34b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef34b-122">Header</span></span>|<span data-ttu-id="ef34b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ef34b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef34b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef34b-124">Authorization</span></span>|<span data-ttu-id="ef34b-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef34b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef34b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ef34b-126">Accept</span></span>|<span data-ttu-id="ef34b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ef34b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef34b-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef34b-128">Request body</span></span>
<span data-ttu-id="ef34b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef34b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef34b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef34b-130">Response</span></span>
<span data-ttu-id="ef34b-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef34b-131">If successful, this method returns a `200 OK` response code and [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef34b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ef34b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef34b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef34b-133">Request</span></span>
<span data-ttu-id="ef34b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef34b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="ef34b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef34b-135">Response</span></span>
<span data-ttu-id="ef34b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef34b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 934

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
    "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
    "valueType": "boolean",
    "displayName": "Display Name value",
    "isTopLevel": true,
    "description": "Description value",
    "documentationUrl": "https://example.com/documentationUrl/",
    "keywords": [
      "Keywords value"
    ],
    "constraints": [
      {
        "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
      }
    ],
    "dependencies": [
      {
        "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
        "definitionId": "Definition Id value",
        "constraints": [
          {
            "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
          }
        ]
      }
    ],
    "propertyDefinitionIds": [
      "Property Definition Ids value"
    ]
  }
}
```




