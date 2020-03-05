---
title: Получение Граупполициуплоадеддефинитион
description: Чтение свойств и связей объекта Граупполициуплоадеддефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9b7cc9e7623a4954934f6e236c22ce5042390059
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463842"
---
# <a name="get-grouppolicyuploadeddefinition"></a><span data-ttu-id="62e00-103">Получение Граупполициуплоадеддефинитион</span><span class="sxs-lookup"><span data-stu-id="62e00-103">Get groupPolicyUploadedDefinition</span></span>

<span data-ttu-id="62e00-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="62e00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62e00-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62e00-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62e00-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62e00-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62e00-107">Чтение свойств и связей объекта [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="62e00-107">Read properties and relationships of the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62e00-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="62e00-108">Prerequisites</span></span>
<span data-ttu-id="62e00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62e00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62e00-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62e00-111">Permission type</span></span>|<span data-ttu-id="62e00-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62e00-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62e00-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62e00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62e00-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="62e00-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="62e00-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62e00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62e00-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62e00-116">Not supported.</span></span>|
|<span data-ttu-id="62e00-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62e00-117">Application</span></span>|<span data-ttu-id="62e00-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="62e00-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62e00-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62e00-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62e00-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="62e00-120">Optional query parameters</span></span>
<span data-ttu-id="62e00-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="62e00-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62e00-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62e00-122">Request headers</span></span>
|<span data-ttu-id="62e00-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62e00-123">Header</span></span>|<span data-ttu-id="62e00-124">Значение</span><span class="sxs-lookup"><span data-stu-id="62e00-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62e00-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="62e00-125">Authorization</span></span>|<span data-ttu-id="62e00-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62e00-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62e00-127">Accept</span><span class="sxs-lookup"><span data-stu-id="62e00-127">Accept</span></span>|<span data-ttu-id="62e00-128">application/json</span><span class="sxs-lookup"><span data-stu-id="62e00-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62e00-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62e00-129">Request body</span></span>
<span data-ttu-id="62e00-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62e00-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62e00-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="62e00-131">Response</span></span>
<span data-ttu-id="62e00-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62e00-132">If successful, this method returns a `200 OK` response code and [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62e00-133">Пример</span><span class="sxs-lookup"><span data-stu-id="62e00-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="62e00-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="62e00-134">Request</span></span>
<span data-ttu-id="62e00-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62e00-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
```

### <a name="response"></a><span data-ttu-id="62e00-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="62e00-136">Response</span></span>
<span data-ttu-id="62e00-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62e00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
    "classType": "machine",
    "displayName": "Display Name value",
    "explainText": "Explain Text value",
    "categoryPath": "Category Path value",
    "supportedOn": "Supported On value",
    "policyType": "admxIngested",
    "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```





