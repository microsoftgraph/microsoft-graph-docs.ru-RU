---
title: Создание Девицеманажементкомплекссеттингинстанце
description: Создание нового объекта Девицеманажементкомплекссеттингинстанце.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: be2c0cbcbdabf13a55645754875ff5c72278cecd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42730104"
---
# <a name="create-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="28360-103">Создание Девицеманажементкомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="28360-103">Create deviceManagementComplexSettingInstance</span></span>

> <span data-ttu-id="28360-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28360-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28360-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28360-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28360-106">Создание нового объекта [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="28360-106">Create a new [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28360-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="28360-107">Prerequisites</span></span>
<span data-ttu-id="28360-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28360-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28360-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28360-110">Permission type</span></span>|<span data-ttu-id="28360-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="28360-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28360-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28360-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28360-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28360-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28360-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28360-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28360-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28360-115">Not supported.</span></span>|
|<span data-ttu-id="28360-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="28360-116">Application</span></span>|<span data-ttu-id="28360-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28360-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28360-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28360-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="28360-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="28360-119">Request headers</span></span>
|<span data-ttu-id="28360-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28360-120">Header</span></span>|<span data-ttu-id="28360-121">Значение</span><span class="sxs-lookup"><span data-stu-id="28360-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28360-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28360-122">Authorization</span></span>|<span data-ttu-id="28360-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28360-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28360-124">Accept</span><span class="sxs-lookup"><span data-stu-id="28360-124">Accept</span></span>|<span data-ttu-id="28360-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28360-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28360-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28360-126">Request body</span></span>
<span data-ttu-id="28360-127">В тексте запроса добавьте представление объекта Девицеманажементкомплекссеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28360-127">In the request body, supply a JSON representation for the deviceManagementComplexSettingInstance object.</span></span>

<span data-ttu-id="28360-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементкомплекссеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="28360-128">The following table shows the properties that are required when you create the deviceManagementComplexSettingInstance.</span></span>

|<span data-ttu-id="28360-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="28360-129">Property</span></span>|<span data-ttu-id="28360-130">Тип</span><span class="sxs-lookup"><span data-stu-id="28360-130">Type</span></span>|<span data-ttu-id="28360-131">Описание</span><span class="sxs-lookup"><span data-stu-id="28360-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28360-132">id</span><span class="sxs-lookup"><span data-stu-id="28360-132">id</span></span>|<span data-ttu-id="28360-133">String</span><span class="sxs-lookup"><span data-stu-id="28360-133">String</span></span>|<span data-ttu-id="28360-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="28360-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="28360-135">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="28360-135">definitionId</span></span>|<span data-ttu-id="28360-136">String</span><span class="sxs-lookup"><span data-stu-id="28360-136">String</span></span>|<span data-ttu-id="28360-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="28360-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="28360-138">валуежсон</span><span class="sxs-lookup"><span data-stu-id="28360-138">valueJson</span></span>|<span data-ttu-id="28360-139">String</span><span class="sxs-lookup"><span data-stu-id="28360-139">String</span></span>|<span data-ttu-id="28360-140">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="28360-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="28360-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="28360-141">Response</span></span>
<span data-ttu-id="28360-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28360-142">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28360-143">Пример</span><span class="sxs-lookup"><span data-stu-id="28360-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="28360-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="28360-144">Request</span></span>
<span data-ttu-id="28360-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28360-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="28360-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="28360-146">Response</span></span>
<span data-ttu-id="28360-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28360-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 207

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```




