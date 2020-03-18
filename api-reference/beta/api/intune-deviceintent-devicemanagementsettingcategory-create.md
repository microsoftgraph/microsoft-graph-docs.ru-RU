---
title: Создание Девицеманажементсеттингкатегори
description: Создание нового объекта Девицеманажементсеттингкатегори.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 331437082df79e302c3ab9a2b3603fbf5e8963ea
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815137"
---
# <a name="create-devicemanagementsettingcategory"></a><span data-ttu-id="3adb9-103">Создание Девицеманажементсеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="3adb9-103">Create deviceManagementSettingCategory</span></span>

> <span data-ttu-id="3adb9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3adb9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3adb9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3adb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3adb9-106">Создание нового объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="3adb9-106">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3adb9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3adb9-107">Prerequisites</span></span>
<span data-ttu-id="3adb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3adb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3adb9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3adb9-110">Permission type</span></span>|<span data-ttu-id="3adb9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3adb9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3adb9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3adb9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3adb9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3adb9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3adb9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3adb9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3adb9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3adb9-115">Not supported.</span></span>|
|<span data-ttu-id="3adb9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3adb9-116">Application</span></span>|<span data-ttu-id="3adb9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3adb9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3adb9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3adb9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/categories
```

## <a name="request-headers"></a><span data-ttu-id="3adb9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3adb9-119">Request headers</span></span>
|<span data-ttu-id="3adb9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3adb9-120">Header</span></span>|<span data-ttu-id="3adb9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3adb9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3adb9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3adb9-122">Authorization</span></span>|<span data-ttu-id="3adb9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3adb9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3adb9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3adb9-124">Accept</span></span>|<span data-ttu-id="3adb9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3adb9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3adb9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3adb9-126">Request body</span></span>
<span data-ttu-id="3adb9-127">В тексте запроса добавьте представление объекта Девицеманажементсеттингкатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3adb9-127">In the request body, supply a JSON representation for the deviceManagementSettingCategory object.</span></span>

<span data-ttu-id="3adb9-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементсеттингкатегори.</span><span class="sxs-lookup"><span data-stu-id="3adb9-128">The following table shows the properties that are required when you create the deviceManagementSettingCategory.</span></span>

|<span data-ttu-id="3adb9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3adb9-129">Property</span></span>|<span data-ttu-id="3adb9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3adb9-130">Type</span></span>|<span data-ttu-id="3adb9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3adb9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3adb9-132">id</span><span class="sxs-lookup"><span data-stu-id="3adb9-132">id</span></span>|<span data-ttu-id="3adb9-133">String</span><span class="sxs-lookup"><span data-stu-id="3adb9-133">String</span></span>|<span data-ttu-id="3adb9-134">Идентификатор категории</span><span class="sxs-lookup"><span data-stu-id="3adb9-134">The category ID</span></span>|
|<span data-ttu-id="3adb9-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3adb9-135">displayName</span></span>|<span data-ttu-id="3adb9-136">Строка</span><span class="sxs-lookup"><span data-stu-id="3adb9-136">String</span></span>|<span data-ttu-id="3adb9-137">Имя категории</span><span class="sxs-lookup"><span data-stu-id="3adb9-137">The category name</span></span>|
|<span data-ttu-id="3adb9-138">хасрекуиредсеттинг</span><span class="sxs-lookup"><span data-stu-id="3adb9-138">hasRequiredSetting</span></span>|<span data-ttu-id="3adb9-139">Логический</span><span class="sxs-lookup"><span data-stu-id="3adb9-139">Boolean</span></span>|<span data-ttu-id="3adb9-140">Категория содержит параметры, необходимые для верхнего уровня</span><span class="sxs-lookup"><span data-stu-id="3adb9-140">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="3adb9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3adb9-141">Response</span></span>
<span data-ttu-id="3adb9-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3adb9-142">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3adb9-143">Пример</span><span class="sxs-lookup"><span data-stu-id="3adb9-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="3adb9-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="3adb9-144">Request</span></span>
<span data-ttu-id="3adb9-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3adb9-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/categories
Content-type: application/json
Content-length: 144

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="3adb9-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="3adb9-146">Response</span></span>
<span data-ttu-id="3adb9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3adb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 193

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




