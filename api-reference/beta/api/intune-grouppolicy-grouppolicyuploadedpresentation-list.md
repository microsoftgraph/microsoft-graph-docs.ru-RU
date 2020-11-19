---
title: Список Граупполициуплоадедпресентатионс
description: Список свойств и связей объектов Граупполициуплоадедпресентатион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 534110e18216c79eab18c6c8b1c8ddeed114d1c7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49224538"
---
# <a name="list-grouppolicyuploadedpresentations"></a><span data-ttu-id="8af52-103">Список Граупполициуплоадедпресентатионс</span><span class="sxs-lookup"><span data-stu-id="8af52-103">List groupPolicyUploadedPresentations</span></span>

<span data-ttu-id="8af52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8af52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8af52-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8af52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8af52-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8af52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8af52-107">Список свойств и связей объектов [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="8af52-107">List properties and relationships of the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8af52-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8af52-108">Prerequisites</span></span>
<span data-ttu-id="8af52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8af52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8af52-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8af52-111">Permission type</span></span>|<span data-ttu-id="8af52-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8af52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8af52-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8af52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8af52-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8af52-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8af52-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8af52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8af52-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8af52-116">Not supported.</span></span>|
|<span data-ttu-id="8af52-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8af52-117">Application</span></span>|<span data-ttu-id="8af52-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8af52-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8af52-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8af52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="8af52-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8af52-120">Request headers</span></span>
|<span data-ttu-id="8af52-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8af52-121">Header</span></span>|<span data-ttu-id="8af52-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8af52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8af52-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8af52-123">Authorization</span></span>|<span data-ttu-id="8af52-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8af52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8af52-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8af52-125">Accept</span></span>|<span data-ttu-id="8af52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8af52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8af52-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8af52-127">Request body</span></span>
<span data-ttu-id="8af52-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8af52-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8af52-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8af52-129">Response</span></span>
<span data-ttu-id="8af52-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8af52-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8af52-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8af52-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8af52-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8af52-132">Request</span></span>
<span data-ttu-id="8af52-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8af52-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="8af52-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8af52-134">Response</span></span>
<span data-ttu-id="8af52-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8af52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
      "label": "Label value",
      "id": "b9f611e8-11e8-b9f6-e811-f6b9e811f6b9",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




