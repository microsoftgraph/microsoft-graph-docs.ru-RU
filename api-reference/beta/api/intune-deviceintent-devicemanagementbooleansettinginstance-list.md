---
title: Список Девицеманажементбулеансеттингинстанцес
description: Список свойств и связей объектов Девицеманажементбулеансеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a747a21e8a176dcf00f5cdbb68ceb3d0b1417095
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49235387"
---
# <a name="list-devicemanagementbooleansettinginstances"></a><span data-ttu-id="02d75-103">Список Девицеманажементбулеансеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="02d75-103">List deviceManagementBooleanSettingInstances</span></span>

<span data-ttu-id="02d75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02d75-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02d75-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02d75-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02d75-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02d75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02d75-107">Список свойств и связей объектов [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="02d75-107">List properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02d75-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="02d75-108">Prerequisites</span></span>
<span data-ttu-id="02d75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02d75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02d75-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02d75-111">Permission type</span></span>|<span data-ttu-id="02d75-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="02d75-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02d75-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02d75-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02d75-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="02d75-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="02d75-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02d75-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02d75-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02d75-116">Not supported.</span></span>|
|<span data-ttu-id="02d75-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="02d75-117">Application</span></span>|<span data-ttu-id="02d75-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="02d75-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02d75-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02d75-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="02d75-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="02d75-120">Request headers</span></span>
|<span data-ttu-id="02d75-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02d75-121">Header</span></span>|<span data-ttu-id="02d75-122">Значение</span><span class="sxs-lookup"><span data-stu-id="02d75-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02d75-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02d75-123">Authorization</span></span>|<span data-ttu-id="02d75-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02d75-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02d75-125">Accept</span><span class="sxs-lookup"><span data-stu-id="02d75-125">Accept</span></span>|<span data-ttu-id="02d75-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02d75-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02d75-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02d75-127">Request body</span></span>
<span data-ttu-id="02d75-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02d75-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02d75-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="02d75-129">Response</span></span>
<span data-ttu-id="02d75-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="02d75-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02d75-131">Пример</span><span class="sxs-lookup"><span data-stu-id="02d75-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="02d75-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="02d75-132">Request</span></span>
<span data-ttu-id="02d75-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02d75-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="02d75-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="02d75-134">Response</span></span>
<span data-ttu-id="02d75-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02d75-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
      "id": "bb9b0041-0041-bb9b-4100-9bbb41009bbb",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value",
      "value": true
    }
  ]
}
```




