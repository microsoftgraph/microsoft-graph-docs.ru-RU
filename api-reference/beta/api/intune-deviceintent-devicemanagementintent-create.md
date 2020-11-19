---
title: Создание Девицеманажементинтент
description: Создание нового объекта Девицеманажементинтент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cde7ad8536edbcab146a5d93e1a94624491c3b3f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49278277"
---
# <a name="create-devicemanagementintent"></a><span data-ttu-id="f5e81-103">Создание Девицеманажементинтент</span><span class="sxs-lookup"><span data-stu-id="f5e81-103">Create deviceManagementIntent</span></span>

<span data-ttu-id="f5e81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5e81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5e81-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5e81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5e81-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5e81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5e81-107">Создание нового объекта [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) .</span><span class="sxs-lookup"><span data-stu-id="f5e81-107">Create a new [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5e81-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f5e81-108">Prerequisites</span></span>
<span data-ttu-id="f5e81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5e81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5e81-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5e81-111">Permission type</span></span>|<span data-ttu-id="f5e81-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5e81-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5e81-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5e81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5e81-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5e81-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5e81-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5e81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5e81-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5e81-116">Not supported.</span></span>|
|<span data-ttu-id="f5e81-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5e81-117">Application</span></span>|<span data-ttu-id="f5e81-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5e81-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5e81-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5e81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="f5e81-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f5e81-120">Request headers</span></span>
|<span data-ttu-id="f5e81-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f5e81-121">Header</span></span>|<span data-ttu-id="f5e81-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f5e81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5e81-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5e81-123">Authorization</span></span>|<span data-ttu-id="f5e81-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5e81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5e81-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f5e81-125">Accept</span></span>|<span data-ttu-id="f5e81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5e81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5e81-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5e81-127">Request body</span></span>
<span data-ttu-id="f5e81-128">В тексте запроса добавьте представление объекта Девицеманажементинтент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5e81-128">In the request body, supply a JSON representation for the deviceManagementIntent object.</span></span>

<span data-ttu-id="f5e81-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтент.</span><span class="sxs-lookup"><span data-stu-id="f5e81-129">The following table shows the properties that are required when you create the deviceManagementIntent.</span></span>

|<span data-ttu-id="f5e81-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5e81-130">Property</span></span>|<span data-ttu-id="f5e81-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f5e81-131">Type</span></span>|<span data-ttu-id="f5e81-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f5e81-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5e81-133">id</span><span class="sxs-lookup"><span data-stu-id="f5e81-133">id</span></span>|<span data-ttu-id="f5e81-134">String</span><span class="sxs-lookup"><span data-stu-id="f5e81-134">String</span></span>|<span data-ttu-id="f5e81-135">Идентификатор намерения</span><span class="sxs-lookup"><span data-stu-id="f5e81-135">The intent ID</span></span>|
|<span data-ttu-id="f5e81-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f5e81-136">displayName</span></span>|<span data-ttu-id="f5e81-137">String</span><span class="sxs-lookup"><span data-stu-id="f5e81-137">String</span></span>|<span data-ttu-id="f5e81-138">Имя пользователя для данного отображаемого имени</span><span class="sxs-lookup"><span data-stu-id="f5e81-138">The user given display name</span></span>|
|<span data-ttu-id="f5e81-139">description</span><span class="sxs-lookup"><span data-stu-id="f5e81-139">description</span></span>|<span data-ttu-id="f5e81-140">String</span><span class="sxs-lookup"><span data-stu-id="f5e81-140">String</span></span>|<span data-ttu-id="f5e81-141">Описание, заданное пользователем</span><span class="sxs-lookup"><span data-stu-id="f5e81-141">The user given description</span></span>|
|<span data-ttu-id="f5e81-142">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f5e81-142">isAssigned</span></span>|<span data-ttu-id="f5e81-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5e81-143">Boolean</span></span>|<span data-ttu-id="f5e81-144">Указывает, назначена ли пользователю задача</span><span class="sxs-lookup"><span data-stu-id="f5e81-144">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="f5e81-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5e81-145">lastModifiedDateTime</span></span>|<span data-ttu-id="f5e81-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5e81-146">DateTimeOffset</span></span>|<span data-ttu-id="f5e81-147">Время последнего изменения намерения</span><span class="sxs-lookup"><span data-stu-id="f5e81-147">When the intent was last modified</span></span>|
|<span data-ttu-id="f5e81-148">templateId</span><span class="sxs-lookup"><span data-stu-id="f5e81-148">templateId</span></span>|<span data-ttu-id="f5e81-149">String</span><span class="sxs-lookup"><span data-stu-id="f5e81-149">String</span></span>|<span data-ttu-id="f5e81-150">Идентификатор шаблона, на основе которого была создана эта цель (при наличии)</span><span class="sxs-lookup"><span data-stu-id="f5e81-150">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="f5e81-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f5e81-151">roleScopeTagIds</span></span>|<span data-ttu-id="f5e81-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f5e81-152">String collection</span></span>|<span data-ttu-id="f5e81-153">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f5e81-153">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="f5e81-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5e81-154">Response</span></span>
<span data-ttu-id="f5e81-155">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f5e81-155">If successful, this method returns a `201 Created` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5e81-156">Пример</span><span class="sxs-lookup"><span data-stu-id="f5e81-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5e81-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5e81-157">Request</span></span>
<span data-ttu-id="f5e81-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5e81-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f5e81-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5e81-159">Response</span></span>
<span data-ttu-id="f5e81-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f5e81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




