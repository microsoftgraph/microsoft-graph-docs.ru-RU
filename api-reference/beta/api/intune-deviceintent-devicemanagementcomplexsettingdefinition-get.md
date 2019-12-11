---
title: Получение Девицеманажементкомплекссеттингдефинитион
description: Чтение свойств и связей объекта Девицеманажементкомплекссеттингдефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 319f0b76ea65980cec6d07f809d9c3b08be96889
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946065"
---
# <a name="get-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="72375-103">Получение Девицеманажементкомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="72375-103">Get deviceManagementComplexSettingDefinition</span></span>

> <span data-ttu-id="72375-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72375-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72375-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72375-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72375-106">Чтение свойств и связей объекта [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="72375-106">Read properties and relationships of the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72375-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="72375-107">Prerequisites</span></span>
<span data-ttu-id="72375-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72375-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72375-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72375-110">Permission type</span></span>|<span data-ttu-id="72375-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72375-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72375-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72375-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72375-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="72375-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="72375-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72375-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72375-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72375-115">Not supported.</span></span>|
|<span data-ttu-id="72375-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72375-116">Application</span></span>|<span data-ttu-id="72375-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="72375-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72375-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72375-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="72375-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72375-119">Optional query parameters</span></span>
<span data-ttu-id="72375-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="72375-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72375-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72375-121">Request headers</span></span>
|<span data-ttu-id="72375-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72375-122">Header</span></span>|<span data-ttu-id="72375-123">Значение</span><span class="sxs-lookup"><span data-stu-id="72375-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72375-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72375-124">Authorization</span></span>|<span data-ttu-id="72375-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72375-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72375-126">Accept</span><span class="sxs-lookup"><span data-stu-id="72375-126">Accept</span></span>|<span data-ttu-id="72375-127">application/json</span><span class="sxs-lookup"><span data-stu-id="72375-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72375-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="72375-128">Request body</span></span>
<span data-ttu-id="72375-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72375-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72375-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="72375-130">Response</span></span>
<span data-ttu-id="72375-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72375-131">If successful, this method returns a `200 OK` response code and [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72375-132">Пример</span><span class="sxs-lookup"><span data-stu-id="72375-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="72375-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="72375-133">Request</span></span>
<span data-ttu-id="72375-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72375-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="72375-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="72375-135">Response</span></span>
<span data-ttu-id="72375-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72375-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





