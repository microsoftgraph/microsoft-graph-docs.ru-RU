---
title: Обновление Девицеандаппманажементассигнментфилтер
description: Обновление свойств объекта Девицеандаппманажементассигнментфилтер.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5fd7242879c9a086b08895637ad811b5fd48160
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791730"
---
# <a name="update-deviceandappmanagementassignmentfilter"></a><span data-ttu-id="a64a1-103">Обновление Девицеандаппманажементассигнментфилтер</span><span class="sxs-lookup"><span data-stu-id="a64a1-103">Update deviceAndAppManagementAssignmentFilter</span></span>

<span data-ttu-id="a64a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a64a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a64a1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a64a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a64a1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a64a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a64a1-107">Обновление свойств объекта [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) .</span><span class="sxs-lookup"><span data-stu-id="a64a1-107">Update the properties of a [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a64a1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a64a1-108">Prerequisites</span></span>
<span data-ttu-id="a64a1-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a64a1-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a64a1-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a64a1-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a64a1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a64a1-111">Permission type</span></span>|<span data-ttu-id="a64a1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a64a1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a64a1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a64a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a64a1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a64a1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a64a1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a64a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a64a1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a64a1-116">Not supported.</span></span>|
|<span data-ttu-id="a64a1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a64a1-117">Application</span></span>|<span data-ttu-id="a64a1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a64a1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a64a1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a64a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

## <a name="request-headers"></a><span data-ttu-id="a64a1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a64a1-120">Request headers</span></span>
|<span data-ttu-id="a64a1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a64a1-121">Header</span></span>|<span data-ttu-id="a64a1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a64a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a64a1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a64a1-123">Authorization</span></span>|<span data-ttu-id="a64a1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a64a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a64a1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a64a1-125">Accept</span></span>|<span data-ttu-id="a64a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a64a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a64a1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a64a1-127">Request body</span></span>
<span data-ttu-id="a64a1-128">В тексте запроса добавьте представление объекта [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a64a1-128">In the request body, supply a JSON representation for the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

<span data-ttu-id="a64a1-129">В следующей таблице приведены свойства, необходимые при создании [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span><span class="sxs-lookup"><span data-stu-id="a64a1-129">The following table shows the properties that are required when you create the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span></span>

|<span data-ttu-id="a64a1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a64a1-130">Property</span></span>|<span data-ttu-id="a64a1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a64a1-131">Type</span></span>|<span data-ttu-id="a64a1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a64a1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a64a1-133">id</span><span class="sxs-lookup"><span data-stu-id="a64a1-133">id</span></span>|<span data-ttu-id="a64a1-134">String</span><span class="sxs-lookup"><span data-stu-id="a64a1-134">String</span></span>|<span data-ttu-id="a64a1-135">Ключ фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="a64a1-135">Key of the Assignment Filter.</span></span>|
|<span data-ttu-id="a64a1-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a64a1-136">createdDateTime</span></span>|<span data-ttu-id="a64a1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a64a1-137">DateTimeOffset</span></span>|<span data-ttu-id="a64a1-138">Время создания фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="a64a1-138">Creation time of the Assignment Filter.</span></span>|
|<span data-ttu-id="a64a1-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a64a1-139">lastModifiedDateTime</span></span>|<span data-ttu-id="a64a1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a64a1-140">DateTimeOffset</span></span>|<span data-ttu-id="a64a1-141">Время последнего изменения фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="a64a1-141">Last modified time of the Assignment Filter.</span></span>|
|<span data-ttu-id="a64a1-142">displayName</span><span class="sxs-lookup"><span data-stu-id="a64a1-142">displayName</span></span>|<span data-ttu-id="a64a1-143">Строка</span><span class="sxs-lookup"><span data-stu-id="a64a1-143">String</span></span>|<span data-ttu-id="a64a1-144">DisplayName фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="a64a1-144">DisplayName of the Assignment Filter.</span></span>|
|<span data-ttu-id="a64a1-145">description</span><span class="sxs-lookup"><span data-stu-id="a64a1-145">description</span></span>|<span data-ttu-id="a64a1-146">String</span><span class="sxs-lookup"><span data-stu-id="a64a1-146">String</span></span>|<span data-ttu-id="a64a1-147">Описание фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="a64a1-147">Description of the Assignment Filter.</span></span>|
|<span data-ttu-id="a64a1-148">platform</span><span class="sxs-lookup"><span data-stu-id="a64a1-148">platform</span></span>|[<span data-ttu-id="a64a1-149">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="a64a1-149">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="a64a1-150">Тип платформы устройств, к которым будет применяться фильтр назначений.</span><span class="sxs-lookup"><span data-stu-id="a64a1-150">Platform type of the devices on which the Assignment Filter will be applicable.</span></span> <span data-ttu-id="a64a1-151">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a64a1-151">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="a64a1-152">правила</span><span class="sxs-lookup"><span data-stu-id="a64a1-152">rule</span></span>|<span data-ttu-id="a64a1-153">String</span><span class="sxs-lookup"><span data-stu-id="a64a1-153">String</span></span>|<span data-ttu-id="a64a1-154">Определение правила для фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="a64a1-154">Rule definition of the Assignment Filter.</span></span>|
|<span data-ttu-id="a64a1-155">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="a64a1-155">roleScopeTags</span></span>|<span data-ttu-id="a64a1-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a64a1-156">String collection</span></span>|<span data-ttu-id="a64a1-157">RoleScopeTags фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="a64a1-157">RoleScopeTags of the Assignment Filter.</span></span>|



## <a name="response"></a><span data-ttu-id="a64a1-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="a64a1-158">Response</span></span>
<span data-ttu-id="a64a1-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a64a1-159">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a64a1-160">Пример</span><span class="sxs-lookup"><span data-stu-id="a64a1-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="a64a1-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="a64a1-161">Request</span></span>
<span data-ttu-id="a64a1-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a64a1-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a64a1-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="a64a1-163">Response</span></span>
<span data-ttu-id="a64a1-164">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="a64a1-164">Here is an example of the response.</span></span> <span data-ttu-id="a64a1-165">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="a64a1-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a64a1-166">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a64a1-166">All of the properties will be returned from an actual call.</span></span>
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



