---
title: Получение Граупполицидефинитионфиле
description: Чтение свойств и связей объекта Граупполицидефинитионфиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9d1b589b624cb3168d93ae5371dc13a59b7e189
ms.sourcegitcommit: 705b32b9a64516d8138fab34c173b7df4f78a6ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/05/2019
ms.locfileid: "35576398"
---
# <a name="get-grouppolicydefinitionfile"></a><span data-ttu-id="2db10-103">Получение Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="2db10-103">Get groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="2db10-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2db10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2db10-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2db10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2db10-106">Чтение свойств и связей объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="2db10-106">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2db10-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2db10-107">Prerequisites</span></span>
<span data-ttu-id="2db10-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2db10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2db10-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2db10-110">Permission type</span></span>|<span data-ttu-id="2db10-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2db10-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2db10-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2db10-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2db10-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2db10-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2db10-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2db10-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2db10-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2db10-115">Not supported.</span></span>|
|<span data-ttu-id="2db10-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2db10-116">Application</span></span>|<span data-ttu-id="2db10-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2db10-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2db10-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2db10-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2db10-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2db10-119">Optional query parameters</span></span>
<span data-ttu-id="2db10-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2db10-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2db10-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2db10-121">Request headers</span></span>
|<span data-ttu-id="2db10-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2db10-122">Header</span></span>|<span data-ttu-id="2db10-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2db10-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2db10-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2db10-124">Authorization</span></span>|<span data-ttu-id="2db10-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2db10-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2db10-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2db10-126">Accept</span></span>|<span data-ttu-id="2db10-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2db10-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2db10-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2db10-128">Request body</span></span>
<span data-ttu-id="2db10-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2db10-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2db10-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2db10-130">Response</span></span>
<span data-ttu-id="2db10-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2db10-131">If successful, this method returns a `200 OK` response code and [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2db10-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2db10-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2db10-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2db10-133">Request</span></span>
<span data-ttu-id="2db10-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2db10-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
```

### <a name="response"></a><span data-ttu-id="2db10-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2db10-135">Response</span></span>
<span data-ttu-id="2db10-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2db10-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



