---
title: Список Девицеманажементинтежерсеттингинстанцес
description: Список свойств и связей объектов Девицеманажементинтежерсеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 649f241ac8030bbd5c2b08366710737f6e679cae
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945916"
---
# <a name="list-devicemanagementintegersettinginstances"></a><span data-ttu-id="87f4d-103">Список Девицеманажементинтежерсеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="87f4d-103">List deviceManagementIntegerSettingInstances</span></span>

> <span data-ttu-id="87f4d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87f4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87f4d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87f4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87f4d-106">Список свойств и связей объектов [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="87f4d-106">List properties and relationships of the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87f4d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="87f4d-107">Prerequisites</span></span>
<span data-ttu-id="87f4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87f4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87f4d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87f4d-110">Permission type</span></span>|<span data-ttu-id="87f4d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87f4d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87f4d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87f4d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87f4d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87f4d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87f4d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87f4d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87f4d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87f4d-115">Not supported.</span></span>|
|<span data-ttu-id="87f4d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87f4d-116">Application</span></span>|<span data-ttu-id="87f4d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87f4d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87f4d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87f4d-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="87f4d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="87f4d-119">Request headers</span></span>
|<span data-ttu-id="87f4d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87f4d-120">Header</span></span>|<span data-ttu-id="87f4d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="87f4d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87f4d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87f4d-122">Authorization</span></span>|<span data-ttu-id="87f4d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87f4d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87f4d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="87f4d-124">Accept</span></span>|<span data-ttu-id="87f4d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="87f4d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87f4d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87f4d-126">Request body</span></span>
<span data-ttu-id="87f4d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87f4d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87f4d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="87f4d-128">Response</span></span>
<span data-ttu-id="87f4d-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="87f4d-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87f4d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="87f4d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="87f4d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="87f4d-131">Request</span></span>
<span data-ttu-id="87f4d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87f4d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="87f4d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="87f4d-133">Response</span></span>
<span data-ttu-id="87f4d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87f4d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





