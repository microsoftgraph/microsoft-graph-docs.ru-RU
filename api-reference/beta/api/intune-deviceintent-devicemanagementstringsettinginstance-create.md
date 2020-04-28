---
title: Создание Девицеманажементстрингсеттингинстанце
description: Создание нового объекта Девицеманажементстрингсеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f4f52a8bfe2087594da5d8da98e9cac0ca56a2fe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43325259"
---
# <a name="create-devicemanagementstringsettinginstance"></a><span data-ttu-id="277a9-103">Создание Девицеманажементстрингсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="277a9-103">Create deviceManagementStringSettingInstance</span></span>

<span data-ttu-id="277a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="277a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="277a9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="277a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="277a9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="277a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="277a9-107">Создание нового объекта [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="277a9-107">Create a new [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="277a9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="277a9-108">Prerequisites</span></span>
<span data-ttu-id="277a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="277a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="277a9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="277a9-111">Permission type</span></span>|<span data-ttu-id="277a9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="277a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="277a9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="277a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="277a9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="277a9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="277a9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="277a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="277a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="277a9-116">Not supported.</span></span>|
|<span data-ttu-id="277a9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="277a9-117">Application</span></span>|<span data-ttu-id="277a9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="277a9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="277a9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="277a9-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="277a9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="277a9-120">Request headers</span></span>
|<span data-ttu-id="277a9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="277a9-121">Header</span></span>|<span data-ttu-id="277a9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="277a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="277a9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="277a9-123">Authorization</span></span>|<span data-ttu-id="277a9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="277a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="277a9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="277a9-125">Accept</span></span>|<span data-ttu-id="277a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="277a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="277a9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="277a9-127">Request body</span></span>
<span data-ttu-id="277a9-128">В тексте запроса добавьте представление объекта Девицеманажементстрингсеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="277a9-128">In the request body, supply a JSON representation for the deviceManagementStringSettingInstance object.</span></span>

<span data-ttu-id="277a9-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементстрингсеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="277a9-129">The following table shows the properties that are required when you create the deviceManagementStringSettingInstance.</span></span>

|<span data-ttu-id="277a9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="277a9-130">Property</span></span>|<span data-ttu-id="277a9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="277a9-131">Type</span></span>|<span data-ttu-id="277a9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="277a9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="277a9-133">id</span><span class="sxs-lookup"><span data-stu-id="277a9-133">id</span></span>|<span data-ttu-id="277a9-134">String</span><span class="sxs-lookup"><span data-stu-id="277a9-134">String</span></span>|<span data-ttu-id="277a9-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="277a9-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="277a9-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="277a9-136">definitionId</span></span>|<span data-ttu-id="277a9-137">String</span><span class="sxs-lookup"><span data-stu-id="277a9-137">String</span></span>|<span data-ttu-id="277a9-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="277a9-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="277a9-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="277a9-139">valueJson</span></span>|<span data-ttu-id="277a9-140">String</span><span class="sxs-lookup"><span data-stu-id="277a9-140">String</span></span>|<span data-ttu-id="277a9-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="277a9-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="277a9-142">value</span><span class="sxs-lookup"><span data-stu-id="277a9-142">value</span></span>|<span data-ttu-id="277a9-143">String</span><span class="sxs-lookup"><span data-stu-id="277a9-143">String</span></span>|<span data-ttu-id="277a9-144">Строковое значение</span><span class="sxs-lookup"><span data-stu-id="277a9-144">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="277a9-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="277a9-145">Response</span></span>
<span data-ttu-id="277a9-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="277a9-146">If successful, this method returns a `201 Created` response code and a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="277a9-147">Пример</span><span class="sxs-lookup"><span data-stu-id="277a9-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="277a9-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="277a9-148">Request</span></span>
<span data-ttu-id="277a9-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="277a9-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="277a9-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="277a9-150">Response</span></span>
<span data-ttu-id="277a9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="277a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "id": "fef30638-0638-fef3-3806-f3fe3806f3fe",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```



