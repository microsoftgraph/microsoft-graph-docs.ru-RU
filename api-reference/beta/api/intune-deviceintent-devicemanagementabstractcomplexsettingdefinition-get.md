---
title: Получение Девицеманажементабстракткомплекссеттингдефинитион
description: Чтение свойств и связей объекта Девицеманажементабстракткомплекссеттингдефинитион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a104ad9a2d403c1777897d8e8e9b70bcb527957
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800212"
---
# <a name="get-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="eb124-103">Получение Девицеманажементабстракткомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="eb124-103">Get deviceManagementAbstractComplexSettingDefinition</span></span>

> <span data-ttu-id="eb124-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb124-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb124-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb124-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb124-106">Чтение свойств и связей объекта [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="eb124-106">Read properties and relationships of the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb124-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eb124-107">Prerequisites</span></span>
<span data-ttu-id="eb124-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb124-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb124-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb124-110">Permission type</span></span>|<span data-ttu-id="eb124-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb124-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb124-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb124-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb124-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb124-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eb124-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb124-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb124-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb124-115">Not supported.</span></span>|
|<span data-ttu-id="eb124-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb124-116">Application</span></span>|<span data-ttu-id="eb124-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb124-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb124-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb124-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="eb124-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eb124-119">Optional query parameters</span></span>
<span data-ttu-id="eb124-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eb124-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb124-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb124-121">Request headers</span></span>
|<span data-ttu-id="eb124-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb124-122">Header</span></span>|<span data-ttu-id="eb124-123">Значение</span><span class="sxs-lookup"><span data-stu-id="eb124-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb124-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb124-124">Authorization</span></span>|<span data-ttu-id="eb124-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb124-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb124-126">Accept</span><span class="sxs-lookup"><span data-stu-id="eb124-126">Accept</span></span>|<span data-ttu-id="eb124-127">application/json</span><span class="sxs-lookup"><span data-stu-id="eb124-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb124-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb124-128">Request body</span></span>
<span data-ttu-id="eb124-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb124-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb124-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb124-130">Response</span></span>
<span data-ttu-id="eb124-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb124-131">If successful, this method returns a `200 OK` response code and [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb124-132">Пример</span><span class="sxs-lookup"><span data-stu-id="eb124-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb124-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb124-133">Request</span></span>
<span data-ttu-id="eb124-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb124-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="eb124-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb124-135">Response</span></span>
<span data-ttu-id="eb124-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb124-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 928

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
    "id": "1b703309-3309-1b70-0933-701b0933701b",
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
    "implementations": [
      "Implementations value"
    ]
  }
}
```





