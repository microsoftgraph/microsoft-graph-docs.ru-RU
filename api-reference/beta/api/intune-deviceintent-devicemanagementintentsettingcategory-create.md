---
title: Создание Девицеманажементинтентсеттингкатегори
description: Создание нового объекта Девицеманажементинтентсеттингкатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c92ab47984984bc97e37ab071798ba345a0c963c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470877"
---
# <a name="create-devicemanagementintentsettingcategory"></a><span data-ttu-id="2e259-103">Создание Девицеманажементинтентсеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="2e259-103">Create deviceManagementIntentSettingCategory</span></span>

<span data-ttu-id="2e259-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2e259-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e259-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e259-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e259-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e259-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e259-107">Создание нового объекта [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="2e259-107">Create a new [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e259-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2e259-108">Prerequisites</span></span>
<span data-ttu-id="2e259-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e259-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e259-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e259-111">Permission type</span></span>|<span data-ttu-id="2e259-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e259-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e259-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e259-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e259-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e259-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2e259-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e259-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e259-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e259-116">Not supported.</span></span>|
|<span data-ttu-id="2e259-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e259-117">Application</span></span>|<span data-ttu-id="2e259-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e259-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e259-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e259-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="2e259-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2e259-120">Request headers</span></span>
|<span data-ttu-id="2e259-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e259-121">Header</span></span>|<span data-ttu-id="2e259-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2e259-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e259-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e259-123">Authorization</span></span>|<span data-ttu-id="2e259-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e259-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e259-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2e259-125">Accept</span></span>|<span data-ttu-id="2e259-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e259-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e259-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e259-127">Request body</span></span>
<span data-ttu-id="2e259-128">В тексте запроса добавьте представление объекта Девицеманажементинтентсеттингкатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e259-128">In the request body, supply a JSON representation for the deviceManagementIntentSettingCategory object.</span></span>

<span data-ttu-id="2e259-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтентсеттингкатегори.</span><span class="sxs-lookup"><span data-stu-id="2e259-129">The following table shows the properties that are required when you create the deviceManagementIntentSettingCategory.</span></span>

|<span data-ttu-id="2e259-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e259-130">Property</span></span>|<span data-ttu-id="2e259-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2e259-131">Type</span></span>|<span data-ttu-id="2e259-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2e259-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e259-133">id</span><span class="sxs-lookup"><span data-stu-id="2e259-133">id</span></span>|<span data-ttu-id="2e259-134">String</span><span class="sxs-lookup"><span data-stu-id="2e259-134">String</span></span>|<span data-ttu-id="2e259-135">Идентификатор категории, наследуемый от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="2e259-135">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="2e259-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2e259-136">displayName</span></span>|<span data-ttu-id="2e259-137">Строка</span><span class="sxs-lookup"><span data-stu-id="2e259-137">String</span></span>|<span data-ttu-id="2e259-138">Имя категории, унаследованное от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="2e259-138">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="2e259-139">хасрекуиредсеттинг</span><span class="sxs-lookup"><span data-stu-id="2e259-139">hasRequiredSetting</span></span>|<span data-ttu-id="2e259-140">Логический</span><span class="sxs-lookup"><span data-stu-id="2e259-140">Boolean</span></span>|<span data-ttu-id="2e259-141">Категория содержит обязательный параметр верхнего уровня, наследуемого от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="2e259-141">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2e259-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e259-142">Response</span></span>
<span data-ttu-id="2e259-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e259-143">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e259-144">Пример</span><span class="sxs-lookup"><span data-stu-id="2e259-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e259-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e259-145">Request</span></span>
<span data-ttu-id="2e259-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e259-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2e259-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e259-147">Response</span></span>
<span data-ttu-id="2e259-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e259-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





