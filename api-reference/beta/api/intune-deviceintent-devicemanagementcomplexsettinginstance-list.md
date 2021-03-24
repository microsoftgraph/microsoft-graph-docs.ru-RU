---
title: Список deviceManagementComplexSettingInstances
description: Список свойств и связей объектов deviceManagementComplexSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5bb53b4537e8e886ccd7223c24832f5e3b8e3b91
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127133"
---
# <a name="list-devicemanagementcomplexsettinginstances"></a><span data-ttu-id="6a627-103">Список deviceManagementComplexSettingInstances</span><span class="sxs-lookup"><span data-stu-id="6a627-103">List deviceManagementComplexSettingInstances</span></span>

<span data-ttu-id="6a627-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a627-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a627-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a627-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a627-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a627-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a627-107">Список свойств и связей [объектов deviceManagementComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="6a627-107">List properties and relationships of the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a627-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6a627-108">Prerequisites</span></span>
<span data-ttu-id="6a627-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a627-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a627-111">Permission type</span></span>|<span data-ttu-id="6a627-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a627-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a627-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a627-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a627-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a627-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a627-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a627-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a627-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a627-116">Not supported.</span></span>|
|<span data-ttu-id="6a627-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6a627-117">Application</span></span>|<span data-ttu-id="6a627-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a627-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a627-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a627-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/settings
GET /deviceManagement/templates/{deviceManagementTemplateId}/settings
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="6a627-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6a627-120">Request headers</span></span>
|<span data-ttu-id="6a627-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a627-121">Header</span></span>|<span data-ttu-id="6a627-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6a627-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a627-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a627-123">Authorization</span></span>|<span data-ttu-id="6a627-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a627-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a627-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6a627-125">Accept</span></span>|<span data-ttu-id="6a627-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a627-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a627-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a627-127">Request body</span></span>
<span data-ttu-id="6a627-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a627-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a627-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a627-129">Response</span></span>
<span data-ttu-id="6a627-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6a627-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a627-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6a627-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a627-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a627-132">Request</span></span>
<span data-ttu-id="6a627-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a627-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="6a627-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a627-134">Response</span></span>
<span data-ttu-id="6a627-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a627-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 256

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
      "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```




