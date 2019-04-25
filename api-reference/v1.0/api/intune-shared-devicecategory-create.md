---
title: Создание объекта deviceCategory
description: Создание объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 76c1d0c8b22484b3a35d0db49c5a4e578e656880
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577037"
---
# <a name="create-devicecategory"></a><span data-ttu-id="c9672-103">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="c9672-103">Create deviceCategory</span></span>

> <span data-ttu-id="c9672-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9672-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9672-105">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="c9672-105">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9672-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c9672-106">Prerequisites</span></span>
<span data-ttu-id="c9672-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9672-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9672-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9672-109">Permission type</span></span>|<span data-ttu-id="c9672-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9672-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9672-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9672-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c9672-112">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="c9672-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c9672-113">Девицеманажементманажед Devices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c9672-113">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="c9672-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9672-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9672-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9672-115">Not supported.</span></span>|
|<span data-ttu-id="c9672-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9672-116">Application</span></span>|<span data-ttu-id="c9672-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9672-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9672-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9672-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="c9672-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9672-119">Request headers</span></span>
|<span data-ttu-id="c9672-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9672-120">Header</span></span>|<span data-ttu-id="c9672-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c9672-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9672-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9672-122">Authorization</span></span>|<span data-ttu-id="c9672-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9672-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9672-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c9672-124">Accept</span></span>|<span data-ttu-id="c9672-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9672-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9672-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9672-126">Request body</span></span>
<span data-ttu-id="c9672-127">В теле запроса добавьте представление объекта deviceCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9672-127">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="c9672-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="c9672-128">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="c9672-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9672-129">Property</span></span>|<span data-ttu-id="c9672-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c9672-130">Type</span></span>|<span data-ttu-id="c9672-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c9672-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9672-132">id</span><span class="sxs-lookup"><span data-stu-id="c9672-132">id</span></span>|<span data-ttu-id="c9672-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c9672-133">String</span></span>|<span data-ttu-id="c9672-134">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="c9672-134">Unique identifier for the device category.</span></span> <span data-ttu-id="c9672-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9672-135">Read-only.</span></span>|
|<span data-ttu-id="c9672-136">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="c9672-136">**Onboarding**</span></span>|
|<span data-ttu-id="c9672-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c9672-137">displayName</span></span>|<span data-ttu-id="c9672-138">String</span><span class="sxs-lookup"><span data-stu-id="c9672-138">String</span></span>|<span data-ttu-id="c9672-139">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="c9672-139">Display name for the device category.</span></span>|
|<span data-ttu-id="c9672-140">description</span><span class="sxs-lookup"><span data-stu-id="c9672-140">description</span></span>|<span data-ttu-id="c9672-141">String</span><span class="sxs-lookup"><span data-stu-id="c9672-141">String</span></span>|<span data-ttu-id="c9672-142">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="c9672-142">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="c9672-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9672-143">Response</span></span>
<span data-ttu-id="c9672-144">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c9672-144">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9672-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c9672-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9672-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9672-146">Request</span></span>
<span data-ttu-id="c9672-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9672-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c9672-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9672-148">Response</span></span>
<span data-ttu-id="c9672-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9672-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



