---
title: Список Граупполициуплоадеддефинитионс
description: Список свойств и связей объектов Граупполициуплоадеддефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f7549d04e728d7b9aeb15185909fe0d81fb32cdd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463835"
---
# <a name="list-grouppolicyuploadeddefinitions"></a><span data-ttu-id="8bbf0-103">Список Граупполициуплоадеддефинитионс</span><span class="sxs-lookup"><span data-stu-id="8bbf0-103">List groupPolicyUploadedDefinitions</span></span>

<span data-ttu-id="8bbf0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8bbf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8bbf0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bbf0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bbf0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bbf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bbf0-107">Список свойств и связей объектов [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="8bbf0-107">List properties and relationships of the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bbf0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8bbf0-108">Prerequisites</span></span>
<span data-ttu-id="8bbf0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bbf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bbf0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bbf0-111">Permission type</span></span>|<span data-ttu-id="8bbf0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bbf0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bbf0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bbf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8bbf0-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bbf0-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8bbf0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bbf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bbf0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bbf0-116">Not supported.</span></span>|
|<span data-ttu-id="8bbf0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bbf0-117">Application</span></span>|<span data-ttu-id="8bbf0-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bbf0-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bbf0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bbf0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyDefinitions
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
```

## <a name="request-headers"></a><span data-ttu-id="8bbf0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8bbf0-120">Request headers</span></span>
|<span data-ttu-id="8bbf0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8bbf0-121">Header</span></span>|<span data-ttu-id="8bbf0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8bbf0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bbf0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bbf0-123">Authorization</span></span>|<span data-ttu-id="8bbf0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bbf0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bbf0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8bbf0-125">Accept</span></span>|<span data-ttu-id="8bbf0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8bbf0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bbf0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bbf0-127">Request body</span></span>
<span data-ttu-id="8bbf0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8bbf0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bbf0-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8bbf0-129">Response</span></span>
<span data-ttu-id="8bbf0-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8bbf0-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bbf0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8bbf0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bbf0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bbf0-132">Request</span></span>
<span data-ttu-id="8bbf0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bbf0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions
```

### <a name="response"></a><span data-ttu-id="8bbf0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bbf0-134">Response</span></span>
<span data-ttu-id="8bbf0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8bbf0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 475

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
      "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```





