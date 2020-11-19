---
title: Обновление Девицеманажементсеттингкатегори
description: Обновление свойств объекта Девицеманажементсеттингкатегори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b3889af273c6a0c80a7437994c660bcbb9b0ce1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49229627"
---
# <a name="update-devicemanagementsettingcategory"></a><span data-ttu-id="f630b-103">Обновление Девицеманажементсеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="f630b-103">Update deviceManagementSettingCategory</span></span>

<span data-ttu-id="f630b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f630b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f630b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f630b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f630b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f630b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f630b-107">Обновление свойств объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="f630b-107">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f630b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f630b-108">Prerequisites</span></span>
<span data-ttu-id="f630b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f630b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f630b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f630b-111">Permission type</span></span>|<span data-ttu-id="f630b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f630b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f630b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f630b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f630b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f630b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f630b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f630b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f630b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f630b-116">Not supported.</span></span>|
|<span data-ttu-id="f630b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f630b-117">Application</span></span>|<span data-ttu-id="f630b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f630b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f630b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f630b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="f630b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f630b-120">Request headers</span></span>
|<span data-ttu-id="f630b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f630b-121">Header</span></span>|<span data-ttu-id="f630b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f630b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f630b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f630b-123">Authorization</span></span>|<span data-ttu-id="f630b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f630b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f630b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f630b-125">Accept</span></span>|<span data-ttu-id="f630b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f630b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f630b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f630b-127">Request body</span></span>
<span data-ttu-id="f630b-128">В тексте запроса добавьте представление объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f630b-128">In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

<span data-ttu-id="f630b-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="f630b-129">The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>

|<span data-ttu-id="f630b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f630b-130">Property</span></span>|<span data-ttu-id="f630b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f630b-131">Type</span></span>|<span data-ttu-id="f630b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f630b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f630b-133">id</span><span class="sxs-lookup"><span data-stu-id="f630b-133">id</span></span>|<span data-ttu-id="f630b-134">String</span><span class="sxs-lookup"><span data-stu-id="f630b-134">String</span></span>|<span data-ttu-id="f630b-135">Идентификатор категории</span><span class="sxs-lookup"><span data-stu-id="f630b-135">The category ID</span></span>|
|<span data-ttu-id="f630b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f630b-136">displayName</span></span>|<span data-ttu-id="f630b-137">String</span><span class="sxs-lookup"><span data-stu-id="f630b-137">String</span></span>|<span data-ttu-id="f630b-138">Имя категории</span><span class="sxs-lookup"><span data-stu-id="f630b-138">The category name</span></span>|
|<span data-ttu-id="f630b-139">хасрекуиредсеттинг</span><span class="sxs-lookup"><span data-stu-id="f630b-139">hasRequiredSetting</span></span>|<span data-ttu-id="f630b-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="f630b-140">Boolean</span></span>|<span data-ttu-id="f630b-141">Категория содержит параметры, необходимые для верхнего уровня</span><span class="sxs-lookup"><span data-stu-id="f630b-141">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="f630b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="f630b-142">Response</span></span>
<span data-ttu-id="f630b-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f630b-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f630b-144">Пример</span><span class="sxs-lookup"><span data-stu-id="f630b-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="f630b-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="f630b-145">Request</span></span>
<span data-ttu-id="f630b-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f630b-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f630b-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="f630b-147">Response</span></span>
<span data-ttu-id="f630b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f630b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




