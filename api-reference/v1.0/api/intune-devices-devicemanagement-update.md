---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c13988e02ed5edcefb9bc830304359dce469d8c3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754351"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="cda85-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cda85-103">Update deviceManagement</span></span>

<span data-ttu-id="cda85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cda85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cda85-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cda85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cda85-106">Обновление свойств объекта [deviceManagement](../resources/intune-devices-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="cda85-106">Update the properties of a [deviceManagement](../resources/intune-devices-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cda85-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cda85-107">Prerequisites</span></span>
<span data-ttu-id="cda85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cda85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cda85-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cda85-110">Permission type</span></span>|<span data-ttu-id="cda85-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cda85-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cda85-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cda85-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cda85-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cda85-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cda85-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cda85-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cda85-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cda85-115">Not supported.</span></span>|
|<span data-ttu-id="cda85-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cda85-116">Application</span></span>|<span data-ttu-id="cda85-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cda85-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cda85-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cda85-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="cda85-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cda85-119">Request headers</span></span>
|<span data-ttu-id="cda85-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cda85-120">Header</span></span>|<span data-ttu-id="cda85-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cda85-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cda85-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cda85-122">Authorization</span></span>|<span data-ttu-id="cda85-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cda85-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cda85-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cda85-124">Accept</span></span>|<span data-ttu-id="cda85-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cda85-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cda85-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cda85-126">Request body</span></span>
<span data-ttu-id="cda85-127">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-devices-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cda85-127">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-devices-devicemanagement.md) object.</span></span>

<span data-ttu-id="cda85-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-devices-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="cda85-128">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-devices-devicemanagement.md).</span></span>

|<span data-ttu-id="cda85-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cda85-129">Property</span></span>|<span data-ttu-id="cda85-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cda85-130">Type</span></span>|<span data-ttu-id="cda85-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cda85-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cda85-132">id</span><span class="sxs-lookup"><span data-stu-id="cda85-132">id</span></span>|<span data-ttu-id="cda85-133">String</span><span class="sxs-lookup"><span data-stu-id="cda85-133">String</span></span>|<span data-ttu-id="cda85-134">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="cda85-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="cda85-135">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="cda85-135">subscriptionState</span></span>|[<span data-ttu-id="cda85-136">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="cda85-136">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="cda85-137">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="cda85-137">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="cda85-138">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="cda85-138">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="cda85-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="cda85-139">Response</span></span>
<span data-ttu-id="cda85-140">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-devices-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cda85-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-devices-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cda85-141">Пример</span><span class="sxs-lookup"><span data-stu-id="cda85-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="cda85-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="cda85-142">Request</span></span>
<span data-ttu-id="cda85-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cda85-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "subscriptionState": "active"
}
```

### <a name="response"></a><span data-ttu-id="cda85-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="cda85-144">Response</span></span>
<span data-ttu-id="cda85-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cda85-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 141

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active"
}
```




