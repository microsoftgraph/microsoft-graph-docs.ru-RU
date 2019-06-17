---
title: Обновление Девицеманажементинтент
description: Обновление свойств объекта Девицеманажементинтент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd8b85ccab0153b749ff29be13187e3fd2fd4ef6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960449"
---
# <a name="update-devicemanagementintent"></a><span data-ttu-id="e4a50-103">Обновление Девицеманажементинтент</span><span class="sxs-lookup"><span data-stu-id="e4a50-103">Update deviceManagementIntent</span></span>

> <span data-ttu-id="e4a50-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4a50-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4a50-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4a50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4a50-106">Обновление свойств объекта [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) .</span><span class="sxs-lookup"><span data-stu-id="e4a50-106">Update the properties of a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4a50-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e4a50-107">Prerequisites</span></span>
<span data-ttu-id="e4a50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4a50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4a50-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4a50-110">Permission type</span></span>|<span data-ttu-id="e4a50-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4a50-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4a50-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4a50-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4a50-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a50-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4a50-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4a50-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4a50-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4a50-115">Not supported.</span></span>|
|<span data-ttu-id="e4a50-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4a50-116">Application</span></span>|<span data-ttu-id="e4a50-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4a50-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4a50-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4a50-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}
```

## <a name="request-headers"></a><span data-ttu-id="e4a50-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4a50-119">Request headers</span></span>
|<span data-ttu-id="e4a50-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4a50-120">Header</span></span>|<span data-ttu-id="e4a50-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e4a50-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4a50-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4a50-122">Authorization</span></span>|<span data-ttu-id="e4a50-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4a50-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4a50-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e4a50-124">Accept</span></span>|<span data-ttu-id="e4a50-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4a50-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4a50-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4a50-126">Request body</span></span>
<span data-ttu-id="e4a50-127">В тексте запроса добавьте представление объекта [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4a50-127">In the request body, supply a JSON representation for the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

<span data-ttu-id="e4a50-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md).</span><span class="sxs-lookup"><span data-stu-id="e4a50-128">The following table shows the properties that are required when you create the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).</span></span>

|<span data-ttu-id="e4a50-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4a50-129">Property</span></span>|<span data-ttu-id="e4a50-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e4a50-130">Type</span></span>|<span data-ttu-id="e4a50-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e4a50-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4a50-132">id</span><span class="sxs-lookup"><span data-stu-id="e4a50-132">id</span></span>|<span data-ttu-id="e4a50-133">String</span><span class="sxs-lookup"><span data-stu-id="e4a50-133">String</span></span>|<span data-ttu-id="e4a50-134">Идентификатор намерения</span><span class="sxs-lookup"><span data-stu-id="e4a50-134">The intent ID</span></span>|
|<span data-ttu-id="e4a50-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e4a50-135">displayName</span></span>|<span data-ttu-id="e4a50-136">Строка</span><span class="sxs-lookup"><span data-stu-id="e4a50-136">String</span></span>|<span data-ttu-id="e4a50-137">Имя пользователя для данного отображаемого имени</span><span class="sxs-lookup"><span data-stu-id="e4a50-137">The user given display name</span></span>|
|<span data-ttu-id="e4a50-138">description</span><span class="sxs-lookup"><span data-stu-id="e4a50-138">description</span></span>|<span data-ttu-id="e4a50-139">String</span><span class="sxs-lookup"><span data-stu-id="e4a50-139">String</span></span>|<span data-ttu-id="e4a50-140">Описание, заданное пользователем</span><span class="sxs-lookup"><span data-stu-id="e4a50-140">The user given description</span></span>|
|<span data-ttu-id="e4a50-141">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e4a50-141">isAssigned</span></span>|<span data-ttu-id="e4a50-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4a50-142">Boolean</span></span>|<span data-ttu-id="e4a50-143">Указывает, назначена ли пользователю задача</span><span class="sxs-lookup"><span data-stu-id="e4a50-143">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="e4a50-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4a50-144">lastModifiedDateTime</span></span>|<span data-ttu-id="e4a50-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4a50-145">DateTimeOffset</span></span>|<span data-ttu-id="e4a50-146">Время последнего изменения намерения</span><span class="sxs-lookup"><span data-stu-id="e4a50-146">When the intent was last modified</span></span>|
|<span data-ttu-id="e4a50-147">templateId</span><span class="sxs-lookup"><span data-stu-id="e4a50-147">templateId</span></span>|<span data-ttu-id="e4a50-148">String</span><span class="sxs-lookup"><span data-stu-id="e4a50-148">String</span></span>|<span data-ttu-id="e4a50-149">Идентификатор шаблона, на основе которого была создана эта цель (при наличии)</span><span class="sxs-lookup"><span data-stu-id="e4a50-149">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="e4a50-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e4a50-150">roleScopeTagIds</span></span>|<span data-ttu-id="e4a50-151">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e4a50-151">String collection</span></span>|<span data-ttu-id="e4a50-152">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e4a50-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="e4a50-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4a50-153">Response</span></span>
<span data-ttu-id="e4a50-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4a50-154">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4a50-155">Пример</span><span class="sxs-lookup"><span data-stu-id="e4a50-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4a50-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4a50-156">Request</span></span>
<span data-ttu-id="e4a50-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4a50-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="e4a50-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4a50-158">Response</span></span>
<span data-ttu-id="e4a50-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4a50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





