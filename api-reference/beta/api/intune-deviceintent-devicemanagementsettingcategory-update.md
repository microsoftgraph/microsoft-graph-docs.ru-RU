---
title: Обновление Девицеманажементсеттингкатегори
description: Обновление свойств объекта Девицеманажементсеттингкатегори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f561d6a34f3ba793b2f313684669b6ac860f31f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986660"
---
# <a name="update-devicemanagementsettingcategory"></a><span data-ttu-id="98edc-103">Обновление Девицеманажементсеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="98edc-103">Update deviceManagementSettingCategory</span></span>

<span data-ttu-id="98edc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98edc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98edc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98edc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98edc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98edc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98edc-107">Обновление свойств объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="98edc-107">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98edc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="98edc-108">Prerequisites</span></span>
<span data-ttu-id="98edc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98edc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98edc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98edc-111">Permission type</span></span>|<span data-ttu-id="98edc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98edc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98edc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98edc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98edc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98edc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98edc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98edc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98edc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98edc-116">Not supported.</span></span>|
|<span data-ttu-id="98edc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98edc-117">Application</span></span>|<span data-ttu-id="98edc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98edc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98edc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98edc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="98edc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="98edc-120">Request headers</span></span>
|<span data-ttu-id="98edc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98edc-121">Header</span></span>|<span data-ttu-id="98edc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="98edc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98edc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98edc-123">Authorization</span></span>|<span data-ttu-id="98edc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98edc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98edc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98edc-125">Accept</span></span>|<span data-ttu-id="98edc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98edc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98edc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98edc-127">Request body</span></span>
<span data-ttu-id="98edc-128">В тексте запроса добавьте представление объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98edc-128">In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

<span data-ttu-id="98edc-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="98edc-129">The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>

|<span data-ttu-id="98edc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="98edc-130">Property</span></span>|<span data-ttu-id="98edc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="98edc-131">Type</span></span>|<span data-ttu-id="98edc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="98edc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98edc-133">id</span><span class="sxs-lookup"><span data-stu-id="98edc-133">id</span></span>|<span data-ttu-id="98edc-134">String</span><span class="sxs-lookup"><span data-stu-id="98edc-134">String</span></span>|<span data-ttu-id="98edc-135">Идентификатор категории</span><span class="sxs-lookup"><span data-stu-id="98edc-135">The category ID</span></span>|
|<span data-ttu-id="98edc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="98edc-136">displayName</span></span>|<span data-ttu-id="98edc-137">String</span><span class="sxs-lookup"><span data-stu-id="98edc-137">String</span></span>|<span data-ttu-id="98edc-138">Имя категории</span><span class="sxs-lookup"><span data-stu-id="98edc-138">The category name</span></span>|
|<span data-ttu-id="98edc-139">хасрекуиредсеттинг</span><span class="sxs-lookup"><span data-stu-id="98edc-139">hasRequiredSetting</span></span>|<span data-ttu-id="98edc-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="98edc-140">Boolean</span></span>|<span data-ttu-id="98edc-141">Категория содержит параметры, необходимые для верхнего уровня</span><span class="sxs-lookup"><span data-stu-id="98edc-141">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="98edc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="98edc-142">Response</span></span>
<span data-ttu-id="98edc-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98edc-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98edc-144">Пример</span><span class="sxs-lookup"><span data-stu-id="98edc-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="98edc-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="98edc-145">Request</span></span>
<span data-ttu-id="98edc-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98edc-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/categories/{deviceManagementSettingCategoryId}
Content-type: application/json
Content-length: 144

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="98edc-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="98edc-147">Response</span></span>
<span data-ttu-id="98edc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98edc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 193

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```






