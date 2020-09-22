---
title: Создание Девицеманажементкомплекссеттингинстанце
description: Создание нового объекта Девицеманажементкомплекссеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 64335a7d5737f93f29afa52e433158fddbe3d640
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088246"
---
# <a name="create-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="b6bca-103">Создание Девицеманажементкомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="b6bca-103">Create deviceManagementComplexSettingInstance</span></span>

<span data-ttu-id="b6bca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6bca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6bca-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6bca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6bca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6bca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6bca-107">Создание нового объекта [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="b6bca-107">Create a new [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6bca-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6bca-108">Prerequisites</span></span>
<span data-ttu-id="b6bca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6bca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6bca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6bca-111">Permission type</span></span>|<span data-ttu-id="b6bca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6bca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6bca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6bca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6bca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6bca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6bca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6bca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6bca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6bca-116">Not supported.</span></span>|
|<span data-ttu-id="b6bca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6bca-117">Application</span></span>|<span data-ttu-id="b6bca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6bca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6bca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6bca-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b6bca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b6bca-120">Request headers</span></span>
|<span data-ttu-id="b6bca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6bca-121">Header</span></span>|<span data-ttu-id="b6bca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b6bca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6bca-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6bca-123">Authorization</span></span>|<span data-ttu-id="b6bca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6bca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6bca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6bca-125">Accept</span></span>|<span data-ttu-id="b6bca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6bca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6bca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6bca-127">Request body</span></span>
<span data-ttu-id="b6bca-128">В тексте запроса добавьте представление объекта Девицеманажементкомплекссеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6bca-128">In the request body, supply a JSON representation for the deviceManagementComplexSettingInstance object.</span></span>

<span data-ttu-id="b6bca-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементкомплекссеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="b6bca-129">The following table shows the properties that are required when you create the deviceManagementComplexSettingInstance.</span></span>

|<span data-ttu-id="b6bca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6bca-130">Property</span></span>|<span data-ttu-id="b6bca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b6bca-131">Type</span></span>|<span data-ttu-id="b6bca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b6bca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6bca-133">id</span><span class="sxs-lookup"><span data-stu-id="b6bca-133">id</span></span>|<span data-ttu-id="b6bca-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b6bca-134">String</span></span>|<span data-ttu-id="b6bca-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="b6bca-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="b6bca-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="b6bca-136">definitionId</span></span>|<span data-ttu-id="b6bca-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b6bca-137">String</span></span>|<span data-ttu-id="b6bca-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="b6bca-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="b6bca-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="b6bca-139">valueJson</span></span>|<span data-ttu-id="b6bca-140">Строка</span><span class="sxs-lookup"><span data-stu-id="b6bca-140">String</span></span>|<span data-ttu-id="b6bca-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="b6bca-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b6bca-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6bca-142">Response</span></span>
<span data-ttu-id="b6bca-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6bca-143">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6bca-144">Пример</span><span class="sxs-lookup"><span data-stu-id="b6bca-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6bca-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6bca-145">Request</span></span>
<span data-ttu-id="b6bca-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6bca-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6bca-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6bca-147">Response</span></span>
<span data-ttu-id="b6bca-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6bca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






