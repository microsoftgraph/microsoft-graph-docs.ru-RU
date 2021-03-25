---
title: List groupPolicyUploadedDefinitions
description: Список свойств и связей объектов groupPolicyUploadedDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 21466e44dc0945a8449311dd3e20d085c124cda6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156963"
---
# <a name="list-grouppolicyuploadeddefinitions"></a><span data-ttu-id="14a6a-103">List groupPolicyUploadedDefinitions</span><span class="sxs-lookup"><span data-stu-id="14a6a-103">List groupPolicyUploadedDefinitions</span></span>

<span data-ttu-id="14a6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14a6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14a6a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14a6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14a6a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14a6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14a6a-107">Список свойств и связей объектов [groupPolicyUploadedDefinition.](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)</span><span class="sxs-lookup"><span data-stu-id="14a6a-107">List properties and relationships of the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14a6a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="14a6a-108">Prerequisites</span></span>
<span data-ttu-id="14a6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14a6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14a6a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14a6a-111">Permission type</span></span>|<span data-ttu-id="14a6a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14a6a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14a6a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14a6a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14a6a-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a6a-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14a6a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14a6a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14a6a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14a6a-116">Not supported.</span></span>|
|<span data-ttu-id="14a6a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="14a6a-117">Application</span></span>|<span data-ttu-id="14a6a-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a6a-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14a6a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14a6a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyDefinitions
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
```

## <a name="request-headers"></a><span data-ttu-id="14a6a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="14a6a-120">Request headers</span></span>
|<span data-ttu-id="14a6a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14a6a-121">Header</span></span>|<span data-ttu-id="14a6a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="14a6a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14a6a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14a6a-123">Authorization</span></span>|<span data-ttu-id="14a6a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14a6a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14a6a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14a6a-125">Accept</span></span>|<span data-ttu-id="14a6a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14a6a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14a6a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14a6a-127">Request body</span></span>
<span data-ttu-id="14a6a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14a6a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14a6a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="14a6a-129">Response</span></span>
<span data-ttu-id="14a6a-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="14a6a-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14a6a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="14a6a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="14a6a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="14a6a-132">Request</span></span>
<span data-ttu-id="14a6a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14a6a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions
```

### <a name="response"></a><span data-ttu-id="14a6a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="14a6a-134">Response</span></span>
<span data-ttu-id="14a6a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14a6a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




