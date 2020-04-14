---
title: Создание Девицеманажементтемплатесеттингкатегори
description: Создание нового объекта Девицеманажементтемплатесеттингкатегори.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5550c696b9b8b039f913fcb4843f9858b8f21a74
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43427475"
---
# <a name="create-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="adfce-103">Создание Девицеманажементтемплатесеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="adfce-103">Create deviceManagementTemplateSettingCategory</span></span>

<span data-ttu-id="adfce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adfce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="adfce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adfce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adfce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="adfce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adfce-107">Создание нового объекта [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="adfce-107">Create a new [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adfce-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="adfce-108">Prerequisites</span></span>
<span data-ttu-id="adfce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adfce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adfce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adfce-111">Permission type</span></span>|<span data-ttu-id="adfce-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="adfce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adfce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adfce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adfce-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adfce-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="adfce-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adfce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adfce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adfce-116">Not supported.</span></span>|
|<span data-ttu-id="adfce-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="adfce-117">Application</span></span>|<span data-ttu-id="adfce-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adfce-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="adfce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adfce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="adfce-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="adfce-120">Request headers</span></span>
|<span data-ttu-id="adfce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="adfce-121">Header</span></span>|<span data-ttu-id="adfce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="adfce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adfce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="adfce-123">Authorization</span></span>|<span data-ttu-id="adfce-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="adfce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adfce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="adfce-125">Accept</span></span>|<span data-ttu-id="adfce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="adfce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adfce-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="adfce-127">Request body</span></span>
<span data-ttu-id="adfce-128">В тексте запроса добавьте представление объекта Девицеманажементтемплатесеттингкатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adfce-128">In the request body, supply a JSON representation for the deviceManagementTemplateSettingCategory object.</span></span>

<span data-ttu-id="adfce-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементтемплатесеттингкатегори.</span><span class="sxs-lookup"><span data-stu-id="adfce-129">The following table shows the properties that are required when you create the deviceManagementTemplateSettingCategory.</span></span>

|<span data-ttu-id="adfce-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="adfce-130">Property</span></span>|<span data-ttu-id="adfce-131">Тип</span><span class="sxs-lookup"><span data-stu-id="adfce-131">Type</span></span>|<span data-ttu-id="adfce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="adfce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adfce-133">id</span><span class="sxs-lookup"><span data-stu-id="adfce-133">id</span></span>|<span data-ttu-id="adfce-134">String</span><span class="sxs-lookup"><span data-stu-id="adfce-134">String</span></span>|<span data-ttu-id="adfce-135">Идентификатор категории, наследуемый от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="adfce-135">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="adfce-136">displayName</span><span class="sxs-lookup"><span data-stu-id="adfce-136">displayName</span></span>|<span data-ttu-id="adfce-137">Строка</span><span class="sxs-lookup"><span data-stu-id="adfce-137">String</span></span>|<span data-ttu-id="adfce-138">Имя категории, унаследованное от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="adfce-138">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="adfce-139">хасрекуиредсеттинг</span><span class="sxs-lookup"><span data-stu-id="adfce-139">hasRequiredSetting</span></span>|<span data-ttu-id="adfce-140">Логическое</span><span class="sxs-lookup"><span data-stu-id="adfce-140">Boolean</span></span>|<span data-ttu-id="adfce-141">Категория содержит обязательный параметр верхнего уровня, наследуемого от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="adfce-141">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="adfce-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="adfce-142">Response</span></span>
<span data-ttu-id="adfce-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="adfce-143">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adfce-144">Пример</span><span class="sxs-lookup"><span data-stu-id="adfce-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="adfce-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="adfce-145">Request</span></span>
<span data-ttu-id="adfce-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adfce-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="adfce-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="adfce-147">Response</span></span>
<span data-ttu-id="adfce-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adfce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



