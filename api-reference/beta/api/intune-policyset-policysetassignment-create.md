---
title: Создание Полицисетассигнмент
description: Создание нового объекта Полицисетассигнмент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6b0958d319e4423e72eb9476094ff582ed1595be
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802106"
---
# <a name="create-policysetassignment"></a><span data-ttu-id="bf3bb-103">Создание Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="bf3bb-103">Create policySetAssignment</span></span>

> <span data-ttu-id="bf3bb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf3bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf3bb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf3bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf3bb-106">Создание нового объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="bf3bb-106">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf3bb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bf3bb-107">Prerequisites</span></span>
<span data-ttu-id="bf3bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf3bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf3bb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf3bb-110">Permission type</span></span>|<span data-ttu-id="bf3bb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf3bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf3bb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf3bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf3bb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf3bb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf3bb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf3bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf3bb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf3bb-115">Not supported.</span></span>|
|<span data-ttu-id="bf3bb-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bf3bb-116">Application</span></span>|<span data-ttu-id="bf3bb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf3bb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf3bb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf3bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="bf3bb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bf3bb-119">Request headers</span></span>
|<span data-ttu-id="bf3bb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf3bb-120">Header</span></span>|<span data-ttu-id="bf3bb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bf3bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf3bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf3bb-122">Authorization</span></span>|<span data-ttu-id="bf3bb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf3bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf3bb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bf3bb-124">Accept</span></span>|<span data-ttu-id="bf3bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf3bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf3bb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf3bb-126">Request body</span></span>
<span data-ttu-id="bf3bb-127">В тексте запроса добавьте представление объекта Полицисетассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf3bb-127">In the request body, supply a JSON representation for the policySetAssignment object.</span></span>

<span data-ttu-id="bf3bb-128">В следующей таблице приведены свойства, необходимые при создании Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="bf3bb-128">The following table shows the properties that are required when you create the policySetAssignment.</span></span>

|<span data-ttu-id="bf3bb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf3bb-129">Property</span></span>|<span data-ttu-id="bf3bb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bf3bb-130">Type</span></span>|<span data-ttu-id="bf3bb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bf3bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf3bb-132">id</span><span class="sxs-lookup"><span data-stu-id="bf3bb-132">id</span></span>|<span data-ttu-id="bf3bb-133">String</span><span class="sxs-lookup"><span data-stu-id="bf3bb-133">String</span></span>|<span data-ttu-id="bf3bb-134">Ключ Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="bf3bb-134">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="bf3bb-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf3bb-135">lastModifiedDateTime</span></span>|<span data-ttu-id="bf3bb-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf3bb-136">DateTimeOffset</span></span>|<span data-ttu-id="bf3bb-137">Время последнего изменения Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="bf3bb-137">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="bf3bb-138">target</span><span class="sxs-lookup"><span data-stu-id="bf3bb-138">target</span></span>|[<span data-ttu-id="bf3bb-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bf3bb-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bf3bb-140">Целевая группа Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="bf3bb-140">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="bf3bb-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf3bb-141">Response</span></span>
<span data-ttu-id="bf3bb-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf3bb-142">If successful, this method returns a `201 Created` response code and a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf3bb-143">Пример</span><span class="sxs-lookup"><span data-stu-id="bf3bb-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf3bb-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf3bb-144">Request</span></span>
<span data-ttu-id="bf3bb-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf3bb-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="bf3bb-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf3bb-146">Response</span></span>
<span data-ttu-id="bf3bb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf3bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




