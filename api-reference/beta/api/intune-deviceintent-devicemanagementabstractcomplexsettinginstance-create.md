---
title: Создание Девицеманажементабстракткомплекссеттингинстанце
description: Создание нового объекта Девицеманажементабстракткомплекссеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14f61069ae07034e9b7809d958f683a4bf9587a1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43331198"
---
# <a name="create-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="6c717-103">Создание Девицеманажементабстракткомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="6c717-103">Create deviceManagementAbstractComplexSettingInstance</span></span>

<span data-ttu-id="6c717-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c717-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c717-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c717-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c717-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c717-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c717-107">Создание нового объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="6c717-107">Create a new [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c717-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6c717-108">Prerequisites</span></span>
<span data-ttu-id="6c717-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c717-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c717-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c717-111">Permission type</span></span>|<span data-ttu-id="6c717-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c717-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c717-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c717-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c717-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c717-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c717-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c717-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c717-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c717-116">Not supported.</span></span>|
|<span data-ttu-id="6c717-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c717-117">Application</span></span>|<span data-ttu-id="6c717-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c717-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c717-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c717-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/settings
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="6c717-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6c717-120">Request headers</span></span>
|<span data-ttu-id="6c717-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c717-121">Header</span></span>|<span data-ttu-id="6c717-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6c717-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c717-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c717-123">Authorization</span></span>|<span data-ttu-id="6c717-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c717-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c717-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6c717-125">Accept</span></span>|<span data-ttu-id="6c717-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c717-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c717-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c717-127">Request body</span></span>
<span data-ttu-id="6c717-128">В тексте запроса добавьте представление объекта Девицеманажементабстракткомплекссеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c717-128">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingInstance object.</span></span>

<span data-ttu-id="6c717-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементабстракткомплекссеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="6c717-129">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingInstance.</span></span>

|<span data-ttu-id="6c717-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c717-130">Property</span></span>|<span data-ttu-id="6c717-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6c717-131">Type</span></span>|<span data-ttu-id="6c717-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6c717-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c717-133">id</span><span class="sxs-lookup"><span data-stu-id="6c717-133">id</span></span>|<span data-ttu-id="6c717-134">String</span><span class="sxs-lookup"><span data-stu-id="6c717-134">String</span></span>|<span data-ttu-id="6c717-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="6c717-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="6c717-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="6c717-136">definitionId</span></span>|<span data-ttu-id="6c717-137">String</span><span class="sxs-lookup"><span data-stu-id="6c717-137">String</span></span>|<span data-ttu-id="6c717-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="6c717-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="6c717-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="6c717-139">valueJson</span></span>|<span data-ttu-id="6c717-140">String</span><span class="sxs-lookup"><span data-stu-id="6c717-140">String</span></span>|<span data-ttu-id="6c717-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="6c717-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="6c717-142">имплементатионид</span><span class="sxs-lookup"><span data-stu-id="6c717-142">implementationId</span></span>|<span data-ttu-id="6c717-143">String</span><span class="sxs-lookup"><span data-stu-id="6c717-143">String</span></span>|<span data-ttu-id="6c717-144">Идентификатор определения для выбранной реализации этого сложного параметра</span><span class="sxs-lookup"><span data-stu-id="6c717-144">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="6c717-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c717-145">Response</span></span>
<span data-ttu-id="6c717-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c717-146">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c717-147">Пример</span><span class="sxs-lookup"><span data-stu-id="6c717-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c717-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c717-148">Request</span></span>
<span data-ttu-id="6c717-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c717-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```

### <a name="response"></a><span data-ttu-id="6c717-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c717-150">Response</span></span>
<span data-ttu-id="6c717-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c717-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "id": "433e9565-9565-433e-6595-3e4365953e43",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```



