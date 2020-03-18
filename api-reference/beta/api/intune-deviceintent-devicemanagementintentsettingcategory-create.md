---
title: Создание Девицеманажементинтентсеттингкатегори
description: Создание нового объекта Девицеманажементинтентсеттингкатегори.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 360c2277c6cac339c5000e58c73759f846bcc4ae
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815221"
---
# <a name="create-devicemanagementintentsettingcategory"></a><span data-ttu-id="b6931-103">Создание Девицеманажементинтентсеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="b6931-103">Create deviceManagementIntentSettingCategory</span></span>

> <span data-ttu-id="b6931-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6931-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6931-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6931-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6931-106">Создание нового объекта [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="b6931-106">Create a new [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6931-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6931-107">Prerequisites</span></span>
<span data-ttu-id="b6931-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6931-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6931-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6931-110">Permission type</span></span>|<span data-ttu-id="b6931-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6931-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6931-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6931-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6931-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6931-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6931-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6931-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6931-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6931-115">Not supported.</span></span>|
|<span data-ttu-id="b6931-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b6931-116">Application</span></span>|<span data-ttu-id="b6931-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6931-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6931-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6931-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="b6931-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b6931-119">Request headers</span></span>
|<span data-ttu-id="b6931-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6931-120">Header</span></span>|<span data-ttu-id="b6931-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b6931-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6931-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6931-122">Authorization</span></span>|<span data-ttu-id="b6931-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6931-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6931-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b6931-124">Accept</span></span>|<span data-ttu-id="b6931-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6931-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6931-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6931-126">Request body</span></span>
<span data-ttu-id="b6931-127">В тексте запроса добавьте представление объекта Девицеманажементинтентсеттингкатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6931-127">In the request body, supply a JSON representation for the deviceManagementIntentSettingCategory object.</span></span>

<span data-ttu-id="b6931-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтентсеттингкатегори.</span><span class="sxs-lookup"><span data-stu-id="b6931-128">The following table shows the properties that are required when you create the deviceManagementIntentSettingCategory.</span></span>

|<span data-ttu-id="b6931-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6931-129">Property</span></span>|<span data-ttu-id="b6931-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b6931-130">Type</span></span>|<span data-ttu-id="b6931-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b6931-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6931-132">id</span><span class="sxs-lookup"><span data-stu-id="b6931-132">id</span></span>|<span data-ttu-id="b6931-133">String</span><span class="sxs-lookup"><span data-stu-id="b6931-133">String</span></span>|<span data-ttu-id="b6931-134">Идентификатор категории, наследуемый от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="b6931-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="b6931-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b6931-135">displayName</span></span>|<span data-ttu-id="b6931-136">Строка</span><span class="sxs-lookup"><span data-stu-id="b6931-136">String</span></span>|<span data-ttu-id="b6931-137">Имя категории, унаследованное от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="b6931-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="b6931-138">хасрекуиредсеттинг</span><span class="sxs-lookup"><span data-stu-id="b6931-138">hasRequiredSetting</span></span>|<span data-ttu-id="b6931-139">Логический</span><span class="sxs-lookup"><span data-stu-id="b6931-139">Boolean</span></span>|<span data-ttu-id="b6931-140">Категория содержит обязательный параметр верхнего уровня, наследуемого от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="b6931-140">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b6931-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6931-141">Response</span></span>
<span data-ttu-id="b6931-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6931-142">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6931-143">Пример</span><span class="sxs-lookup"><span data-stu-id="b6931-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6931-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6931-144">Request</span></span>
<span data-ttu-id="b6931-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6931-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories
Content-type: application/json
Content-length: 150

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="b6931-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6931-146">Response</span></span>
<span data-ttu-id="b6931-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6931-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 199

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




