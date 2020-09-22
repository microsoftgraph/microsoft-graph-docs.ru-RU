---
title: Обновление Девицеандаппманажементассигнментфилтер
description: Обновление свойств объекта Девицеандаппманажементассигнментфилтер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff69e8d1675e9909052e286951ee2fedc5f0b4c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999876"
---
# <a name="update-deviceandappmanagementassignmentfilter"></a><span data-ttu-id="085cf-103">Обновление Девицеандаппманажементассигнментфилтер</span><span class="sxs-lookup"><span data-stu-id="085cf-103">Update deviceAndAppManagementAssignmentFilter</span></span>

<span data-ttu-id="085cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="085cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="085cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="085cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="085cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="085cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="085cf-107">Обновление свойств объекта [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) .</span><span class="sxs-lookup"><span data-stu-id="085cf-107">Update the properties of a [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="085cf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="085cf-108">Prerequisites</span></span>
<span data-ttu-id="085cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="085cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="085cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="085cf-111">Permission type</span></span>|<span data-ttu-id="085cf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="085cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="085cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="085cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="085cf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="085cf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="085cf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="085cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="085cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="085cf-116">Not supported.</span></span>|
|<span data-ttu-id="085cf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="085cf-117">Application</span></span>|<span data-ttu-id="085cf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="085cf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="085cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="085cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

## <a name="request-headers"></a><span data-ttu-id="085cf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="085cf-120">Request headers</span></span>
|<span data-ttu-id="085cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="085cf-121">Header</span></span>|<span data-ttu-id="085cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="085cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="085cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="085cf-123">Authorization</span></span>|<span data-ttu-id="085cf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="085cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="085cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="085cf-125">Accept</span></span>|<span data-ttu-id="085cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="085cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="085cf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="085cf-127">Request body</span></span>
<span data-ttu-id="085cf-128">В тексте запроса добавьте представление объекта [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="085cf-128">In the request body, supply a JSON representation for the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

<span data-ttu-id="085cf-129">В следующей таблице приведены свойства, необходимые при создании [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span><span class="sxs-lookup"><span data-stu-id="085cf-129">The following table shows the properties that are required when you create the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span></span>

|<span data-ttu-id="085cf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="085cf-130">Property</span></span>|<span data-ttu-id="085cf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="085cf-131">Type</span></span>|<span data-ttu-id="085cf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="085cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="085cf-133">id</span><span class="sxs-lookup"><span data-stu-id="085cf-133">id</span></span>|<span data-ttu-id="085cf-134">String</span><span class="sxs-lookup"><span data-stu-id="085cf-134">String</span></span>|<span data-ttu-id="085cf-135">Ключ фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="085cf-135">Key of the Assignment Filter.</span></span>|
|<span data-ttu-id="085cf-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="085cf-136">createdDateTime</span></span>|<span data-ttu-id="085cf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="085cf-137">DateTimeOffset</span></span>|<span data-ttu-id="085cf-138">Время создания фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="085cf-138">Creation time of the Assignment Filter.</span></span>|
|<span data-ttu-id="085cf-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="085cf-139">lastModifiedDateTime</span></span>|<span data-ttu-id="085cf-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="085cf-140">DateTimeOffset</span></span>|<span data-ttu-id="085cf-141">Время последнего изменения фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="085cf-141">Last modified time of the Assignment Filter.</span></span>|
|<span data-ttu-id="085cf-142">displayName</span><span class="sxs-lookup"><span data-stu-id="085cf-142">displayName</span></span>|<span data-ttu-id="085cf-143">String</span><span class="sxs-lookup"><span data-stu-id="085cf-143">String</span></span>|<span data-ttu-id="085cf-144">DisplayName фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="085cf-144">DisplayName of the Assignment Filter.</span></span>|
|<span data-ttu-id="085cf-145">description</span><span class="sxs-lookup"><span data-stu-id="085cf-145">description</span></span>|<span data-ttu-id="085cf-146">String</span><span class="sxs-lookup"><span data-stu-id="085cf-146">String</span></span>|<span data-ttu-id="085cf-147">Описание фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="085cf-147">Description of the Assignment Filter.</span></span>|
|<span data-ttu-id="085cf-148">платформа</span><span class="sxs-lookup"><span data-stu-id="085cf-148">platform</span></span>|[<span data-ttu-id="085cf-149">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="085cf-149">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="085cf-150">Тип платформы устройств, к которым будет применяться фильтр назначений.</span><span class="sxs-lookup"><span data-stu-id="085cf-150">Platform type of the devices on which the Assignment Filter will be applicable.</span></span> <span data-ttu-id="085cf-151">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="085cf-151">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="085cf-152">правила</span><span class="sxs-lookup"><span data-stu-id="085cf-152">rule</span></span>|<span data-ttu-id="085cf-153">String</span><span class="sxs-lookup"><span data-stu-id="085cf-153">String</span></span>|<span data-ttu-id="085cf-154">Определение правила для фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="085cf-154">Rule definition of the Assignment Filter.</span></span>|
|<span data-ttu-id="085cf-155">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="085cf-155">roleScopeTags</span></span>|<span data-ttu-id="085cf-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="085cf-156">String collection</span></span>|<span data-ttu-id="085cf-157">RoleScopeTags фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="085cf-157">RoleScopeTags of the Assignment Filter.</span></span>|



## <a name="response"></a><span data-ttu-id="085cf-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="085cf-158">Response</span></span>
<span data-ttu-id="085cf-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="085cf-159">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="085cf-160">Пример</span><span class="sxs-lookup"><span data-stu-id="085cf-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="085cf-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="085cf-161">Request</span></span>
<span data-ttu-id="085cf-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="085cf-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
Content-type: application/json
Content-length: 274

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="085cf-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="085cf-163">Response</span></span>
<span data-ttu-id="085cf-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="085cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 446

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "id": "819818db-18db-8198-db18-9881db189881",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```






