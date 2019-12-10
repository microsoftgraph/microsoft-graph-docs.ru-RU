---
title: Создание объекта deviceCategory
description: Создание объекта deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d4ca7f17ba5dd98605f4e1ea1f5db1b54c96d69
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940168"
---
# <a name="create-devicecategory"></a><span data-ttu-id="f0db9-103">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="f0db9-103">Create deviceCategory</span></span>

> <span data-ttu-id="f0db9-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f0db9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f0db9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0db9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0db9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0db9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0db9-107">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="f0db9-107">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0db9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0db9-108">Prerequisites</span></span>

<span data-ttu-id="f0db9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0db9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0db9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0db9-111">Permission type</span></span>|<span data-ttu-id="f0db9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0db9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0db9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0db9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f0db9-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="f0db9-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f0db9-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0db9-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f0db9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0db9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0db9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0db9-117">Not supported.</span></span>|
|<span data-ttu-id="f0db9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0db9-118">Application</span></span>||
| <span data-ttu-id="f0db9-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="f0db9-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f0db9-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0db9-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0db9-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0db9-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="f0db9-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f0db9-122">Request headers</span></span>

|<span data-ttu-id="f0db9-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0db9-123">Header</span></span>|<span data-ttu-id="f0db9-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f0db9-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0db9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0db9-125">Authorization</span></span>|<span data-ttu-id="f0db9-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0db9-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0db9-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f0db9-127">Accept</span></span>|<span data-ttu-id="f0db9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f0db9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0db9-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f0db9-129">Request body</span></span>

<span data-ttu-id="f0db9-130">В теле запроса добавьте представление объекта deviceCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0db9-130">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="f0db9-131">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="f0db9-131">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="f0db9-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0db9-132">Property</span></span>|<span data-ttu-id="f0db9-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f0db9-133">Type</span></span>|<span data-ttu-id="f0db9-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f0db9-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0db9-135">id</span><span class="sxs-lookup"><span data-stu-id="f0db9-135">id</span></span>|<span data-ttu-id="f0db9-136">String</span><span class="sxs-lookup"><span data-stu-id="f0db9-136">String</span></span>|<span data-ttu-id="f0db9-137">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="f0db9-137">Unique identifier for the device category.</span></span> <span data-ttu-id="f0db9-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0db9-138">Read-only.</span></span>|
|<span data-ttu-id="f0db9-139">**оббоардинг**</span><span class="sxs-lookup"><span data-stu-id="f0db9-139">**Obboarding**</span></span>|
|<span data-ttu-id="f0db9-140">description</span><span class="sxs-lookup"><span data-stu-id="f0db9-140">description</span></span>|<span data-ttu-id="f0db9-141">String</span><span class="sxs-lookup"><span data-stu-id="f0db9-141">String</span></span>|<span data-ttu-id="f0db9-142">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="f0db9-142">Optional description for the device category.</span></span>|
|<span data-ttu-id="f0db9-143">displayName</span><span class="sxs-lookup"><span data-stu-id="f0db9-143">displayName</span></span>|<span data-ttu-id="f0db9-144">Строка</span><span class="sxs-lookup"><span data-stu-id="f0db9-144">String</span></span>|<span data-ttu-id="f0db9-145">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="f0db9-145">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="f0db9-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0db9-146">Response</span></span>

<span data-ttu-id="f0db9-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f0db9-147">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0db9-148">Пример</span><span class="sxs-lookup"><span data-stu-id="f0db9-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0db9-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0db9-149">Request</span></span>

<span data-ttu-id="f0db9-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0db9-150">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="f0db9-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0db9-151">Response</span></span>

<span data-ttu-id="f0db9-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0db9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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











