---
title: Список Девицеманажементабстракткомплекссеттингдефинитионс
description: Список свойств и связей объектов Девицеманажементабстракткомплекссеттингдефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac7278a02037a957f9801199dc9d76759c7593af
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636464"
---
# <a name="list-devicemanagementabstractcomplexsettingdefinitions"></a><span data-ttu-id="3ad48-103">Список Девицеманажементабстракткомплекссеттингдефинитионс</span><span class="sxs-lookup"><span data-stu-id="3ad48-103">List deviceManagementAbstractComplexSettingDefinitions</span></span>

> <span data-ttu-id="3ad48-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ad48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ad48-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ad48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ad48-106">Список свойств и связей объектов [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="3ad48-106">List properties and relationships of the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ad48-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3ad48-107">Prerequisites</span></span>
<span data-ttu-id="3ad48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ad48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ad48-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ad48-110">Permission type</span></span>|<span data-ttu-id="3ad48-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ad48-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ad48-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ad48-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ad48-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ad48-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3ad48-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ad48-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ad48-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ad48-115">Not supported.</span></span>|
|<span data-ttu-id="3ad48-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ad48-116">Application</span></span>|<span data-ttu-id="3ad48-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ad48-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ad48-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ad48-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="3ad48-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3ad48-119">Request headers</span></span>
|<span data-ttu-id="3ad48-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ad48-120">Header</span></span>|<span data-ttu-id="3ad48-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3ad48-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ad48-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ad48-122">Authorization</span></span>|<span data-ttu-id="3ad48-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ad48-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ad48-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3ad48-124">Accept</span></span>|<span data-ttu-id="3ad48-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ad48-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ad48-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ad48-126">Request body</span></span>
<span data-ttu-id="3ad48-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ad48-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ad48-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ad48-128">Response</span></span>
<span data-ttu-id="3ad48-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ad48-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ad48-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3ad48-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ad48-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ad48-131">Request</span></span>
<span data-ttu-id="3ad48-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ad48-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="3ad48-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ad48-133">Response</span></span>
<span data-ttu-id="3ad48-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ad48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1228

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





