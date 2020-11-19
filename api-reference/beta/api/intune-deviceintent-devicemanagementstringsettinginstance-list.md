---
title: Список Девицеманажементстрингсеттингинстанцес
description: Список свойств и связей объектов Девицеманажементстрингсеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba9f1ae9348ce2c75336fd3fd8a25c94f97c429c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300157"
---
# <a name="list-devicemanagementstringsettinginstances"></a><span data-ttu-id="bac16-103">Список Девицеманажементстрингсеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="bac16-103">List deviceManagementStringSettingInstances</span></span>

<span data-ttu-id="bac16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bac16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bac16-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bac16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bac16-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bac16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bac16-107">Список свойств и связей объектов [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="bac16-107">List properties and relationships of the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bac16-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bac16-108">Prerequisites</span></span>
<span data-ttu-id="bac16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bac16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bac16-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bac16-111">Permission type</span></span>|<span data-ttu-id="bac16-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bac16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bac16-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bac16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bac16-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bac16-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bac16-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bac16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bac16-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bac16-116">Not supported.</span></span>|
|<span data-ttu-id="bac16-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bac16-117">Application</span></span>|<span data-ttu-id="bac16-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bac16-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bac16-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bac16-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="bac16-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bac16-120">Request headers</span></span>
|<span data-ttu-id="bac16-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bac16-121">Header</span></span>|<span data-ttu-id="bac16-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bac16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bac16-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bac16-123">Authorization</span></span>|<span data-ttu-id="bac16-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bac16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bac16-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bac16-125">Accept</span></span>|<span data-ttu-id="bac16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bac16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bac16-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bac16-127">Request body</span></span>
<span data-ttu-id="bac16-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bac16-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bac16-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bac16-129">Response</span></span>
<span data-ttu-id="bac16-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bac16-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bac16-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bac16-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bac16-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bac16-132">Request</span></span>
<span data-ttu-id="bac16-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bac16-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="bac16-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bac16-134">Response</span></span>
<span data-ttu-id="bac16-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bac16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
      "id": "fef30638-0638-fef3-3806-f3fe3806f3fe",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value",
      "value": "Value value"
    }
  ]
}
```




