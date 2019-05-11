---
title: Получение Граупполицидефинитион
description: Чтение свойств и связей объекта Граупполицидефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 28ee836810647582803837f8bdaf3ab975d76974
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905107"
---
# <a name="get-grouppolicydefinition"></a><span data-ttu-id="55b07-103">Получение Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="55b07-103">Get groupPolicyDefinition</span></span>

> <span data-ttu-id="55b07-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55b07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55b07-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55b07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55b07-106">Чтение свойств и связей объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="55b07-106">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55b07-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="55b07-107">Prerequisites</span></span>
<span data-ttu-id="55b07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55b07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55b07-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55b07-110">Permission type</span></span>|<span data-ttu-id="55b07-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55b07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55b07-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55b07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55b07-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="55b07-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="55b07-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55b07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55b07-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55b07-115">Not supported.</span></span>|
|<span data-ttu-id="55b07-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55b07-116">Application</span></span>|<span data-ttu-id="55b07-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55b07-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55b07-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55b07-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="55b07-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="55b07-119">Optional query parameters</span></span>
<span data-ttu-id="55b07-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="55b07-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55b07-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55b07-121">Request headers</span></span>
|<span data-ttu-id="55b07-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55b07-122">Header</span></span>|<span data-ttu-id="55b07-123">Значение</span><span class="sxs-lookup"><span data-stu-id="55b07-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55b07-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55b07-124">Authorization</span></span>|<span data-ttu-id="55b07-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55b07-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55b07-126">Accept</span><span class="sxs-lookup"><span data-stu-id="55b07-126">Accept</span></span>|<span data-ttu-id="55b07-127">application/json</span><span class="sxs-lookup"><span data-stu-id="55b07-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55b07-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55b07-128">Request body</span></span>
<span data-ttu-id="55b07-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55b07-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55b07-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="55b07-130">Response</span></span>
<span data-ttu-id="55b07-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55b07-131">If successful, this method returns a `200 OK` response code and [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55b07-132">Пример</span><span class="sxs-lookup"><span data-stu-id="55b07-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="55b07-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="55b07-133">Request</span></span>
<span data-ttu-id="55b07-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55b07-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
```

### <a name="response"></a><span data-ttu-id="55b07-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="55b07-135">Response</span></span>
<span data-ttu-id="55b07-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55b07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 435

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyDefinition",
    "classType": "machine",
    "displayName": "Display Name value",
    "explainText": "Explain Text value",
    "categoryPath": "Category Path value",
    "supportedOn": "Supported On value",
    "policyType": "admxIngested",
    "id": "f9607947-7947-f960-4779-60f9477960f9",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```




