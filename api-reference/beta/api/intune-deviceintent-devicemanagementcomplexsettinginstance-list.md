---
title: Список Девицеманажементкомплекссеттингинстанцес
description: Список свойств и связей объектов Девицеманажементкомплекссеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c1eb19ee400c6e131b5ae0aafd97a7fc2298985
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43329110"
---
# <a name="list-devicemanagementcomplexsettinginstances"></a><span data-ttu-id="ec333-103">Список Девицеманажементкомплекссеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="ec333-103">List deviceManagementComplexSettingInstances</span></span>

<span data-ttu-id="ec333-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec333-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec333-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec333-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec333-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec333-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec333-107">Список свойств и связей объектов [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="ec333-107">List properties and relationships of the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec333-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ec333-108">Prerequisites</span></span>
<span data-ttu-id="ec333-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec333-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec333-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec333-111">Permission type</span></span>|<span data-ttu-id="ec333-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec333-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec333-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec333-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec333-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec333-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ec333-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec333-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec333-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec333-116">Not supported.</span></span>|
|<span data-ttu-id="ec333-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec333-117">Application</span></span>|<span data-ttu-id="ec333-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec333-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec333-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec333-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="ec333-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ec333-120">Request headers</span></span>
|<span data-ttu-id="ec333-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec333-121">Header</span></span>|<span data-ttu-id="ec333-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ec333-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec333-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec333-123">Authorization</span></span>|<span data-ttu-id="ec333-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec333-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec333-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ec333-125">Accept</span></span>|<span data-ttu-id="ec333-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec333-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec333-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ec333-127">Request body</span></span>
<span data-ttu-id="ec333-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec333-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec333-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec333-129">Response</span></span>
<span data-ttu-id="ec333-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec333-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec333-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ec333-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec333-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec333-132">Request</span></span>
<span data-ttu-id="ec333-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec333-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="ec333-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec333-134">Response</span></span>
<span data-ttu-id="ec333-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec333-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



