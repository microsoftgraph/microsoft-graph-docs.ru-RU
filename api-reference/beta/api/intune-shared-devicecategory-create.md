---
title: Создание объекта deviceCategory
description: Создание объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9f40ec6beb11ed6a299c23b6da905466a47fc5e9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153713"
---
# <a name="create-devicecategory"></a><span data-ttu-id="04cc2-103">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="04cc2-103">Create deviceCategory</span></span>

> <span data-ttu-id="04cc2-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="04cc2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04cc2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04cc2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04cc2-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04cc2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04cc2-107">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="04cc2-107">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04cc2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="04cc2-108">Prerequisites</span></span>

<span data-ttu-id="04cc2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04cc2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="04cc2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04cc2-111">Permission type</span></span>|<span data-ttu-id="04cc2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04cc2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04cc2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04cc2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="04cc2-114">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="04cc2-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="04cc2-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04cc2-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="04cc2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04cc2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04cc2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04cc2-117">Not supported.</span></span>|
|<span data-ttu-id="04cc2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04cc2-118">Application</span></span>|<span data-ttu-id="04cc2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04cc2-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04cc2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04cc2-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="04cc2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04cc2-121">Request headers</span></span>

|<span data-ttu-id="04cc2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04cc2-122">Header</span></span>|<span data-ttu-id="04cc2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="04cc2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04cc2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04cc2-124">Authorization</span></span>|<span data-ttu-id="04cc2-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="04cc2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04cc2-126">Accept</span><span class="sxs-lookup"><span data-stu-id="04cc2-126">Accept</span></span>|<span data-ttu-id="04cc2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="04cc2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04cc2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04cc2-128">Request body</span></span>

<span data-ttu-id="04cc2-129">В теле запроса добавьте представление объекта deviceCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04cc2-129">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="04cc2-130">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="04cc2-130">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="04cc2-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="04cc2-131">Property</span></span>|<span data-ttu-id="04cc2-132">Тип</span><span class="sxs-lookup"><span data-stu-id="04cc2-132">Type</span></span>|<span data-ttu-id="04cc2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="04cc2-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04cc2-134">id</span><span class="sxs-lookup"><span data-stu-id="04cc2-134">id</span></span>|<span data-ttu-id="04cc2-135">String</span><span class="sxs-lookup"><span data-stu-id="04cc2-135">String</span></span>|<span data-ttu-id="04cc2-136">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="04cc2-136">Unique identifier for the device category.</span></span> <span data-ttu-id="04cc2-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04cc2-137">Read-only.</span></span>|
|<span data-ttu-id="04cc2-138">**Оббоардинг**</span><span class="sxs-lookup"><span data-stu-id="04cc2-138">**Obboarding**</span></span>|
|<span data-ttu-id="04cc2-139">description</span><span class="sxs-lookup"><span data-stu-id="04cc2-139">description</span></span>|<span data-ttu-id="04cc2-140">String</span><span class="sxs-lookup"><span data-stu-id="04cc2-140">String</span></span>|<span data-ttu-id="04cc2-141">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="04cc2-141">Optional description for the device category.</span></span>|
|<span data-ttu-id="04cc2-142">displayName</span><span class="sxs-lookup"><span data-stu-id="04cc2-142">displayName</span></span>|<span data-ttu-id="04cc2-143">String</span><span class="sxs-lookup"><span data-stu-id="04cc2-143">String</span></span>|<span data-ttu-id="04cc2-144">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="04cc2-144">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="04cc2-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="04cc2-145">Response</span></span>

<span data-ttu-id="04cc2-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="04cc2-146">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04cc2-147">Пример</span><span class="sxs-lookup"><span data-stu-id="04cc2-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="04cc2-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="04cc2-148">Request</span></span>

<span data-ttu-id="04cc2-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04cc2-149">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="04cc2-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="04cc2-150">Response</span></span>

<span data-ttu-id="04cc2-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04cc2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



