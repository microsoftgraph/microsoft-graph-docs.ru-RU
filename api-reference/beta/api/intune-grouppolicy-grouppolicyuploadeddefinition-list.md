---
title: Список Граупполициуплоадеддефинитионс
description: Список свойств и связей объектов Граупполициуплоадеддефинитион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01fd83bbd4aace0e6663fe4379341336af004400
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803745"
---
# <a name="list-grouppolicyuploadeddefinitions"></a><span data-ttu-id="afaad-103">Список Граупполициуплоадеддефинитионс</span><span class="sxs-lookup"><span data-stu-id="afaad-103">List groupPolicyUploadedDefinitions</span></span>

> <span data-ttu-id="afaad-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afaad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afaad-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="afaad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afaad-106">Список свойств и связей объектов [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="afaad-106">List properties and relationships of the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afaad-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="afaad-107">Prerequisites</span></span>
<span data-ttu-id="afaad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afaad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afaad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afaad-110">Permission type</span></span>|<span data-ttu-id="afaad-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="afaad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afaad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afaad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="afaad-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="afaad-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="afaad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afaad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afaad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afaad-115">Not supported.</span></span>|
|<span data-ttu-id="afaad-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="afaad-116">Application</span></span>|<span data-ttu-id="afaad-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="afaad-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="afaad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afaad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyDefinitions
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
```

## <a name="request-headers"></a><span data-ttu-id="afaad-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="afaad-119">Request headers</span></span>
|<span data-ttu-id="afaad-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="afaad-120">Header</span></span>|<span data-ttu-id="afaad-121">Значение</span><span class="sxs-lookup"><span data-stu-id="afaad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afaad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="afaad-122">Authorization</span></span>|<span data-ttu-id="afaad-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afaad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afaad-124">Accept</span><span class="sxs-lookup"><span data-stu-id="afaad-124">Accept</span></span>|<span data-ttu-id="afaad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="afaad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afaad-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afaad-126">Request body</span></span>
<span data-ttu-id="afaad-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="afaad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afaad-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="afaad-128">Response</span></span>
<span data-ttu-id="afaad-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="afaad-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afaad-130">Пример</span><span class="sxs-lookup"><span data-stu-id="afaad-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="afaad-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="afaad-131">Request</span></span>
<span data-ttu-id="afaad-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afaad-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions
```

### <a name="response"></a><span data-ttu-id="afaad-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="afaad-133">Response</span></span>
<span data-ttu-id="afaad-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="afaad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
      "classType": "machine",
      "displayName": "Display Name value",
      "explainText": "Explain Text value",
      "categoryPath": "Category Path value",
      "supportedOn": "Supported On value",
      "policyType": "admxIngested",
      "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
      "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




