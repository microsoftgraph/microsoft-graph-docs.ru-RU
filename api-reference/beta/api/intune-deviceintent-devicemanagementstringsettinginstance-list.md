---
title: Список Девицеманажементстрингсеттингинстанцес
description: Список свойств и связей объектов Девицеманажементстрингсеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14a3c55fd63fd129031d82576e58d28a054bf8d6
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945524"
---
# <a name="list-devicemanagementstringsettinginstances"></a><span data-ttu-id="4e113-103">Список Девицеманажементстрингсеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="4e113-103">List deviceManagementStringSettingInstances</span></span>

> <span data-ttu-id="4e113-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e113-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e113-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e113-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e113-106">Список свойств и связей объектов [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="4e113-106">List properties and relationships of the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e113-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4e113-107">Prerequisites</span></span>
<span data-ttu-id="4e113-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e113-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e113-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e113-110">Permission type</span></span>|<span data-ttu-id="4e113-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e113-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e113-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e113-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e113-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e113-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4e113-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e113-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e113-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e113-115">Not supported.</span></span>|
|<span data-ttu-id="4e113-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e113-116">Application</span></span>|<span data-ttu-id="4e113-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e113-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e113-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e113-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4e113-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4e113-119">Request headers</span></span>
|<span data-ttu-id="4e113-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e113-120">Header</span></span>|<span data-ttu-id="4e113-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4e113-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e113-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e113-122">Authorization</span></span>|<span data-ttu-id="4e113-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e113-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e113-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4e113-124">Accept</span></span>|<span data-ttu-id="4e113-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e113-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e113-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e113-126">Request body</span></span>
<span data-ttu-id="4e113-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e113-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e113-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e113-128">Response</span></span>
<span data-ttu-id="4e113-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e113-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e113-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4e113-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e113-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e113-131">Request</span></span>
<span data-ttu-id="4e113-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e113-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="4e113-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e113-133">Response</span></span>
<span data-ttu-id="4e113-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e113-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





