---
title: Получение Граупполициуплоадедпресентатион
description: Чтение свойств и связей объекта Граупполициуплоадедпресентатион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2ec14e961c46ae7ea1aad2af17ef0c8f7a143cc3
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161720"
---
# <a name="get-grouppolicyuploadedpresentation"></a><span data-ttu-id="03b91-103">Получение Граупполициуплоадедпресентатион</span><span class="sxs-lookup"><span data-stu-id="03b91-103">Get groupPolicyUploadedPresentation</span></span>

> <span data-ttu-id="03b91-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03b91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03b91-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03b91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03b91-106">Чтение свойств и связей объекта [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="03b91-106">Read properties and relationships of the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03b91-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03b91-107">Prerequisites</span></span>
<span data-ttu-id="03b91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03b91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03b91-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03b91-110">Permission type</span></span>|<span data-ttu-id="03b91-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03b91-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03b91-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03b91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03b91-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="03b91-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="03b91-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03b91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03b91-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03b91-115">Not supported.</span></span>|
|<span data-ttu-id="03b91-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03b91-116">Application</span></span>|<span data-ttu-id="03b91-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="03b91-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03b91-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03b91-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03b91-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="03b91-119">Optional query parameters</span></span>
<span data-ttu-id="03b91-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="03b91-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03b91-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03b91-121">Request headers</span></span>
|<span data-ttu-id="03b91-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03b91-122">Header</span></span>|<span data-ttu-id="03b91-123">Значение</span><span class="sxs-lookup"><span data-stu-id="03b91-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03b91-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="03b91-124">Authorization</span></span>|<span data-ttu-id="03b91-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03b91-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03b91-126">Accept</span><span class="sxs-lookup"><span data-stu-id="03b91-126">Accept</span></span>|<span data-ttu-id="03b91-127">application/json</span><span class="sxs-lookup"><span data-stu-id="03b91-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03b91-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03b91-128">Request body</span></span>
<span data-ttu-id="03b91-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03b91-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03b91-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="03b91-130">Response</span></span>
<span data-ttu-id="03b91-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03b91-131">If successful, this method returns a `200 OK` response code and [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03b91-132">Пример</span><span class="sxs-lookup"><span data-stu-id="03b91-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="03b91-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="03b91-133">Request</span></span>
<span data-ttu-id="03b91-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03b91-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="03b91-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="03b91-135">Response</span></span>
<span data-ttu-id="03b91-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03b91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
    "label": "Label value",
    "id": "b9f611e8-11e8-b9f6-e811-f6b9e811f6b9",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```





