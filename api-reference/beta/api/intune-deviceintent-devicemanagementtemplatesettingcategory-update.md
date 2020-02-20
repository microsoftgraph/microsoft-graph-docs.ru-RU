---
title: Обновление Девицеманажементтемплатесеттингкатегори
description: Обновление свойств объекта Девицеманажементтемплатесеттингкатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4cde03209d777eeb21c8d2caaee9973e512784c4
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162269"
---
# <a name="update-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="867f3-103">Обновление Девицеманажементтемплатесеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="867f3-103">Update deviceManagementTemplateSettingCategory</span></span>

> <span data-ttu-id="867f3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="867f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="867f3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="867f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="867f3-106">Обновление свойств объекта [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="867f3-106">Update the properties of a [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="867f3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="867f3-107">Prerequisites</span></span>
<span data-ttu-id="867f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="867f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="867f3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="867f3-110">Permission type</span></span>|<span data-ttu-id="867f3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="867f3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="867f3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="867f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="867f3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="867f3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="867f3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="867f3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="867f3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="867f3-115">Not supported.</span></span>|
|<span data-ttu-id="867f3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="867f3-116">Application</span></span>|<span data-ttu-id="867f3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="867f3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="867f3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="867f3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="867f3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="867f3-119">Request headers</span></span>
|<span data-ttu-id="867f3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="867f3-120">Header</span></span>|<span data-ttu-id="867f3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="867f3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="867f3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="867f3-122">Authorization</span></span>|<span data-ttu-id="867f3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="867f3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="867f3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="867f3-124">Accept</span></span>|<span data-ttu-id="867f3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="867f3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="867f3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="867f3-126">Request body</span></span>
<span data-ttu-id="867f3-127">В тексте запроса добавьте представление объекта [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="867f3-127">In the request body, supply a JSON representation for the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

<span data-ttu-id="867f3-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="867f3-128">The following table shows the properties that are required when you create the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md).</span></span>

|<span data-ttu-id="867f3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="867f3-129">Property</span></span>|<span data-ttu-id="867f3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="867f3-130">Type</span></span>|<span data-ttu-id="867f3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="867f3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="867f3-132">id</span><span class="sxs-lookup"><span data-stu-id="867f3-132">id</span></span>|<span data-ttu-id="867f3-133">String</span><span class="sxs-lookup"><span data-stu-id="867f3-133">String</span></span>|<span data-ttu-id="867f3-134">Идентификатор категории, наследуемый от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="867f3-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="867f3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="867f3-135">displayName</span></span>|<span data-ttu-id="867f3-136">Строка</span><span class="sxs-lookup"><span data-stu-id="867f3-136">String</span></span>|<span data-ttu-id="867f3-137">Имя категории, унаследованное от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="867f3-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="867f3-138">хасрекуиредсеттинг</span><span class="sxs-lookup"><span data-stu-id="867f3-138">hasRequiredSetting</span></span>|<span data-ttu-id="867f3-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="867f3-139">Boolean</span></span>|<span data-ttu-id="867f3-140">Категория содержит обязательный параметр верхнего уровня, наследуемого от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="867f3-140">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="867f3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="867f3-141">Response</span></span>
<span data-ttu-id="867f3-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="867f3-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="867f3-143">Пример</span><span class="sxs-lookup"><span data-stu-id="867f3-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="867f3-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="867f3-144">Request</span></span>
<span data-ttu-id="867f3-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="867f3-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
Content-type: application/json
Content-length: 152

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="867f3-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="867f3-146">Response</span></span>
<span data-ttu-id="867f3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="867f3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 201

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "cd213562-3562-cd21-6235-21cd623521cd",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```





