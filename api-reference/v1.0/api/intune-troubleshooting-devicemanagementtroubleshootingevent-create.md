---
title: Создание объекта deviceManagementTroubleshootingEvent
description: Создание объекта deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd63c88c26f27c30072cb40b61ed54ec96f583bb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025710"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="a1de1-103">Создание объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a1de1-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="a1de1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1de1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1de1-105">Создание объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a1de1-105">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1de1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a1de1-106">Prerequisites</span></span>
<span data-ttu-id="a1de1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1de1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1de1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1de1-109">Permission type</span></span>|<span data-ttu-id="a1de1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1de1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1de1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1de1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a1de1-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1de1-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a1de1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1de1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1de1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1de1-114">Not supported.</span></span>|
|<span data-ttu-id="a1de1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1de1-115">Application</span></span>|<span data-ttu-id="a1de1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1de1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1de1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1de1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="a1de1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1de1-118">Request headers</span></span>
|<span data-ttu-id="a1de1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1de1-119">Header</span></span>|<span data-ttu-id="a1de1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a1de1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1de1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1de1-121">Authorization</span></span>|<span data-ttu-id="a1de1-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1de1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1de1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a1de1-123">Accept</span></span>|<span data-ttu-id="a1de1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a1de1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1de1-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1de1-125">Request body</span></span>
<span data-ttu-id="a1de1-126">В теле запроса добавьте представление объекта deviceManagementTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1de1-126">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="a1de1-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="a1de1-127">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="a1de1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1de1-128">Property</span></span>|<span data-ttu-id="a1de1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a1de1-129">Type</span></span>|<span data-ttu-id="a1de1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a1de1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1de1-131">id</span><span class="sxs-lookup"><span data-stu-id="a1de1-131">id</span></span>|<span data-ttu-id="a1de1-132">Строка</span><span class="sxs-lookup"><span data-stu-id="a1de1-132">String</span></span>|<span data-ttu-id="a1de1-133">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="a1de1-133">UUID for the object</span></span>|
|<span data-ttu-id="a1de1-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="a1de1-134">eventDateTime</span></span>|<span data-ttu-id="a1de1-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1de1-135">DateTimeOffset</span></span>|<span data-ttu-id="a1de1-136">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="a1de1-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="a1de1-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="a1de1-137">correlationId</span></span>|<span data-ttu-id="a1de1-138">String</span><span class="sxs-lookup"><span data-stu-id="a1de1-138">String</span></span>|<span data-ttu-id="a1de1-139">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="a1de1-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="a1de1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1de1-140">Response</span></span>
<span data-ttu-id="a1de1-141">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a1de1-141">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1de1-142">Пример</span><span class="sxs-lookup"><span data-stu-id="a1de1-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1de1-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1de1-143">Request</span></span>
<span data-ttu-id="a1de1-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1de1-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="a1de1-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1de1-145">Response</span></span>
<span data-ttu-id="a1de1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1de1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```



