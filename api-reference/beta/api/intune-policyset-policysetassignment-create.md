---
title: Создание Полицисетассигнмент
description: Создание нового объекта Полицисетассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 103737f4b8b2e4c17a5c6683ffbb165d051ddcde
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706515"
---
# <a name="create-policysetassignment"></a><span data-ttu-id="5afdc-103">Создание Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="5afdc-103">Create policySetAssignment</span></span>

<span data-ttu-id="5afdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5afdc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5afdc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5afdc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5afdc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5afdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5afdc-107">Создание нового объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5afdc-107">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5afdc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5afdc-108">Prerequisites</span></span>
<span data-ttu-id="5afdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5afdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5afdc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5afdc-111">Permission type</span></span>|<span data-ttu-id="5afdc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5afdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5afdc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5afdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5afdc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5afdc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5afdc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5afdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5afdc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5afdc-116">Not supported.</span></span>|
|<span data-ttu-id="5afdc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5afdc-117">Application</span></span>|<span data-ttu-id="5afdc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5afdc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5afdc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5afdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="5afdc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5afdc-120">Request headers</span></span>
|<span data-ttu-id="5afdc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5afdc-121">Header</span></span>|<span data-ttu-id="5afdc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5afdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5afdc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5afdc-123">Authorization</span></span>|<span data-ttu-id="5afdc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5afdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5afdc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5afdc-125">Accept</span></span>|<span data-ttu-id="5afdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5afdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5afdc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5afdc-127">Request body</span></span>
<span data-ttu-id="5afdc-128">В тексте запроса добавьте представление объекта Полицисетассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5afdc-128">In the request body, supply a JSON representation for the policySetAssignment object.</span></span>

<span data-ttu-id="5afdc-129">В следующей таблице приведены свойства, необходимые при создании Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="5afdc-129">The following table shows the properties that are required when you create the policySetAssignment.</span></span>

|<span data-ttu-id="5afdc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5afdc-130">Property</span></span>|<span data-ttu-id="5afdc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5afdc-131">Type</span></span>|<span data-ttu-id="5afdc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5afdc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5afdc-133">id</span><span class="sxs-lookup"><span data-stu-id="5afdc-133">id</span></span>|<span data-ttu-id="5afdc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5afdc-134">String</span></span>|<span data-ttu-id="5afdc-135">Ключ Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="5afdc-135">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="5afdc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5afdc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5afdc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5afdc-137">DateTimeOffset</span></span>|<span data-ttu-id="5afdc-138">Время последнего изменения Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="5afdc-138">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="5afdc-139">target</span><span class="sxs-lookup"><span data-stu-id="5afdc-139">target</span></span>|[<span data-ttu-id="5afdc-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5afdc-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5afdc-141">Целевая группа Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="5afdc-141">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="5afdc-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="5afdc-142">Response</span></span>
<span data-ttu-id="5afdc-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5afdc-143">If successful, this method returns a `201 Created` response code and a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5afdc-144">Пример</span><span class="sxs-lookup"><span data-stu-id="5afdc-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="5afdc-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="5afdc-145">Request</span></span>
<span data-ttu-id="5afdc-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5afdc-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="5afdc-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="5afdc-147">Response</span></span>
<span data-ttu-id="5afdc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5afdc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 427

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```





