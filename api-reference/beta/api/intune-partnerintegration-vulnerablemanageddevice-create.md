---
title: Создание vulnerableManagedDevice
description: Создайте новый объект vulnerableManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02ada5a0926a3b96e448b8027b3b68ed4be8fe26
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134748"
---
# <a name="create-vulnerablemanageddevice"></a><span data-ttu-id="9304a-103">Создание vulnerableManagedDevice</span><span class="sxs-lookup"><span data-stu-id="9304a-103">Create vulnerableManagedDevice</span></span>

<span data-ttu-id="9304a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9304a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9304a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9304a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9304a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9304a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9304a-107">Создайте новый [объект vulnerableManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9304a-107">Create a new [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9304a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9304a-108">Prerequisites</span></span>
<span data-ttu-id="9304a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9304a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9304a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9304a-111">Permission type</span></span>|<span data-ttu-id="9304a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9304a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9304a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9304a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9304a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9304a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9304a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9304a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9304a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9304a-116">Not supported.</span></span>|
|<span data-ttu-id="9304a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9304a-117">Application</span></span>|<span data-ttu-id="9304a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9304a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9304a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9304a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a><span data-ttu-id="9304a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9304a-120">Request headers</span></span>
|<span data-ttu-id="9304a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9304a-121">Header</span></span>|<span data-ttu-id="9304a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9304a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9304a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9304a-123">Authorization</span></span>|<span data-ttu-id="9304a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9304a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9304a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9304a-125">Accept</span></span>|<span data-ttu-id="9304a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9304a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9304a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9304a-127">Request body</span></span>
<span data-ttu-id="9304a-128">В теле запроса поставляем представление JSON для уязвимого объектаManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="9304a-128">In the request body, supply a JSON representation for the vulnerableManagedDevice object.</span></span>

<span data-ttu-id="9304a-129">В следующей таблице показаны свойства, необходимые при создании vulnerableManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="9304a-129">The following table shows the properties that are required when you create the vulnerableManagedDevice.</span></span>

|<span data-ttu-id="9304a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9304a-130">Property</span></span>|<span data-ttu-id="9304a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9304a-131">Type</span></span>|<span data-ttu-id="9304a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9304a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9304a-133">id</span><span class="sxs-lookup"><span data-stu-id="9304a-133">id</span></span>|<span data-ttu-id="9304a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9304a-134">String</span></span>|<span data-ttu-id="9304a-135">Ключ сущности и ID устройства AAD.</span><span class="sxs-lookup"><span data-stu-id="9304a-135">The entity key, and AAD device ID.</span></span>|
|<span data-ttu-id="9304a-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="9304a-136">managedDeviceId</span></span>|<span data-ttu-id="9304a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9304a-137">String</span></span>|<span data-ttu-id="9304a-138">ID управляемого устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="9304a-138">The Intune managed device ID.</span></span>|
|<span data-ttu-id="9304a-139">displayName</span><span class="sxs-lookup"><span data-stu-id="9304a-139">displayName</span></span>|<span data-ttu-id="9304a-140">Строка</span><span class="sxs-lookup"><span data-stu-id="9304a-140">String</span></span>|<span data-ttu-id="9304a-141">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="9304a-141">The device name.</span></span>|
|<span data-ttu-id="9304a-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9304a-142">lastSyncDateTime</span></span>|<span data-ttu-id="9304a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9304a-143">DateTimeOffset</span></span>|<span data-ttu-id="9304a-144">Последняя дата синхронизации.</span><span class="sxs-lookup"><span data-stu-id="9304a-144">The last sync date.</span></span>|



## <a name="response"></a><span data-ttu-id="9304a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9304a-145">Response</span></span>
<span data-ttu-id="9304a-146">В случае успешной работы этот метод возвращает код ответа и уязвимый `201 Created` [объектManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9304a-146">If successful, this method returns a `201 Created` response code and a [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9304a-147">Пример</span><span class="sxs-lookup"><span data-stu-id="9304a-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="9304a-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="9304a-148">Request</span></span>
<span data-ttu-id="9304a-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9304a-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
Content-type: application/json
Content-length: 214

{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a><span data-ttu-id="9304a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="9304a-150">Response</span></span>
<span data-ttu-id="9304a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9304a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 263

{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "id": "e59891d4-91d4-e598-d491-98e5d49198e5",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```




