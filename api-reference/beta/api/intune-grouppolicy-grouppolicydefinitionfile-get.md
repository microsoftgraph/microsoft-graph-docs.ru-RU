---
title: Get groupPolicyDefinitionFile
description: Чтение свойств и связей объекта groupPolicyDefinitionFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 43aaffa2246c2ecf1c78c77a93f6c4b98cb0d217
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158901"
---
# <a name="get-grouppolicydefinitionfile"></a><span data-ttu-id="515c4-103">Get groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="515c4-103">Get groupPolicyDefinitionFile</span></span>

<span data-ttu-id="515c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="515c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="515c4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="515c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="515c4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="515c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="515c4-107">Чтение свойств и связей объекта [groupPolicyDefinitionFile.](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="515c4-107">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="515c4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="515c4-108">Prerequisites</span></span>
<span data-ttu-id="515c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="515c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="515c4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="515c4-111">Permission type</span></span>|<span data-ttu-id="515c4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="515c4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="515c4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="515c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="515c4-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="515c4-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="515c4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="515c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="515c4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="515c4-116">Not supported.</span></span>|
|<span data-ttu-id="515c4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="515c4-117">Application</span></span>|<span data-ttu-id="515c4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="515c4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="515c4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="515c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitionFile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="515c4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="515c4-120">Optional query parameters</span></span>
<span data-ttu-id="515c4-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="515c4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="515c4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="515c4-122">Request headers</span></span>
|<span data-ttu-id="515c4-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="515c4-123">Header</span></span>|<span data-ttu-id="515c4-124">Значение</span><span class="sxs-lookup"><span data-stu-id="515c4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="515c4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="515c4-125">Authorization</span></span>|<span data-ttu-id="515c4-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="515c4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="515c4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="515c4-127">Accept</span></span>|<span data-ttu-id="515c4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="515c4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="515c4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="515c4-129">Request body</span></span>
<span data-ttu-id="515c4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="515c4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="515c4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="515c4-131">Response</span></span>
<span data-ttu-id="515c4-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="515c4-132">If successful, this method returns a `200 OK` response code and [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="515c4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="515c4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="515c4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="515c4-134">Request</span></span>
<span data-ttu-id="515c4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="515c4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
```

### <a name="response"></a><span data-ttu-id="515c4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="515c4-136">Response</span></span>
<span data-ttu-id="515c4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="515c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




