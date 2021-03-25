---
title: List groupPolicyPresentationValueBooleans
description: Список свойств и связей объектов groupPolicyPresentationValueBoolean.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dd9eb90ff6d0de965d9c1204a08f79f87d6ca6e1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157234"
---
# <a name="list-grouppolicypresentationvaluebooleans"></a><span data-ttu-id="a10de-103">List groupPolicyPresentationValueBooleans</span><span class="sxs-lookup"><span data-stu-id="a10de-103">List groupPolicyPresentationValueBooleans</span></span>

<span data-ttu-id="a10de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a10de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a10de-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a10de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a10de-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a10de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a10de-107">Список свойств и связей объектов [groupPolicyPresentationValueBoolean.](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)</span><span class="sxs-lookup"><span data-stu-id="a10de-107">List properties and relationships of the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a10de-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a10de-108">Prerequisites</span></span>
<span data-ttu-id="a10de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a10de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a10de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a10de-111">Permission type</span></span>|<span data-ttu-id="a10de-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a10de-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a10de-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a10de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a10de-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a10de-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a10de-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a10de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a10de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a10de-116">Not supported.</span></span>|
|<span data-ttu-id="a10de-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a10de-117">Application</span></span>|<span data-ttu-id="a10de-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a10de-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a10de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a10de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="a10de-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a10de-120">Request headers</span></span>
|<span data-ttu-id="a10de-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a10de-121">Header</span></span>|<span data-ttu-id="a10de-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a10de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a10de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a10de-123">Authorization</span></span>|<span data-ttu-id="a10de-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a10de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a10de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a10de-125">Accept</span></span>|<span data-ttu-id="a10de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a10de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a10de-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a10de-127">Request body</span></span>
<span data-ttu-id="a10de-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a10de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a10de-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a10de-129">Response</span></span>
<span data-ttu-id="a10de-130">В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a10de-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a10de-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a10de-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a10de-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a10de-132">Request</span></span>
<span data-ttu-id="a10de-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a10de-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="a10de-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a10de-134">Response</span></span>
<span data-ttu-id="a10de-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a10de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 320

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "id": "be61344f-344f-be61-4f34-61be4f3461be",
      "value": true
    }
  ]
}
```




