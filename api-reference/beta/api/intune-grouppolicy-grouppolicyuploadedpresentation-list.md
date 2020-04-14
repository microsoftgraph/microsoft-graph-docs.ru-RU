---
title: Список Граупполициуплоадедпресентатионс
description: Список свойств и связей объектов Граупполициуплоадедпресентатион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fe4a8e0b98d56814ef931c3b6b05f9db445900bf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440832"
---
# <a name="list-grouppolicyuploadedpresentations"></a><span data-ttu-id="0d03a-103">Список Граупполициуплоадедпресентатионс</span><span class="sxs-lookup"><span data-stu-id="0d03a-103">List groupPolicyUploadedPresentations</span></span>

<span data-ttu-id="0d03a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d03a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d03a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d03a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d03a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d03a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d03a-107">Список свойств и связей объектов [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="0d03a-107">List properties and relationships of the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d03a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0d03a-108">Prerequisites</span></span>
<span data-ttu-id="0d03a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d03a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d03a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d03a-111">Permission type</span></span>|<span data-ttu-id="0d03a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d03a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d03a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d03a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d03a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d03a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0d03a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d03a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d03a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d03a-116">Not supported.</span></span>|
|<span data-ttu-id="0d03a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0d03a-117">Application</span></span>|<span data-ttu-id="0d03a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d03a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d03a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d03a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="0d03a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0d03a-120">Request headers</span></span>
|<span data-ttu-id="0d03a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d03a-121">Header</span></span>|<span data-ttu-id="0d03a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0d03a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d03a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d03a-123">Authorization</span></span>|<span data-ttu-id="0d03a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d03a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d03a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0d03a-125">Accept</span></span>|<span data-ttu-id="0d03a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d03a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d03a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d03a-127">Request body</span></span>
<span data-ttu-id="0d03a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d03a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d03a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d03a-129">Response</span></span>
<span data-ttu-id="0d03a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d03a-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d03a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0d03a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d03a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d03a-132">Request</span></span>
<span data-ttu-id="0d03a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d03a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="0d03a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d03a-134">Response</span></span>
<span data-ttu-id="0d03a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d03a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



