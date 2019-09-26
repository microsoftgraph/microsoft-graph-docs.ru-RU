---
title: Обновление Граупполициконфигуратионассигнмент
description: Обновление свойств объекта Граупполициконфигуратионассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 097c7a828dfabb040ddf2dc27683f47d0dc75797
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179805"
---
# <a name="update-grouppolicyconfigurationassignment"></a><span data-ttu-id="d2d8e-103">Обновление Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="d2d8e-103">Update groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="d2d8e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2d8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2d8e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2d8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2d8e-106">Обновление свойств объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d2d8e-106">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2d8e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d2d8e-107">Prerequisites</span></span>
<span data-ttu-id="d2d8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2d8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2d8e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2d8e-110">Permission type</span></span>|<span data-ttu-id="d2d8e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2d8e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2d8e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2d8e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2d8e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d8e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d2d8e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2d8e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2d8e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2d8e-115">Not supported.</span></span>|
|<span data-ttu-id="d2d8e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2d8e-116">Application</span></span>|<span data-ttu-id="d2d8e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d8e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2d8e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2d8e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d2d8e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2d8e-119">Request headers</span></span>
|<span data-ttu-id="d2d8e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2d8e-120">Header</span></span>|<span data-ttu-id="d2d8e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d2d8e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2d8e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2d8e-122">Authorization</span></span>|<span data-ttu-id="d2d8e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2d8e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2d8e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d2d8e-124">Accept</span></span>|<span data-ttu-id="d2d8e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2d8e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2d8e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2d8e-126">Request body</span></span>
<span data-ttu-id="d2d8e-127">В тексте запроса добавьте представление объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2d8e-127">In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

<span data-ttu-id="d2d8e-128">В следующей таблице приведены свойства, необходимые при создании [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d2d8e-128">The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

|<span data-ttu-id="d2d8e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2d8e-129">Property</span></span>|<span data-ttu-id="d2d8e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d2d8e-130">Type</span></span>|<span data-ttu-id="d2d8e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d2d8e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2d8e-132">id</span><span class="sxs-lookup"><span data-stu-id="d2d8e-132">id</span></span>|<span data-ttu-id="d2d8e-133">String</span><span class="sxs-lookup"><span data-stu-id="d2d8e-133">String</span></span>|<span data-ttu-id="d2d8e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d2d8e-134">Key of the entity.</span></span>|
|<span data-ttu-id="d2d8e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2d8e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d2d8e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2d8e-136">DateTimeOffset</span></span>|<span data-ttu-id="d2d8e-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d2d8e-137">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="d2d8e-138">target</span><span class="sxs-lookup"><span data-stu-id="d2d8e-138">target</span></span>|[<span data-ttu-id="d2d8e-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d2d8e-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d2d8e-140">Тип групп, нацеленных на конфигурацию групповой политики.</span><span class="sxs-lookup"><span data-stu-id="d2d8e-140">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="d2d8e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2d8e-141">Response</span></span>
<span data-ttu-id="d2d8e-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2d8e-142">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2d8e-143">Пример</span><span class="sxs-lookup"><span data-stu-id="d2d8e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2d8e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2d8e-144">Request</span></span>
<span data-ttu-id="d2d8e-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2d8e-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d2d8e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2d8e-146">Response</span></span>
<span data-ttu-id="d2d8e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2d8e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




