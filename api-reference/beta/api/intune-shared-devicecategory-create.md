---
title: Создание объекта deviceCategory
description: Создание объекта deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd1738f6e9f697890e799fe0749d83522a690537
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979822"
---
# <a name="create-devicecategory"></a><span data-ttu-id="dbd46-103">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="dbd46-103">Create deviceCategory</span></span>

> <span data-ttu-id="dbd46-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dbd46-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dbd46-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbd46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbd46-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dbd46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbd46-107">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="dbd46-107">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbd46-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dbd46-108">Prerequisites</span></span>

<span data-ttu-id="dbd46-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbd46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbd46-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbd46-111">Permission type</span></span>|<span data-ttu-id="dbd46-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbd46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbd46-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbd46-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="dbd46-114">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="dbd46-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="dbd46-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbd46-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dbd46-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbd46-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbd46-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbd46-117">Not supported.</span></span>|
|<span data-ttu-id="dbd46-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbd46-118">Application</span></span>|<span data-ttu-id="dbd46-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbd46-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbd46-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbd46-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="dbd46-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbd46-121">Request headers</span></span>

|<span data-ttu-id="dbd46-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dbd46-122">Header</span></span>|<span data-ttu-id="dbd46-123">Значение</span><span class="sxs-lookup"><span data-stu-id="dbd46-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbd46-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dbd46-124">Authorization</span></span>|<span data-ttu-id="dbd46-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbd46-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbd46-126">Accept</span><span class="sxs-lookup"><span data-stu-id="dbd46-126">Accept</span></span>|<span data-ttu-id="dbd46-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dbd46-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbd46-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dbd46-128">Request body</span></span>

<span data-ttu-id="dbd46-129">В теле запроса добавьте представление объекта deviceCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dbd46-129">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="dbd46-130">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="dbd46-130">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="dbd46-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbd46-131">Property</span></span>|<span data-ttu-id="dbd46-132">Тип</span><span class="sxs-lookup"><span data-stu-id="dbd46-132">Type</span></span>|<span data-ttu-id="dbd46-133">Описание</span><span class="sxs-lookup"><span data-stu-id="dbd46-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbd46-134">id</span><span class="sxs-lookup"><span data-stu-id="dbd46-134">id</span></span>|<span data-ttu-id="dbd46-135">String</span><span class="sxs-lookup"><span data-stu-id="dbd46-135">String</span></span>|<span data-ttu-id="dbd46-136">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="dbd46-136">Unique identifier for the device category.</span></span> <span data-ttu-id="dbd46-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dbd46-137">Read-only.</span></span>|
|<span data-ttu-id="dbd46-138">**Оббоардинг**</span><span class="sxs-lookup"><span data-stu-id="dbd46-138">**Obboarding**</span></span>|
|<span data-ttu-id="dbd46-139">description</span><span class="sxs-lookup"><span data-stu-id="dbd46-139">description</span></span>|<span data-ttu-id="dbd46-140">String</span><span class="sxs-lookup"><span data-stu-id="dbd46-140">String</span></span>|<span data-ttu-id="dbd46-141">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="dbd46-141">Optional description for the device category.</span></span>|
|<span data-ttu-id="dbd46-142">displayName</span><span class="sxs-lookup"><span data-stu-id="dbd46-142">displayName</span></span>|<span data-ttu-id="dbd46-143">Строка</span><span class="sxs-lookup"><span data-stu-id="dbd46-143">String</span></span>|<span data-ttu-id="dbd46-144">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="dbd46-144">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="dbd46-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbd46-145">Response</span></span>

<span data-ttu-id="dbd46-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dbd46-146">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbd46-147">Пример</span><span class="sxs-lookup"><span data-stu-id="dbd46-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbd46-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbd46-148">Request</span></span>

<span data-ttu-id="dbd46-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbd46-149">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="dbd46-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbd46-150">Response</span></span>

<span data-ttu-id="dbd46-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dbd46-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



