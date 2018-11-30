---
title: Создание объекта deviceCategory
description: Создание объекта deviceCategory.
ms.openlocfilehash: 43a731716150a7cc9515a6497840cc47271e88c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026889"
---
# <a name="create-devicecategory"></a><span data-ttu-id="59c55-103">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="59c55-103">Create deviceCategory</span></span>

> <span data-ttu-id="59c55-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="59c55-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59c55-105">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="59c55-105">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59c55-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="59c55-106">Prerequisites</span></span>
<span data-ttu-id="59c55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59c55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59c55-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59c55-109">Permission type</span></span>|<span data-ttu-id="59c55-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="59c55-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59c55-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59c55-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="59c55-112">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="59c55-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="59c55-113">DeviceManagementManaged Devices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59c55-113">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="59c55-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59c55-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59c55-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59c55-115">Not supported.</span></span>|
|<span data-ttu-id="59c55-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59c55-116">Application</span></span>|<span data-ttu-id="59c55-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59c55-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59c55-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59c55-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="59c55-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59c55-119">Request headers</span></span>
|<span data-ttu-id="59c55-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59c55-120">Header</span></span>|<span data-ttu-id="59c55-121">Значение</span><span class="sxs-lookup"><span data-stu-id="59c55-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59c55-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="59c55-122">Authorization</span></span>|<span data-ttu-id="59c55-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="59c55-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59c55-124">Accept</span><span class="sxs-lookup"><span data-stu-id="59c55-124">Accept</span></span>|<span data-ttu-id="59c55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59c55-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59c55-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="59c55-126">Request body</span></span>
<span data-ttu-id="59c55-127">В теле запроса добавьте представление объекта deviceCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59c55-127">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="59c55-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="59c55-128">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="59c55-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="59c55-129">Property</span></span>|<span data-ttu-id="59c55-130">Тип</span><span class="sxs-lookup"><span data-stu-id="59c55-130">Type</span></span>|<span data-ttu-id="59c55-131">Описание</span><span class="sxs-lookup"><span data-stu-id="59c55-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59c55-132">id</span><span class="sxs-lookup"><span data-stu-id="59c55-132">id</span></span>|<span data-ttu-id="59c55-133">String</span><span class="sxs-lookup"><span data-stu-id="59c55-133">String</span></span>|<span data-ttu-id="59c55-134">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="59c55-134">Unique identifier for the device category.</span></span> <span data-ttu-id="59c55-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59c55-135">Read-only.</span></span>|
|<span data-ttu-id="59c55-136">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="59c55-136">**Onboarding**</span></span>|
|<span data-ttu-id="59c55-137">displayName</span><span class="sxs-lookup"><span data-stu-id="59c55-137">displayName</span></span>|<span data-ttu-id="59c55-138">String</span><span class="sxs-lookup"><span data-stu-id="59c55-138">String</span></span>|<span data-ttu-id="59c55-139">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="59c55-139">Display name for the device category.</span></span>|
|<span data-ttu-id="59c55-140">описание</span><span class="sxs-lookup"><span data-stu-id="59c55-140">description</span></span>|<span data-ttu-id="59c55-141">String</span><span class="sxs-lookup"><span data-stu-id="59c55-141">String</span></span>|<span data-ttu-id="59c55-142">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="59c55-142">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="59c55-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="59c55-143">Response</span></span>
<span data-ttu-id="59c55-144">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="59c55-144">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59c55-145">Пример</span><span class="sxs-lookup"><span data-stu-id="59c55-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="59c55-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="59c55-146">Request</span></span>
<span data-ttu-id="59c55-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59c55-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="59c55-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="59c55-148">Response</span></span>
<span data-ttu-id="59c55-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="59c55-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



