---
title: Получение Граупполицидефинитионфиле
description: Чтение свойств и связей объекта Граупполицидефинитионфиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7912443afd5fd1fb1e4ac6ffe4b4eda2598b1a2a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454532"
---
# <a name="get-grouppolicydefinitionfile"></a><span data-ttu-id="a4e79-103">Получение Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="a4e79-103">Get groupPolicyDefinitionFile</span></span>

<span data-ttu-id="a4e79-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4e79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4e79-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4e79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4e79-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4e79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4e79-107">Чтение свойств и связей объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="a4e79-107">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4e79-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a4e79-108">Prerequisites</span></span>
<span data-ttu-id="a4e79-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4e79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4e79-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4e79-111">Permission type</span></span>|<span data-ttu-id="a4e79-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4e79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4e79-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4e79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4e79-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4e79-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a4e79-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4e79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4e79-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4e79-116">Not supported.</span></span>|
|<span data-ttu-id="a4e79-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4e79-117">Application</span></span>|<span data-ttu-id="a4e79-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4e79-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4e79-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4e79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitionFile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4e79-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a4e79-120">Optional query parameters</span></span>
<span data-ttu-id="a4e79-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a4e79-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4e79-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4e79-122">Request headers</span></span>
|<span data-ttu-id="a4e79-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4e79-123">Header</span></span>|<span data-ttu-id="a4e79-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a4e79-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4e79-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4e79-125">Authorization</span></span>|<span data-ttu-id="a4e79-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4e79-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4e79-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a4e79-127">Accept</span></span>|<span data-ttu-id="a4e79-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a4e79-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4e79-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a4e79-129">Request body</span></span>
<span data-ttu-id="a4e79-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4e79-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4e79-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4e79-131">Response</span></span>
<span data-ttu-id="a4e79-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a4e79-132">If successful, this method returns a `200 OK` response code and [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4e79-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a4e79-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4e79-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4e79-134">Request</span></span>
<span data-ttu-id="a4e79-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4e79-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
```

### <a name="response"></a><span data-ttu-id="a4e79-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4e79-136">Response</span></span>
<span data-ttu-id="a4e79-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4e79-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 514

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
    "displayName": "Display Name value",
    "description": "Description value",
    "languageCodes": [
      "Language Codes value"
    ],
    "targetPrefix": "Target Prefix value",
    "targetNamespace": "Target Namespace value",
    "policyType": "admxIngested",
    "revision": "Revision value",
    "id": "940aa2a1-a2a1-940a-a1a2-0a94a1a20a94",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```



