---
title: Обновление managedDevice
description: Обновление свойств объекта managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb84276b6703400606759c48dcb2f6cc7485bdcf
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160580"
---
# <a name="update-manageddevice"></a><span data-ttu-id="eeac9-103">Обновление managedDevice</span><span class="sxs-lookup"><span data-stu-id="eeac9-103">Update managedDevice</span></span>

<span data-ttu-id="eeac9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eeac9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eeac9-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeac9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eeac9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eeac9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eeac9-107">Обновление свойств объекта [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="eeac9-107">Update the properties of a [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eeac9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="eeac9-108">Prerequisites</span></span>
<span data-ttu-id="eeac9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeac9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeac9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eeac9-111">Permission type</span></span>|<span data-ttu-id="eeac9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eeac9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eeac9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eeac9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eeac9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeac9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eeac9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eeac9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eeac9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeac9-116">Not supported.</span></span>|
|<span data-ttu-id="eeac9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eeac9-117">Application</span></span>|<span data-ttu-id="eeac9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeac9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eeac9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eeac9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="eeac9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eeac9-120">Request headers</span></span>
|<span data-ttu-id="eeac9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eeac9-121">Header</span></span>|<span data-ttu-id="eeac9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eeac9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eeac9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eeac9-123">Authorization</span></span>|<span data-ttu-id="eeac9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eeac9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eeac9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eeac9-125">Accept</span></span>|<span data-ttu-id="eeac9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eeac9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eeac9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eeac9-127">Request body</span></span>
<span data-ttu-id="eeac9-128">В теле запроса добавьте представление объекта [managedDevice](../resources/intune-shared-manageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eeac9-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

<span data-ttu-id="eeac9-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="eeac9-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-shared-manageddevice.md).</span></span>

|<span data-ttu-id="eeac9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eeac9-130">Property</span></span>|<span data-ttu-id="eeac9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eeac9-131">Type</span></span>|<span data-ttu-id="eeac9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eeac9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeac9-133">id</span><span class="sxs-lookup"><span data-stu-id="eeac9-133">id</span></span>|<span data-ttu-id="eeac9-134">String</span><span class="sxs-lookup"><span data-stu-id="eeac9-134">String</span></span>|<span data-ttu-id="eeac9-135">Ключ сущности управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="eeac9-135">Key of Managed device entity.</span></span>|



## <a name="response"></a><span data-ttu-id="eeac9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="eeac9-136">Response</span></span>
<span data-ttu-id="eeac9-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDevice](../resources/intune-shared-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eeac9-137">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-shared-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeac9-138">Пример</span><span class="sxs-lookup"><span data-stu-id="eeac9-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="eeac9-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="eeac9-139">Request</span></span>
<span data-ttu-id="eeac9-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eeac9-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 55

{
  "@odata.type": "#microsoft.graph.managedDevice"
}
```

### <a name="response"></a><span data-ttu-id="eeac9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="eeac9-141">Response</span></span>
<span data-ttu-id="eeac9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eeac9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 104

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70"
}
```




