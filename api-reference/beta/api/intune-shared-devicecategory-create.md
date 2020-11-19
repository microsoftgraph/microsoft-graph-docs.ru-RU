---
title: Создание объекта deviceCategory
description: Создание объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c846a2dda0d39b0086398af51afe8ebd6a08bff
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49232734"
---
# <a name="create-devicecategory"></a><span data-ttu-id="39d19-103">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="39d19-103">Create deviceCategory</span></span>

<span data-ttu-id="39d19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39d19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39d19-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="39d19-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="39d19-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39d19-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39d19-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39d19-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39d19-108">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="39d19-108">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39d19-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="39d19-109">Prerequisites</span></span>

<span data-ttu-id="39d19-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39d19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39d19-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39d19-112">Permission type</span></span>|<span data-ttu-id="39d19-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39d19-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39d19-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39d19-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="39d19-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="39d19-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="39d19-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39d19-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="39d19-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39d19-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39d19-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39d19-118">Not supported.</span></span>|
|<span data-ttu-id="39d19-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="39d19-119">Application</span></span>||
| <span data-ttu-id="39d19-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="39d19-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="39d19-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39d19-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="39d19-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39d19-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="39d19-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="39d19-123">Request headers</span></span>

|<span data-ttu-id="39d19-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39d19-124">Header</span></span>|<span data-ttu-id="39d19-125">Значение</span><span class="sxs-lookup"><span data-stu-id="39d19-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39d19-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39d19-126">Authorization</span></span>|<span data-ttu-id="39d19-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39d19-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39d19-128">Accept</span><span class="sxs-lookup"><span data-stu-id="39d19-128">Accept</span></span>|<span data-ttu-id="39d19-129">application/json</span><span class="sxs-lookup"><span data-stu-id="39d19-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39d19-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39d19-130">Request body</span></span>

<span data-ttu-id="39d19-131">В теле запроса добавьте представление объекта deviceCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39d19-131">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="39d19-132">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="39d19-132">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="39d19-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="39d19-133">Property</span></span>|<span data-ttu-id="39d19-134">Тип</span><span class="sxs-lookup"><span data-stu-id="39d19-134">Type</span></span>|<span data-ttu-id="39d19-135">Описание</span><span class="sxs-lookup"><span data-stu-id="39d19-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39d19-136">id</span><span class="sxs-lookup"><span data-stu-id="39d19-136">id</span></span>|<span data-ttu-id="39d19-137">String</span><span class="sxs-lookup"><span data-stu-id="39d19-137">String</span></span>|<span data-ttu-id="39d19-138">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="39d19-138">Unique identifier for the device category.</span></span> <span data-ttu-id="39d19-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39d19-139">Read-only.</span></span>|
|<span data-ttu-id="39d19-140">**оббоардинг**</span><span class="sxs-lookup"><span data-stu-id="39d19-140">**Obboarding**</span></span>|
|<span data-ttu-id="39d19-141">description</span><span class="sxs-lookup"><span data-stu-id="39d19-141">description</span></span>|<span data-ttu-id="39d19-142">String</span><span class="sxs-lookup"><span data-stu-id="39d19-142">String</span></span>|<span data-ttu-id="39d19-143">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="39d19-143">Optional description for the device category.</span></span>|
|<span data-ttu-id="39d19-144">displayName</span><span class="sxs-lookup"><span data-stu-id="39d19-144">displayName</span></span>|<span data-ttu-id="39d19-145">String</span><span class="sxs-lookup"><span data-stu-id="39d19-145">String</span></span>|<span data-ttu-id="39d19-146">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="39d19-146">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="39d19-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="39d19-147">Response</span></span>

<span data-ttu-id="39d19-148">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="39d19-148">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39d19-149">Пример</span><span class="sxs-lookup"><span data-stu-id="39d19-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="39d19-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="39d19-150">Request</span></span>

<span data-ttu-id="39d19-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39d19-151">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="39d19-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="39d19-152">Response</span></span>

<span data-ttu-id="39d19-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39d19-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










