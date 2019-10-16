---
title: Обновление Полицисетассигнмент
description: Обновление свойств объекта Полицисетассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c3d2f0f5824e45dd76b5fbda46c5e7702105390a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536296"
---
# <a name="update-policysetassignment"></a><span data-ttu-id="89ddc-103">Обновление Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="89ddc-103">Update policySetAssignment</span></span>

> <span data-ttu-id="89ddc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89ddc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89ddc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89ddc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89ddc-106">Обновление свойств объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="89ddc-106">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89ddc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="89ddc-107">Prerequisites</span></span>
<span data-ttu-id="89ddc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89ddc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89ddc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89ddc-110">Permission type</span></span>|<span data-ttu-id="89ddc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89ddc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89ddc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89ddc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89ddc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ddc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89ddc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89ddc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89ddc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89ddc-115">Not supported.</span></span>|
|<span data-ttu-id="89ddc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="89ddc-116">Application</span></span>|<span data-ttu-id="89ddc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ddc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89ddc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89ddc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="89ddc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89ddc-119">Request headers</span></span>
|<span data-ttu-id="89ddc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89ddc-120">Header</span></span>|<span data-ttu-id="89ddc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="89ddc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89ddc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89ddc-122">Authorization</span></span>|<span data-ttu-id="89ddc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89ddc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89ddc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="89ddc-124">Accept</span></span>|<span data-ttu-id="89ddc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89ddc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89ddc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89ddc-126">Request body</span></span>
<span data-ttu-id="89ddc-127">В тексте запроса добавьте представление объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89ddc-127">In the request body, supply a JSON representation for the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

<span data-ttu-id="89ddc-128">В следующей таблице приведены свойства, необходимые при создании [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md).</span><span class="sxs-lookup"><span data-stu-id="89ddc-128">The following table shows the properties that are required when you create the [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>

|<span data-ttu-id="89ddc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="89ddc-129">Property</span></span>|<span data-ttu-id="89ddc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="89ddc-130">Type</span></span>|<span data-ttu-id="89ddc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="89ddc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89ddc-132">id</span><span class="sxs-lookup"><span data-stu-id="89ddc-132">id</span></span>|<span data-ttu-id="89ddc-133">String</span><span class="sxs-lookup"><span data-stu-id="89ddc-133">String</span></span>|<span data-ttu-id="89ddc-134">Ключ Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="89ddc-134">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="89ddc-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89ddc-135">lastModifiedDateTime</span></span>|<span data-ttu-id="89ddc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89ddc-136">DateTimeOffset</span></span>|<span data-ttu-id="89ddc-137">Время последнего изменения Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="89ddc-137">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="89ddc-138">target</span><span class="sxs-lookup"><span data-stu-id="89ddc-138">target</span></span>|[<span data-ttu-id="89ddc-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="89ddc-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="89ddc-140">Целевая группа Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="89ddc-140">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="89ddc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="89ddc-141">Response</span></span>
<span data-ttu-id="89ddc-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89ddc-142">If successful, this method returns a `200 OK` response code and an updated [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89ddc-143">Пример</span><span class="sxs-lookup"><span data-stu-id="89ddc-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="89ddc-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="89ddc-144">Request</span></span>
<span data-ttu-id="89ddc-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89ddc-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89ddc-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="89ddc-146">Response</span></span>
<span data-ttu-id="89ddc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89ddc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






