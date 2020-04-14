---
title: Список Девицеманажементколлектионсеттингинстанцес
description: Список свойств и связей объектов Девицеманажементколлектионсеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 54a21b20de9ed664bc88b9fdde77904fe4bf8af1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43428352"
---
# <a name="list-devicemanagementcollectionsettinginstances"></a><span data-ttu-id="70cec-103">Список Девицеманажементколлектионсеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="70cec-103">List deviceManagementCollectionSettingInstances</span></span>

<span data-ttu-id="70cec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70cec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70cec-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70cec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70cec-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70cec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70cec-107">Список свойств и связей объектов [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="70cec-107">List properties and relationships of the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70cec-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="70cec-108">Prerequisites</span></span>
<span data-ttu-id="70cec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70cec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70cec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70cec-111">Permission type</span></span>|<span data-ttu-id="70cec-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70cec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70cec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70cec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70cec-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="70cec-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="70cec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70cec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70cec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70cec-116">Not supported.</span></span>|
|<span data-ttu-id="70cec-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="70cec-117">Application</span></span>|<span data-ttu-id="70cec-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="70cec-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70cec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70cec-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="70cec-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="70cec-120">Request headers</span></span>
|<span data-ttu-id="70cec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70cec-121">Header</span></span>|<span data-ttu-id="70cec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="70cec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70cec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70cec-123">Authorization</span></span>|<span data-ttu-id="70cec-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70cec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70cec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="70cec-125">Accept</span></span>|<span data-ttu-id="70cec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70cec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70cec-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70cec-127">Request body</span></span>
<span data-ttu-id="70cec-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70cec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70cec-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="70cec-129">Response</span></span>
<span data-ttu-id="70cec-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70cec-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70cec-131">Пример</span><span class="sxs-lookup"><span data-stu-id="70cec-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="70cec-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="70cec-132">Request</span></span>
<span data-ttu-id="70cec-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70cec-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="70cec-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="70cec-134">Response</span></span>
<span data-ttu-id="70cec-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70cec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
      "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```



