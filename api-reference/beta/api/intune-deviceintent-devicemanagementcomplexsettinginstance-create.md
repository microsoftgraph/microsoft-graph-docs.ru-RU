---
title: Создание Девицеманажементкомплекссеттингинстанце
description: Создание нового объекта Девицеманажементкомплекссеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7679acd366a0aca354f1252b0bc9447fad16e9f8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946044"
---
# <a name="create-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="dc494-103">Создание Девицеманажементкомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="dc494-103">Create deviceManagementComplexSettingInstance</span></span>

> <span data-ttu-id="dc494-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc494-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc494-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc494-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc494-106">Создание нового объекта [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="dc494-106">Create a new [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc494-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dc494-107">Prerequisites</span></span>
<span data-ttu-id="dc494-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc494-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc494-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc494-110">Permission type</span></span>|<span data-ttu-id="dc494-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc494-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc494-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc494-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc494-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc494-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc494-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc494-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc494-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc494-115">Not supported.</span></span>|
|<span data-ttu-id="dc494-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc494-116">Application</span></span>|<span data-ttu-id="dc494-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc494-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc494-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc494-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="dc494-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dc494-119">Request headers</span></span>
|<span data-ttu-id="dc494-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc494-120">Header</span></span>|<span data-ttu-id="dc494-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dc494-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc494-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc494-122">Authorization</span></span>|<span data-ttu-id="dc494-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc494-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc494-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dc494-124">Accept</span></span>|<span data-ttu-id="dc494-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc494-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc494-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dc494-126">Request body</span></span>
<span data-ttu-id="dc494-127">В тексте запроса добавьте представление объекта Девицеманажементкомплекссеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc494-127">In the request body, supply a JSON representation for the deviceManagementComplexSettingInstance object.</span></span>

<span data-ttu-id="dc494-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементкомплекссеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="dc494-128">The following table shows the properties that are required when you create the deviceManagementComplexSettingInstance.</span></span>

|<span data-ttu-id="dc494-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc494-129">Property</span></span>|<span data-ttu-id="dc494-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dc494-130">Type</span></span>|<span data-ttu-id="dc494-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dc494-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc494-132">id</span><span class="sxs-lookup"><span data-stu-id="dc494-132">id</span></span>|<span data-ttu-id="dc494-133">Строка</span><span class="sxs-lookup"><span data-stu-id="dc494-133">String</span></span>|<span data-ttu-id="dc494-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="dc494-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="dc494-135">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="dc494-135">definitionId</span></span>|<span data-ttu-id="dc494-136">Строка</span><span class="sxs-lookup"><span data-stu-id="dc494-136">String</span></span>|<span data-ttu-id="dc494-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="dc494-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="dc494-138">валуежсон</span><span class="sxs-lookup"><span data-stu-id="dc494-138">valueJson</span></span>|<span data-ttu-id="dc494-139">Строка</span><span class="sxs-lookup"><span data-stu-id="dc494-139">String</span></span>|<span data-ttu-id="dc494-140">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="dc494-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="dc494-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc494-141">Response</span></span>
<span data-ttu-id="dc494-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dc494-142">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc494-143">Пример</span><span class="sxs-lookup"><span data-stu-id="dc494-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc494-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc494-144">Request</span></span>
<span data-ttu-id="dc494-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc494-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dc494-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc494-146">Response</span></span>
<span data-ttu-id="dc494-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc494-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





