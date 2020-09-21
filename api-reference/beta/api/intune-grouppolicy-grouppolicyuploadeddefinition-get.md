---
title: Получение Граупполициуплоадеддефинитион
description: Чтение свойств и связей объекта Граупполициуплоадеддефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 080a08226d66e146f2a50bae2e118475ca6d8fc8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000499"
---
# <a name="get-grouppolicyuploadeddefinition"></a><span data-ttu-id="8da52-103">Получение Граупполициуплоадеддефинитион</span><span class="sxs-lookup"><span data-stu-id="8da52-103">Get groupPolicyUploadedDefinition</span></span>

<span data-ttu-id="8da52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8da52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8da52-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8da52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8da52-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8da52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8da52-107">Чтение свойств и связей объекта [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="8da52-107">Read properties and relationships of the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8da52-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8da52-108">Prerequisites</span></span>
<span data-ttu-id="8da52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8da52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8da52-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8da52-111">Permission type</span></span>|<span data-ttu-id="8da52-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8da52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8da52-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8da52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8da52-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8da52-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8da52-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8da52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8da52-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8da52-116">Not supported.</span></span>|
|<span data-ttu-id="8da52-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8da52-117">Application</span></span>|<span data-ttu-id="8da52-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8da52-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8da52-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8da52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions/{groupPolicyDefinitionId}
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8da52-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="8da52-120">Optional query parameters</span></span>
<span data-ttu-id="8da52-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8da52-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8da52-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8da52-122">Request headers</span></span>
|<span data-ttu-id="8da52-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8da52-123">Header</span></span>|<span data-ttu-id="8da52-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8da52-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8da52-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8da52-125">Authorization</span></span>|<span data-ttu-id="8da52-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8da52-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8da52-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8da52-127">Accept</span></span>|<span data-ttu-id="8da52-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8da52-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8da52-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8da52-129">Request body</span></span>
<span data-ttu-id="8da52-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8da52-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8da52-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8da52-131">Response</span></span>
<span data-ttu-id="8da52-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8da52-132">If successful, this method returns a `200 OK` response code and [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8da52-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8da52-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8da52-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8da52-134">Request</span></span>
<span data-ttu-id="8da52-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8da52-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
```

### <a name="response"></a><span data-ttu-id="8da52-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8da52-136">Response</span></span>
<span data-ttu-id="8da52-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8da52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 513

{
  "value": {
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
}
```






