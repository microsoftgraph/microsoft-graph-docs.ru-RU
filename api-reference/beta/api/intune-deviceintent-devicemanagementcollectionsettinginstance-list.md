---
title: Список Девицеманажементколлектионсеттингинстанцес
description: Список свойств и связей объектов Девицеманажементколлектионсеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a9126442f348d90ba0ab14c3d279441af382cf32
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42472214"
---
# <a name="list-devicemanagementcollectionsettinginstances"></a><span data-ttu-id="7444e-103">Список Девицеманажементколлектионсеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="7444e-103">List deviceManagementCollectionSettingInstances</span></span>

<span data-ttu-id="7444e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7444e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7444e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7444e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7444e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7444e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7444e-107">Список свойств и связей объектов [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="7444e-107">List properties and relationships of the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7444e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7444e-108">Prerequisites</span></span>
<span data-ttu-id="7444e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7444e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7444e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7444e-111">Permission type</span></span>|<span data-ttu-id="7444e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7444e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7444e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7444e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7444e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7444e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7444e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7444e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7444e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7444e-116">Not supported.</span></span>|
|<span data-ttu-id="7444e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7444e-117">Application</span></span>|<span data-ttu-id="7444e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7444e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7444e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7444e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="7444e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7444e-120">Request headers</span></span>
|<span data-ttu-id="7444e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7444e-121">Header</span></span>|<span data-ttu-id="7444e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7444e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7444e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7444e-123">Authorization</span></span>|<span data-ttu-id="7444e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7444e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7444e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7444e-125">Accept</span></span>|<span data-ttu-id="7444e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7444e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7444e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7444e-127">Request body</span></span>
<span data-ttu-id="7444e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7444e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7444e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7444e-129">Response</span></span>
<span data-ttu-id="7444e-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7444e-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7444e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7444e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7444e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7444e-132">Request</span></span>
<span data-ttu-id="7444e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7444e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="7444e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7444e-134">Response</span></span>
<span data-ttu-id="7444e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7444e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





