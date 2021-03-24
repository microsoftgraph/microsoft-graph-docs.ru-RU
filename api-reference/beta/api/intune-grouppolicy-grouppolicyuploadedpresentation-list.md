---
title: List groupPolicyUploadedPresentations
description: Список свойств и связей объектов groupPolicyUploadedPresentation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56d8dde5188821ec7e4ec5f7e7ddce413ee00e90
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145546"
---
# <a name="list-grouppolicyuploadedpresentations"></a><span data-ttu-id="72c29-103">List groupPolicyUploadedPresentations</span><span class="sxs-lookup"><span data-stu-id="72c29-103">List groupPolicyUploadedPresentations</span></span>

<span data-ttu-id="72c29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72c29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72c29-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72c29-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72c29-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72c29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72c29-107">Список свойств и связей [объектов groupPolicyUploadedPresentation.](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)</span><span class="sxs-lookup"><span data-stu-id="72c29-107">List properties and relationships of the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72c29-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="72c29-108">Prerequisites</span></span>
<span data-ttu-id="72c29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72c29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72c29-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72c29-111">Permission type</span></span>|<span data-ttu-id="72c29-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72c29-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72c29-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72c29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72c29-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72c29-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72c29-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72c29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72c29-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72c29-116">Not supported.</span></span>|
|<span data-ttu-id="72c29-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="72c29-117">Application</span></span>|<span data-ttu-id="72c29-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72c29-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72c29-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72c29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="72c29-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="72c29-120">Request headers</span></span>
|<span data-ttu-id="72c29-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72c29-121">Header</span></span>|<span data-ttu-id="72c29-122">Значение</span><span class="sxs-lookup"><span data-stu-id="72c29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72c29-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72c29-123">Authorization</span></span>|<span data-ttu-id="72c29-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72c29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72c29-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72c29-125">Accept</span></span>|<span data-ttu-id="72c29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72c29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72c29-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72c29-127">Request body</span></span>
<span data-ttu-id="72c29-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72c29-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72c29-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="72c29-129">Response</span></span>
<span data-ttu-id="72c29-130">В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="72c29-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72c29-131">Пример</span><span class="sxs-lookup"><span data-stu-id="72c29-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="72c29-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="72c29-132">Request</span></span>
<span data-ttu-id="72c29-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72c29-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="72c29-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="72c29-134">Response</span></span>
<span data-ttu-id="72c29-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72c29-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




