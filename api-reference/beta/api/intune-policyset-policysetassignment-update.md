---
title: Обновление Полицисетассигнмент
description: Обновление свойств объекта Полицисетассигнмент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 70f679df2c85caecf9286952bfadb6ddbf6f1c17
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802078"
---
# <a name="update-policysetassignment"></a><span data-ttu-id="44623-103">Обновление Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="44623-103">Update policySetAssignment</span></span>

> <span data-ttu-id="44623-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44623-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44623-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44623-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44623-106">Обновление свойств объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="44623-106">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44623-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="44623-107">Prerequisites</span></span>
<span data-ttu-id="44623-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44623-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44623-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44623-110">Permission type</span></span>|<span data-ttu-id="44623-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44623-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44623-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44623-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44623-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44623-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44623-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44623-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44623-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44623-115">Not supported.</span></span>|
|<span data-ttu-id="44623-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="44623-116">Application</span></span>|<span data-ttu-id="44623-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44623-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44623-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44623-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="44623-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="44623-119">Request headers</span></span>
|<span data-ttu-id="44623-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44623-120">Header</span></span>|<span data-ttu-id="44623-121">Значение</span><span class="sxs-lookup"><span data-stu-id="44623-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44623-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="44623-122">Authorization</span></span>|<span data-ttu-id="44623-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44623-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44623-124">Accept</span><span class="sxs-lookup"><span data-stu-id="44623-124">Accept</span></span>|<span data-ttu-id="44623-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44623-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44623-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44623-126">Request body</span></span>
<span data-ttu-id="44623-127">В тексте запроса добавьте представление объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44623-127">In the request body, supply a JSON representation for the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

<span data-ttu-id="44623-128">В следующей таблице приведены свойства, необходимые при создании [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md).</span><span class="sxs-lookup"><span data-stu-id="44623-128">The following table shows the properties that are required when you create the [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>

|<span data-ttu-id="44623-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="44623-129">Property</span></span>|<span data-ttu-id="44623-130">Тип</span><span class="sxs-lookup"><span data-stu-id="44623-130">Type</span></span>|<span data-ttu-id="44623-131">Описание</span><span class="sxs-lookup"><span data-stu-id="44623-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44623-132">id</span><span class="sxs-lookup"><span data-stu-id="44623-132">id</span></span>|<span data-ttu-id="44623-133">String</span><span class="sxs-lookup"><span data-stu-id="44623-133">String</span></span>|<span data-ttu-id="44623-134">Ключ Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="44623-134">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="44623-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44623-135">lastModifiedDateTime</span></span>|<span data-ttu-id="44623-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44623-136">DateTimeOffset</span></span>|<span data-ttu-id="44623-137">Время последнего изменения Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="44623-137">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="44623-138">target</span><span class="sxs-lookup"><span data-stu-id="44623-138">target</span></span>|[<span data-ttu-id="44623-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="44623-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="44623-140">Целевая группа Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="44623-140">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="44623-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="44623-141">Response</span></span>
<span data-ttu-id="44623-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44623-142">If successful, this method returns a `200 OK` response code and an updated [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44623-143">Пример</span><span class="sxs-lookup"><span data-stu-id="44623-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="44623-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="44623-144">Request</span></span>
<span data-ttu-id="44623-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44623-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="44623-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="44623-146">Response</span></span>
<span data-ttu-id="44623-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44623-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




