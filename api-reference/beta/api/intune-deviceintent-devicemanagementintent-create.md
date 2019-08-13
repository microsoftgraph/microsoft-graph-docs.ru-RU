---
title: Создание Девицеманажементинтент
description: Создание нового объекта Девицеманажементинтент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4e4fc01d4219140b215df6d6ebd186d99c830d1b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313316"
---
# <a name="create-devicemanagementintent"></a><span data-ttu-id="97578-103">Создание Девицеманажементинтент</span><span class="sxs-lookup"><span data-stu-id="97578-103">Create deviceManagementIntent</span></span>

> <span data-ttu-id="97578-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97578-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97578-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97578-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97578-106">Создание нового объекта [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) .</span><span class="sxs-lookup"><span data-stu-id="97578-106">Create a new [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97578-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="97578-107">Prerequisites</span></span>
<span data-ttu-id="97578-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97578-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97578-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97578-110">Permission type</span></span>|<span data-ttu-id="97578-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="97578-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97578-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97578-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97578-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97578-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97578-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97578-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97578-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97578-115">Not supported.</span></span>|
|<span data-ttu-id="97578-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97578-116">Application</span></span>|<span data-ttu-id="97578-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97578-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97578-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97578-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="97578-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97578-119">Request headers</span></span>
|<span data-ttu-id="97578-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97578-120">Header</span></span>|<span data-ttu-id="97578-121">Значение</span><span class="sxs-lookup"><span data-stu-id="97578-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97578-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97578-122">Authorization</span></span>|<span data-ttu-id="97578-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97578-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97578-124">Accept</span><span class="sxs-lookup"><span data-stu-id="97578-124">Accept</span></span>|<span data-ttu-id="97578-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97578-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97578-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="97578-126">Request body</span></span>
<span data-ttu-id="97578-127">В тексте запроса добавьте представление объекта Девицеманажементинтент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97578-127">In the request body, supply a JSON representation for the deviceManagementIntent object.</span></span>

<span data-ttu-id="97578-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтент.</span><span class="sxs-lookup"><span data-stu-id="97578-128">The following table shows the properties that are required when you create the deviceManagementIntent.</span></span>

|<span data-ttu-id="97578-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="97578-129">Property</span></span>|<span data-ttu-id="97578-130">Тип</span><span class="sxs-lookup"><span data-stu-id="97578-130">Type</span></span>|<span data-ttu-id="97578-131">Описание</span><span class="sxs-lookup"><span data-stu-id="97578-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97578-132">id</span><span class="sxs-lookup"><span data-stu-id="97578-132">id</span></span>|<span data-ttu-id="97578-133">String</span><span class="sxs-lookup"><span data-stu-id="97578-133">String</span></span>|<span data-ttu-id="97578-134">Идентификатор намерения</span><span class="sxs-lookup"><span data-stu-id="97578-134">The intent ID</span></span>|
|<span data-ttu-id="97578-135">displayName</span><span class="sxs-lookup"><span data-stu-id="97578-135">displayName</span></span>|<span data-ttu-id="97578-136">Строка</span><span class="sxs-lookup"><span data-stu-id="97578-136">String</span></span>|<span data-ttu-id="97578-137">Имя пользователя для данного отображаемого имени</span><span class="sxs-lookup"><span data-stu-id="97578-137">The user given display name</span></span>|
|<span data-ttu-id="97578-138">description</span><span class="sxs-lookup"><span data-stu-id="97578-138">description</span></span>|<span data-ttu-id="97578-139">String</span><span class="sxs-lookup"><span data-stu-id="97578-139">String</span></span>|<span data-ttu-id="97578-140">Описание, заданное пользователем</span><span class="sxs-lookup"><span data-stu-id="97578-140">The user given description</span></span>|
|<span data-ttu-id="97578-141">isAssigned</span><span class="sxs-lookup"><span data-stu-id="97578-141">isAssigned</span></span>|<span data-ttu-id="97578-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="97578-142">Boolean</span></span>|<span data-ttu-id="97578-143">Указывает, назначена ли пользователю задача</span><span class="sxs-lookup"><span data-stu-id="97578-143">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="97578-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97578-144">lastModifiedDateTime</span></span>|<span data-ttu-id="97578-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97578-145">DateTimeOffset</span></span>|<span data-ttu-id="97578-146">Время последнего изменения намерения</span><span class="sxs-lookup"><span data-stu-id="97578-146">When the intent was last modified</span></span>|
|<span data-ttu-id="97578-147">templateId</span><span class="sxs-lookup"><span data-stu-id="97578-147">templateId</span></span>|<span data-ttu-id="97578-148">String</span><span class="sxs-lookup"><span data-stu-id="97578-148">String</span></span>|<span data-ttu-id="97578-149">Идентификатор шаблона, на основе которого была создана эта цель (при наличии)</span><span class="sxs-lookup"><span data-stu-id="97578-149">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="97578-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="97578-150">roleScopeTagIds</span></span>|<span data-ttu-id="97578-151">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="97578-151">String collection</span></span>|<span data-ttu-id="97578-152">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="97578-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="97578-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="97578-153">Response</span></span>
<span data-ttu-id="97578-154">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97578-154">If successful, this method returns a `201 Created` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97578-155">Пример</span><span class="sxs-lookup"><span data-stu-id="97578-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="97578-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="97578-156">Request</span></span>
<span data-ttu-id="97578-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97578-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents
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

### <a name="response"></a><span data-ttu-id="97578-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="97578-158">Response</span></span>
<span data-ttu-id="97578-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97578-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






