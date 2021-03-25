---
title: Обновление устройстваAndAppManagementAssignmentFilter
description: Обновление свойств объекта deviceAndAppManagementAssignmentFilter.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa80ffa96fcd558ec7c89363406737ca538b6733
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158642"
---
# <a name="update-deviceandappmanagementassignmentfilter"></a><span data-ttu-id="6c281-103">Обновление устройстваAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="6c281-103">Update deviceAndAppManagementAssignmentFilter</span></span>

<span data-ttu-id="6c281-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c281-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c281-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c281-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c281-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c281-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c281-107">Обновление свойств объекта [deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)</span><span class="sxs-lookup"><span data-stu-id="6c281-107">Update the properties of a [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c281-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6c281-108">Prerequisites</span></span>
<span data-ttu-id="6c281-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c281-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c281-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c281-111">Permission type</span></span>|<span data-ttu-id="6c281-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c281-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c281-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c281-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c281-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c281-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c281-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c281-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c281-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c281-116">Not supported.</span></span>|
|<span data-ttu-id="6c281-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6c281-117">Application</span></span>|<span data-ttu-id="6c281-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c281-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c281-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c281-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

## <a name="request-headers"></a><span data-ttu-id="6c281-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6c281-120">Request headers</span></span>
|<span data-ttu-id="6c281-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c281-121">Header</span></span>|<span data-ttu-id="6c281-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6c281-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c281-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c281-123">Authorization</span></span>|<span data-ttu-id="6c281-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c281-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c281-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6c281-125">Accept</span></span>|<span data-ttu-id="6c281-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c281-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c281-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c281-127">Request body</span></span>
<span data-ttu-id="6c281-128">В теле запроса поставляем представление JSON для [объекта deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)</span><span class="sxs-lookup"><span data-stu-id="6c281-128">In the request body, supply a JSON representation for the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

<span data-ttu-id="6c281-129">В следующей таблице показаны свойства, необходимые при создании [устройстваAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)</span><span class="sxs-lookup"><span data-stu-id="6c281-129">The following table shows the properties that are required when you create the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span></span>

|<span data-ttu-id="6c281-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c281-130">Property</span></span>|<span data-ttu-id="6c281-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6c281-131">Type</span></span>|<span data-ttu-id="6c281-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6c281-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c281-133">id</span><span class="sxs-lookup"><span data-stu-id="6c281-133">id</span></span>|<span data-ttu-id="6c281-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6c281-134">String</span></span>|<span data-ttu-id="6c281-135">Ключ фильтра назначения.</span><span class="sxs-lookup"><span data-stu-id="6c281-135">Key of the Assignment Filter.</span></span>|
|<span data-ttu-id="6c281-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c281-136">createdDateTime</span></span>|<span data-ttu-id="6c281-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c281-137">DateTimeOffset</span></span>|<span data-ttu-id="6c281-138">Время создания фильтра назначения.</span><span class="sxs-lookup"><span data-stu-id="6c281-138">Creation time of the Assignment Filter.</span></span>|
|<span data-ttu-id="6c281-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c281-139">lastModifiedDateTime</span></span>|<span data-ttu-id="6c281-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c281-140">DateTimeOffset</span></span>|<span data-ttu-id="6c281-141">Последнее измененное время фильтра назначения.</span><span class="sxs-lookup"><span data-stu-id="6c281-141">Last modified time of the Assignment Filter.</span></span>|
|<span data-ttu-id="6c281-142">displayName</span><span class="sxs-lookup"><span data-stu-id="6c281-142">displayName</span></span>|<span data-ttu-id="6c281-143">Строка</span><span class="sxs-lookup"><span data-stu-id="6c281-143">String</span></span>|<span data-ttu-id="6c281-144">DisplayName фильтра назначения.</span><span class="sxs-lookup"><span data-stu-id="6c281-144">DisplayName of the Assignment Filter.</span></span>|
|<span data-ttu-id="6c281-145">description</span><span class="sxs-lookup"><span data-stu-id="6c281-145">description</span></span>|<span data-ttu-id="6c281-146">Строка</span><span class="sxs-lookup"><span data-stu-id="6c281-146">String</span></span>|<span data-ttu-id="6c281-147">Описание фильтра назначения.</span><span class="sxs-lookup"><span data-stu-id="6c281-147">Description of the Assignment Filter.</span></span>|
|<span data-ttu-id="6c281-148">платформа</span><span class="sxs-lookup"><span data-stu-id="6c281-148">platform</span></span>|[<span data-ttu-id="6c281-149">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="6c281-149">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="6c281-150">Тип платформы устройств, на которых будет применяться фильтр назначения.</span><span class="sxs-lookup"><span data-stu-id="6c281-150">Platform type of the devices on which the Assignment Filter will be applicable.</span></span> <span data-ttu-id="6c281-151">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="6c281-151">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="6c281-152">правило</span><span class="sxs-lookup"><span data-stu-id="6c281-152">rule</span></span>|<span data-ttu-id="6c281-153">Строка</span><span class="sxs-lookup"><span data-stu-id="6c281-153">String</span></span>|<span data-ttu-id="6c281-154">Определение правила фильтра назначения.</span><span class="sxs-lookup"><span data-stu-id="6c281-154">Rule definition of the Assignment Filter.</span></span>|
|<span data-ttu-id="6c281-155">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="6c281-155">roleScopeTags</span></span>|<span data-ttu-id="6c281-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6c281-156">String collection</span></span>|<span data-ttu-id="6c281-157">RoleScopeTags фильтра назначения.</span><span class="sxs-lookup"><span data-stu-id="6c281-157">RoleScopeTags of the Assignment Filter.</span></span>|



## <a name="response"></a><span data-ttu-id="6c281-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c281-158">Response</span></span>
<span data-ttu-id="6c281-159">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6c281-159">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c281-160">Пример</span><span class="sxs-lookup"><span data-stu-id="6c281-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c281-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c281-161">Request</span></span>
<span data-ttu-id="6c281-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c281-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6c281-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c281-163">Response</span></span>
<span data-ttu-id="6c281-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c281-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




