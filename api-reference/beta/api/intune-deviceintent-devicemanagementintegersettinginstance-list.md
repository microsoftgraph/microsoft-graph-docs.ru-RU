---
title: Список Девицеманажементинтежерсеттингинстанцес
description: Список свойств и связей объектов Девицеманажементинтежерсеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 66a7b0c7bad668632cf2f647461322928fec644e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49289680"
---
# <a name="list-devicemanagementintegersettinginstances"></a><span data-ttu-id="f9c89-103">Список Девицеманажементинтежерсеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="f9c89-103">List deviceManagementIntegerSettingInstances</span></span>

<span data-ttu-id="f9c89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9c89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9c89-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9c89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9c89-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9c89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9c89-107">Список свойств и связей объектов [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="f9c89-107">List properties and relationships of the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9c89-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f9c89-108">Prerequisites</span></span>
<span data-ttu-id="f9c89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9c89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9c89-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9c89-111">Permission type</span></span>|<span data-ttu-id="f9c89-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9c89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9c89-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9c89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9c89-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9c89-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f9c89-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9c89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9c89-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9c89-116">Not supported.</span></span>|
|<span data-ttu-id="f9c89-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9c89-117">Application</span></span>|<span data-ttu-id="f9c89-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9c89-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9c89-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9c89-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f9c89-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f9c89-120">Request headers</span></span>
|<span data-ttu-id="f9c89-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9c89-121">Header</span></span>|<span data-ttu-id="f9c89-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f9c89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9c89-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9c89-123">Authorization</span></span>|<span data-ttu-id="f9c89-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9c89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9c89-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f9c89-125">Accept</span></span>|<span data-ttu-id="f9c89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9c89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9c89-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9c89-127">Request body</span></span>
<span data-ttu-id="f9c89-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9c89-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9c89-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9c89-129">Response</span></span>
<span data-ttu-id="f9c89-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9c89-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9c89-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f9c89-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9c89-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9c89-132">Request</span></span>
<span data-ttu-id="f9c89-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9c89-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="f9c89-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9c89-134">Response</span></span>
<span data-ttu-id="f9c89-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9c89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
      "id": "60468ce7-8ce7-6046-e78c-4660e78c4660",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value",
      "value": 5
    }
  ]
}
```




