---
title: Обновление Девицеманажементинтент
description: Обновление свойств объекта Девицеманажементинтент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 30057c5ca95b305aa749b063b8601dc0ae120382
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43327821"
---
# <a name="update-devicemanagementintent"></a><span data-ttu-id="47266-103">Обновление Девицеманажементинтент</span><span class="sxs-lookup"><span data-stu-id="47266-103">Update deviceManagementIntent</span></span>

<span data-ttu-id="47266-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47266-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47266-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47266-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47266-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47266-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47266-107">Обновление свойств объекта [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) .</span><span class="sxs-lookup"><span data-stu-id="47266-107">Update the properties of a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47266-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="47266-108">Prerequisites</span></span>
<span data-ttu-id="47266-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47266-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47266-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47266-111">Permission type</span></span>|<span data-ttu-id="47266-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47266-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47266-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47266-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47266-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47266-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47266-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47266-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47266-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47266-116">Not supported.</span></span>|
|<span data-ttu-id="47266-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47266-117">Application</span></span>|<span data-ttu-id="47266-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47266-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47266-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47266-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}
```

## <a name="request-headers"></a><span data-ttu-id="47266-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="47266-120">Request headers</span></span>
|<span data-ttu-id="47266-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47266-121">Header</span></span>|<span data-ttu-id="47266-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47266-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47266-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47266-123">Authorization</span></span>|<span data-ttu-id="47266-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47266-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47266-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47266-125">Accept</span></span>|<span data-ttu-id="47266-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47266-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47266-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="47266-127">Request body</span></span>
<span data-ttu-id="47266-128">В тексте запроса добавьте представление объекта [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47266-128">In the request body, supply a JSON representation for the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

<span data-ttu-id="47266-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md).</span><span class="sxs-lookup"><span data-stu-id="47266-129">The following table shows the properties that are required when you create the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).</span></span>

|<span data-ttu-id="47266-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="47266-130">Property</span></span>|<span data-ttu-id="47266-131">Тип</span><span class="sxs-lookup"><span data-stu-id="47266-131">Type</span></span>|<span data-ttu-id="47266-132">Описание</span><span class="sxs-lookup"><span data-stu-id="47266-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47266-133">id</span><span class="sxs-lookup"><span data-stu-id="47266-133">id</span></span>|<span data-ttu-id="47266-134">String</span><span class="sxs-lookup"><span data-stu-id="47266-134">String</span></span>|<span data-ttu-id="47266-135">Идентификатор намерения</span><span class="sxs-lookup"><span data-stu-id="47266-135">The intent ID</span></span>|
|<span data-ttu-id="47266-136">displayName</span><span class="sxs-lookup"><span data-stu-id="47266-136">displayName</span></span>|<span data-ttu-id="47266-137">Строка</span><span class="sxs-lookup"><span data-stu-id="47266-137">String</span></span>|<span data-ttu-id="47266-138">Имя пользователя для данного отображаемого имени</span><span class="sxs-lookup"><span data-stu-id="47266-138">The user given display name</span></span>|
|<span data-ttu-id="47266-139">description</span><span class="sxs-lookup"><span data-stu-id="47266-139">description</span></span>|<span data-ttu-id="47266-140">String</span><span class="sxs-lookup"><span data-stu-id="47266-140">String</span></span>|<span data-ttu-id="47266-141">Описание, заданное пользователем</span><span class="sxs-lookup"><span data-stu-id="47266-141">The user given description</span></span>|
|<span data-ttu-id="47266-142">isAssigned</span><span class="sxs-lookup"><span data-stu-id="47266-142">isAssigned</span></span>|<span data-ttu-id="47266-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="47266-143">Boolean</span></span>|<span data-ttu-id="47266-144">Указывает, назначена ли пользователю задача</span><span class="sxs-lookup"><span data-stu-id="47266-144">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="47266-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47266-145">lastModifiedDateTime</span></span>|<span data-ttu-id="47266-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47266-146">DateTimeOffset</span></span>|<span data-ttu-id="47266-147">Время последнего изменения намерения</span><span class="sxs-lookup"><span data-stu-id="47266-147">When the intent was last modified</span></span>|
|<span data-ttu-id="47266-148">templateId</span><span class="sxs-lookup"><span data-stu-id="47266-148">templateId</span></span>|<span data-ttu-id="47266-149">String</span><span class="sxs-lookup"><span data-stu-id="47266-149">String</span></span>|<span data-ttu-id="47266-150">Идентификатор шаблона, на основе которого была создана эта цель (при наличии)</span><span class="sxs-lookup"><span data-stu-id="47266-150">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="47266-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="47266-151">roleScopeTagIds</span></span>|<span data-ttu-id="47266-152">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="47266-152">String collection</span></span>|<span data-ttu-id="47266-153">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="47266-153">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="47266-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="47266-154">Response</span></span>
<span data-ttu-id="47266-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47266-155">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47266-156">Пример</span><span class="sxs-lookup"><span data-stu-id="47266-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="47266-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="47266-157">Request</span></span>
<span data-ttu-id="47266-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47266-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47266-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="47266-159">Response</span></span>
<span data-ttu-id="47266-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47266-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



