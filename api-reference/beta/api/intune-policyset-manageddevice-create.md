---
title: Create managedDevice
description: Создание объекта managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5eeea35062111e7b790d767f206cfa83bab640b2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51124690"
---
# <a name="create-manageddevice"></a><span data-ttu-id="0b0c5-103">Create managedDevice</span><span class="sxs-lookup"><span data-stu-id="0b0c5-103">Create managedDevice</span></span>

<span data-ttu-id="0b0c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b0c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b0c5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b0c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b0c5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b0c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b0c5-107">Создание объекта [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="0b0c5-107">Create a new [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b0c5-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0b0c5-108">Prerequisites</span></span>
<span data-ttu-id="0b0c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b0c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b0c5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b0c5-111">Permission type</span></span>|<span data-ttu-id="0b0c5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b0c5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b0c5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b0c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b0c5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b0c5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b0c5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b0c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b0c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b0c5-116">Not supported.</span></span>|
|<span data-ttu-id="0b0c5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0b0c5-117">Application</span></span>|<span data-ttu-id="0b0c5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b0c5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b0c5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b0c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="0b0c5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0b0c5-120">Request headers</span></span>
|<span data-ttu-id="0b0c5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b0c5-121">Header</span></span>|<span data-ttu-id="0b0c5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0b0c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b0c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b0c5-123">Authorization</span></span>|<span data-ttu-id="0b0c5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b0c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b0c5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b0c5-125">Accept</span></span>|<span data-ttu-id="0b0c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b0c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b0c5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b0c5-127">Request body</span></span>
<span data-ttu-id="0b0c5-128">В тексте запроса добавьте представление объекта managedDevice в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b0c5-128">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="0b0c5-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedDevice.</span><span class="sxs-lookup"><span data-stu-id="0b0c5-129">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="0b0c5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b0c5-130">Property</span></span>|<span data-ttu-id="0b0c5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0b0c5-131">Type</span></span>|<span data-ttu-id="0b0c5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0b0c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b0c5-133">id</span><span class="sxs-lookup"><span data-stu-id="0b0c5-133">id</span></span>|<span data-ttu-id="0b0c5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0b0c5-134">String</span></span>|<span data-ttu-id="0b0c5-135">Ключ сущности управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="0b0c5-135">Key of Managed device entity.</span></span>|



## <a name="response"></a><span data-ttu-id="0b0c5-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b0c5-136">Response</span></span>
<span data-ttu-id="0b0c5-137">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedDevice](../resources/intune-shared-manageddevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0b0c5-137">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune-shared-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b0c5-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0b0c5-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b0c5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b0c5-139">Request</span></span>
<span data-ttu-id="0b0c5-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b0c5-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 55

{
  "@odata.type": "#microsoft.graph.managedDevice"
}
```

### <a name="response"></a><span data-ttu-id="0b0c5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b0c5-141">Response</span></span>
<span data-ttu-id="0b0c5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b0c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 104

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70"
}
```




