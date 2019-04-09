---
title: Список Девицеманажементсеттингдефинитионс
description: Список свойств и связей объектов Девицеманажементсеттингдефинитион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eaf4c3fb65677cc8d9f9ea3e971ff08aefd116e7
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524003"
---
# <a name="list-devicemanagementsettingdefinitions"></a><span data-ttu-id="63d00-103">Список Девицеманажементсеттингдефинитионс</span><span class="sxs-lookup"><span data-stu-id="63d00-103">List deviceManagementSettingDefinitions</span></span>

> <span data-ttu-id="63d00-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63d00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63d00-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63d00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63d00-106">Список свойств и связей объектов [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="63d00-106">List properties and relationships of the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63d00-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="63d00-107">Prerequisites</span></span>
<span data-ttu-id="63d00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63d00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63d00-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63d00-110">Permission type</span></span>|<span data-ttu-id="63d00-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63d00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63d00-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63d00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63d00-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63d00-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="63d00-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63d00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63d00-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63d00-115">Not supported.</span></span>|
|<span data-ttu-id="63d00-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63d00-116">Application</span></span>|<span data-ttu-id="63d00-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63d00-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63d00-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63d00-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="63d00-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63d00-119">Request headers</span></span>
|<span data-ttu-id="63d00-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63d00-120">Header</span></span>|<span data-ttu-id="63d00-121">Значение</span><span class="sxs-lookup"><span data-stu-id="63d00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63d00-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63d00-122">Authorization</span></span>|<span data-ttu-id="63d00-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63d00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63d00-124">Accept</span><span class="sxs-lookup"><span data-stu-id="63d00-124">Accept</span></span>|<span data-ttu-id="63d00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63d00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63d00-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63d00-126">Request body</span></span>
<span data-ttu-id="63d00-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63d00-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63d00-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="63d00-128">Response</span></span>
<span data-ttu-id="63d00-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63d00-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63d00-130">Пример</span><span class="sxs-lookup"><span data-stu-id="63d00-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="63d00-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="63d00-131">Request</span></span>
<span data-ttu-id="63d00-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63d00-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="63d00-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="63d00-133">Response</span></span>
<span data-ttu-id="63d00-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63d00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
      "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
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
      ]
    }
  ]
}
```







