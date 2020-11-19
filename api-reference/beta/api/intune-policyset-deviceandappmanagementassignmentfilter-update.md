---
title: Обновление Девицеандаппманажементассигнментфилтер
description: Обновление свойств объекта Девицеандаппманажементассигнментфилтер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 396fc74e9ba44610810a4c260b33aebe334219c5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49227121"
---
# <a name="update-deviceandappmanagementassignmentfilter"></a><span data-ttu-id="b30f4-103">Обновление Девицеандаппманажементассигнментфилтер</span><span class="sxs-lookup"><span data-stu-id="b30f4-103">Update deviceAndAppManagementAssignmentFilter</span></span>

<span data-ttu-id="b30f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b30f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b30f4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b30f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b30f4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b30f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b30f4-107">Обновление свойств объекта [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) .</span><span class="sxs-lookup"><span data-stu-id="b30f4-107">Update the properties of a [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b30f4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b30f4-108">Prerequisites</span></span>
<span data-ttu-id="b30f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b30f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b30f4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b30f4-111">Permission type</span></span>|<span data-ttu-id="b30f4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b30f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b30f4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b30f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b30f4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b30f4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b30f4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b30f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b30f4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b30f4-116">Not supported.</span></span>|
|<span data-ttu-id="b30f4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b30f4-117">Application</span></span>|<span data-ttu-id="b30f4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b30f4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b30f4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b30f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

## <a name="request-headers"></a><span data-ttu-id="b30f4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b30f4-120">Request headers</span></span>
|<span data-ttu-id="b30f4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b30f4-121">Header</span></span>|<span data-ttu-id="b30f4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b30f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b30f4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b30f4-123">Authorization</span></span>|<span data-ttu-id="b30f4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b30f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b30f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b30f4-125">Accept</span></span>|<span data-ttu-id="b30f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b30f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b30f4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b30f4-127">Request body</span></span>
<span data-ttu-id="b30f4-128">В тексте запроса добавьте представление объекта [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b30f4-128">In the request body, supply a JSON representation for the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

<span data-ttu-id="b30f4-129">В следующей таблице приведены свойства, необходимые при создании [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span><span class="sxs-lookup"><span data-stu-id="b30f4-129">The following table shows the properties that are required when you create the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span></span>

|<span data-ttu-id="b30f4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b30f4-130">Property</span></span>|<span data-ttu-id="b30f4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b30f4-131">Type</span></span>|<span data-ttu-id="b30f4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b30f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b30f4-133">id</span><span class="sxs-lookup"><span data-stu-id="b30f4-133">id</span></span>|<span data-ttu-id="b30f4-134">String</span><span class="sxs-lookup"><span data-stu-id="b30f4-134">String</span></span>|<span data-ttu-id="b30f4-135">Ключ фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="b30f4-135">Key of the Assignment Filter.</span></span>|
|<span data-ttu-id="b30f4-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b30f4-136">createdDateTime</span></span>|<span data-ttu-id="b30f4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b30f4-137">DateTimeOffset</span></span>|<span data-ttu-id="b30f4-138">Время создания фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="b30f4-138">Creation time of the Assignment Filter.</span></span>|
|<span data-ttu-id="b30f4-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b30f4-139">lastModifiedDateTime</span></span>|<span data-ttu-id="b30f4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b30f4-140">DateTimeOffset</span></span>|<span data-ttu-id="b30f4-141">Время последнего изменения фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="b30f4-141">Last modified time of the Assignment Filter.</span></span>|
|<span data-ttu-id="b30f4-142">displayName</span><span class="sxs-lookup"><span data-stu-id="b30f4-142">displayName</span></span>|<span data-ttu-id="b30f4-143">String</span><span class="sxs-lookup"><span data-stu-id="b30f4-143">String</span></span>|<span data-ttu-id="b30f4-144">DisplayName фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="b30f4-144">DisplayName of the Assignment Filter.</span></span>|
|<span data-ttu-id="b30f4-145">description</span><span class="sxs-lookup"><span data-stu-id="b30f4-145">description</span></span>|<span data-ttu-id="b30f4-146">String</span><span class="sxs-lookup"><span data-stu-id="b30f4-146">String</span></span>|<span data-ttu-id="b30f4-147">Описание фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="b30f4-147">Description of the Assignment Filter.</span></span>|
|<span data-ttu-id="b30f4-148">платформа</span><span class="sxs-lookup"><span data-stu-id="b30f4-148">platform</span></span>|[<span data-ttu-id="b30f4-149">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="b30f4-149">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="b30f4-150">Тип платформы устройств, к которым будет применяться фильтр назначений.</span><span class="sxs-lookup"><span data-stu-id="b30f4-150">Platform type of the devices on which the Assignment Filter will be applicable.</span></span> <span data-ttu-id="b30f4-151">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b30f4-151">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="b30f4-152">правила</span><span class="sxs-lookup"><span data-stu-id="b30f4-152">rule</span></span>|<span data-ttu-id="b30f4-153">String</span><span class="sxs-lookup"><span data-stu-id="b30f4-153">String</span></span>|<span data-ttu-id="b30f4-154">Определение правила для фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="b30f4-154">Rule definition of the Assignment Filter.</span></span>|
|<span data-ttu-id="b30f4-155">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="b30f4-155">roleScopeTags</span></span>|<span data-ttu-id="b30f4-156">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b30f4-156">String collection</span></span>|<span data-ttu-id="b30f4-157">RoleScopeTags фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="b30f4-157">RoleScopeTags of the Assignment Filter.</span></span>|



## <a name="response"></a><span data-ttu-id="b30f4-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="b30f4-158">Response</span></span>
<span data-ttu-id="b30f4-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b30f4-159">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b30f4-160">Пример</span><span class="sxs-lookup"><span data-stu-id="b30f4-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="b30f4-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="b30f4-161">Request</span></span>
<span data-ttu-id="b30f4-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b30f4-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b30f4-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="b30f4-163">Response</span></span>
<span data-ttu-id="b30f4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b30f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




