---
title: Создание объекта deviceCategory
description: Создание объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 233046ca0eb9a03c6b43cc58b4c4bf83a90878d8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019189"
---
# <a name="create-devicecategory"></a><span data-ttu-id="71518-103">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="71518-103">Create deviceCategory</span></span>

<span data-ttu-id="71518-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71518-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71518-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71518-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71518-106">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="71518-106">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71518-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="71518-107">Prerequisites</span></span>
<span data-ttu-id="71518-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71518-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71518-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71518-110">Permission type</span></span>|<span data-ttu-id="71518-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71518-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71518-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71518-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="71518-113">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="71518-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="71518-114">Девицеманажементманажед Devices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="71518-114">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="71518-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71518-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71518-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71518-116">Not supported.</span></span>|
|<span data-ttu-id="71518-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71518-117">Application</span></span>|<span data-ttu-id="71518-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71518-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71518-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71518-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="71518-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="71518-120">Request headers</span></span>
|<span data-ttu-id="71518-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71518-121">Header</span></span>|<span data-ttu-id="71518-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71518-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71518-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71518-123">Authorization</span></span>|<span data-ttu-id="71518-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71518-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71518-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71518-125">Accept</span></span>|<span data-ttu-id="71518-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71518-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71518-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="71518-127">Request body</span></span>
<span data-ttu-id="71518-128">В теле запроса добавьте представление объекта deviceCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71518-128">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="71518-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="71518-129">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="71518-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="71518-130">Property</span></span>|<span data-ttu-id="71518-131">Тип</span><span class="sxs-lookup"><span data-stu-id="71518-131">Type</span></span>|<span data-ttu-id="71518-132">Описание</span><span class="sxs-lookup"><span data-stu-id="71518-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71518-133">id</span><span class="sxs-lookup"><span data-stu-id="71518-133">id</span></span>|<span data-ttu-id="71518-134">String</span><span class="sxs-lookup"><span data-stu-id="71518-134">String</span></span>|<span data-ttu-id="71518-135">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="71518-135">Unique identifier for the device category.</span></span> <span data-ttu-id="71518-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="71518-136">Read-only.</span></span>|
|<span data-ttu-id="71518-137">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="71518-137">**Onboarding**</span></span>|
|<span data-ttu-id="71518-138">displayName</span><span class="sxs-lookup"><span data-stu-id="71518-138">displayName</span></span>|<span data-ttu-id="71518-139">String</span><span class="sxs-lookup"><span data-stu-id="71518-139">String</span></span>|<span data-ttu-id="71518-140">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="71518-140">Display name for the device category.</span></span>|
|<span data-ttu-id="71518-141">description</span><span class="sxs-lookup"><span data-stu-id="71518-141">description</span></span>|<span data-ttu-id="71518-142">String</span><span class="sxs-lookup"><span data-stu-id="71518-142">String</span></span>|<span data-ttu-id="71518-143">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="71518-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="71518-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="71518-144">Response</span></span>
<span data-ttu-id="71518-145">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="71518-145">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71518-146">Пример</span><span class="sxs-lookup"><span data-stu-id="71518-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="71518-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="71518-147">Request</span></span>
<span data-ttu-id="71518-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71518-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="71518-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="71518-149">Response</span></span>
<span data-ttu-id="71518-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71518-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```









