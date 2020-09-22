---
title: Список Девицеманажементабстракткомплекссеттингинстанцес
description: Список свойств и связей объектов Девицеманажементабстракткомплекссеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce08033b08ad62a0ed22fbb7ebc5262c558696de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47974403"
---
# <a name="list-devicemanagementabstractcomplexsettinginstances"></a><span data-ttu-id="898cd-103">Список Девицеманажементабстракткомплекссеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="898cd-103">List deviceManagementAbstractComplexSettingInstances</span></span>

<span data-ttu-id="898cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="898cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="898cd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="898cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="898cd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="898cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="898cd-107">Список свойств и связей объектов [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="898cd-107">List properties and relationships of the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="898cd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="898cd-108">Prerequisites</span></span>
<span data-ttu-id="898cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="898cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="898cd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="898cd-111">Permission type</span></span>|<span data-ttu-id="898cd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="898cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="898cd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="898cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="898cd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="898cd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="898cd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="898cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="898cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="898cd-116">Not supported.</span></span>|
|<span data-ttu-id="898cd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="898cd-117">Application</span></span>|<span data-ttu-id="898cd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="898cd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="898cd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="898cd-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="898cd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="898cd-120">Request headers</span></span>
|<span data-ttu-id="898cd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="898cd-121">Header</span></span>|<span data-ttu-id="898cd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="898cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="898cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="898cd-123">Authorization</span></span>|<span data-ttu-id="898cd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="898cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="898cd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="898cd-125">Accept</span></span>|<span data-ttu-id="898cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="898cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="898cd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="898cd-127">Request body</span></span>
<span data-ttu-id="898cd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="898cd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="898cd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="898cd-129">Response</span></span>
<span data-ttu-id="898cd-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="898cd-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="898cd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="898cd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="898cd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="898cd-132">Request</span></span>
<span data-ttu-id="898cd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="898cd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="898cd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="898cd-134">Response</span></span>
<span data-ttu-id="898cd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="898cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
      "id": "433e9565-9565-433e-6595-3e4365953e43",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value",
      "implementationId": "Implementation Id value"
    }
  ]
}
```






