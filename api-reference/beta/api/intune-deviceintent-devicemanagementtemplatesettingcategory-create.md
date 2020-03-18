---
title: Создание Девицеманажементтемплатесеттингкатегори
description: Создание нового объекта Девицеманажементтемплатесеттингкатегори.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 903a39fd2e5b18742027f583a96e5d69b2d6986f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814969"
---
# <a name="create-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="ccd55-103">Создание Девицеманажементтемплатесеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="ccd55-103">Create deviceManagementTemplateSettingCategory</span></span>

> <span data-ttu-id="ccd55-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccd55-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccd55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccd55-106">Создание нового объекта [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="ccd55-106">Create a new [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccd55-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ccd55-107">Prerequisites</span></span>
<span data-ttu-id="ccd55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccd55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccd55-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccd55-110">Permission type</span></span>|<span data-ttu-id="ccd55-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccd55-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccd55-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccd55-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ccd55-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccd55-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ccd55-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccd55-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccd55-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd55-115">Not supported.</span></span>|
|<span data-ttu-id="ccd55-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ccd55-116">Application</span></span>|<span data-ttu-id="ccd55-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccd55-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccd55-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccd55-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="ccd55-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ccd55-119">Request headers</span></span>
|<span data-ttu-id="ccd55-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ccd55-120">Header</span></span>|<span data-ttu-id="ccd55-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ccd55-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccd55-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccd55-122">Authorization</span></span>|<span data-ttu-id="ccd55-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccd55-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccd55-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ccd55-124">Accept</span></span>|<span data-ttu-id="ccd55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ccd55-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccd55-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccd55-126">Request body</span></span>
<span data-ttu-id="ccd55-127">В тексте запроса добавьте представление объекта Девицеманажементтемплатесеттингкатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccd55-127">In the request body, supply a JSON representation for the deviceManagementTemplateSettingCategory object.</span></span>

<span data-ttu-id="ccd55-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементтемплатесеттингкатегори.</span><span class="sxs-lookup"><span data-stu-id="ccd55-128">The following table shows the properties that are required when you create the deviceManagementTemplateSettingCategory.</span></span>

|<span data-ttu-id="ccd55-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccd55-129">Property</span></span>|<span data-ttu-id="ccd55-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ccd55-130">Type</span></span>|<span data-ttu-id="ccd55-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ccd55-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccd55-132">id</span><span class="sxs-lookup"><span data-stu-id="ccd55-132">id</span></span>|<span data-ttu-id="ccd55-133">String</span><span class="sxs-lookup"><span data-stu-id="ccd55-133">String</span></span>|<span data-ttu-id="ccd55-134">Идентификатор категории, наследуемый от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="ccd55-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="ccd55-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ccd55-135">displayName</span></span>|<span data-ttu-id="ccd55-136">Строка</span><span class="sxs-lookup"><span data-stu-id="ccd55-136">String</span></span>|<span data-ttu-id="ccd55-137">Имя категории, унаследованное от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="ccd55-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="ccd55-138">хасрекуиредсеттинг</span><span class="sxs-lookup"><span data-stu-id="ccd55-138">hasRequiredSetting</span></span>|<span data-ttu-id="ccd55-139">Логический</span><span class="sxs-lookup"><span data-stu-id="ccd55-139">Boolean</span></span>|<span data-ttu-id="ccd55-140">Категория содержит обязательный параметр верхнего уровня, наследуемого от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="ccd55-140">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ccd55-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccd55-141">Response</span></span>
<span data-ttu-id="ccd55-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ccd55-142">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccd55-143">Пример</span><span class="sxs-lookup"><span data-stu-id="ccd55-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccd55-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccd55-144">Request</span></span>
<span data-ttu-id="ccd55-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccd55-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories
Content-type: application/json
Content-length: 152

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="ccd55-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccd55-146">Response</span></span>
<span data-ttu-id="ccd55-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccd55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 201

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "cd213562-3562-cd21-6235-21cd623521cd",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




