---
title: Получение Граупполицидефинитион
description: Чтение свойств и связей объекта Граупполицидефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 811baa15f7abcfa9857827f621b13be01464578c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306011"
---
# <a name="get-grouppolicydefinition"></a><span data-ttu-id="34705-103">Получение Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="34705-103">Get groupPolicyDefinition</span></span>

<span data-ttu-id="34705-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34705-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34705-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34705-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34705-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34705-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34705-107">Чтение свойств и связей объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="34705-107">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34705-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="34705-108">Prerequisites</span></span>
<span data-ttu-id="34705-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34705-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34705-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34705-111">Permission type</span></span>|<span data-ttu-id="34705-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34705-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34705-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34705-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34705-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34705-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="34705-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34705-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34705-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34705-116">Not supported.</span></span>|
|<span data-ttu-id="34705-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34705-117">Application</span></span>|<span data-ttu-id="34705-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34705-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34705-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34705-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="34705-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="34705-120">Optional query parameters</span></span>
<span data-ttu-id="34705-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="34705-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34705-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34705-122">Request headers</span></span>
|<span data-ttu-id="34705-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34705-123">Header</span></span>|<span data-ttu-id="34705-124">Значение</span><span class="sxs-lookup"><span data-stu-id="34705-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34705-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34705-125">Authorization</span></span>|<span data-ttu-id="34705-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34705-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34705-127">Accept</span><span class="sxs-lookup"><span data-stu-id="34705-127">Accept</span></span>|<span data-ttu-id="34705-128">application/json</span><span class="sxs-lookup"><span data-stu-id="34705-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34705-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34705-129">Request body</span></span>
<span data-ttu-id="34705-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34705-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34705-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="34705-131">Response</span></span>
<span data-ttu-id="34705-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34705-132">If successful, this method returns a `200 OK` response code and [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34705-133">Пример</span><span class="sxs-lookup"><span data-stu-id="34705-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="34705-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="34705-134">Request</span></span>
<span data-ttu-id="34705-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34705-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
```

### <a name="response"></a><span data-ttu-id="34705-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="34705-136">Response</span></span>
<span data-ttu-id="34705-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34705-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 505

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyDefinition",
    "classType": "machine",
    "displayName": "Display Name value",
    "explainText": "Explain Text value",
    "categoryPath": "Category Path value",
    "supportedOn": "Supported On value",
    "policyType": "admxIngested",
    "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
    "id": "f9607947-7947-f960-4779-60f9477960f9",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```




