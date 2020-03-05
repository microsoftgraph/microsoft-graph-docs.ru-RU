---
title: Обновление Граупполициконфигуратионассигнмент
description: Обновление свойств объекта Граупполициконфигуратионассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a947cae7dd241d11a704ccc9aec10ad45e1c6f41
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465214"
---
# <a name="update-grouppolicyconfigurationassignment"></a><span data-ttu-id="cb3eb-103">Обновление Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="cb3eb-103">Update groupPolicyConfigurationAssignment</span></span>

<span data-ttu-id="cb3eb-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cb3eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb3eb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb3eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb3eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb3eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb3eb-107">Обновление свойств объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="cb3eb-107">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb3eb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cb3eb-108">Prerequisites</span></span>
<span data-ttu-id="cb3eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb3eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb3eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb3eb-111">Permission type</span></span>|<span data-ttu-id="cb3eb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb3eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb3eb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb3eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb3eb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb3eb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cb3eb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb3eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb3eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb3eb-116">Not supported.</span></span>|
|<span data-ttu-id="cb3eb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb3eb-117">Application</span></span>|<span data-ttu-id="cb3eb-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb3eb-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb3eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb3eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="cb3eb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cb3eb-120">Request headers</span></span>
|<span data-ttu-id="cb3eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb3eb-121">Header</span></span>|<span data-ttu-id="cb3eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cb3eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb3eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb3eb-123">Authorization</span></span>|<span data-ttu-id="cb3eb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb3eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb3eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cb3eb-125">Accept</span></span>|<span data-ttu-id="cb3eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb3eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb3eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb3eb-127">Request body</span></span>
<span data-ttu-id="cb3eb-128">В тексте запроса добавьте представление объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb3eb-128">In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

<span data-ttu-id="cb3eb-129">В следующей таблице приведены свойства, необходимые при создании [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cb3eb-129">The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

|<span data-ttu-id="cb3eb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb3eb-130">Property</span></span>|<span data-ttu-id="cb3eb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cb3eb-131">Type</span></span>|<span data-ttu-id="cb3eb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cb3eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb3eb-133">id</span><span class="sxs-lookup"><span data-stu-id="cb3eb-133">id</span></span>|<span data-ttu-id="cb3eb-134">String</span><span class="sxs-lookup"><span data-stu-id="cb3eb-134">String</span></span>|<span data-ttu-id="cb3eb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cb3eb-135">Key of the entity.</span></span>|
|<span data-ttu-id="cb3eb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb3eb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cb3eb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb3eb-137">DateTimeOffset</span></span>|<span data-ttu-id="cb3eb-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cb3eb-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="cb3eb-139">target</span><span class="sxs-lookup"><span data-stu-id="cb3eb-139">target</span></span>|[<span data-ttu-id="cb3eb-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cb3eb-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cb3eb-141">Тип групп, нацеленных на конфигурацию групповой политики.</span><span class="sxs-lookup"><span data-stu-id="cb3eb-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="cb3eb-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb3eb-142">Response</span></span>
<span data-ttu-id="cb3eb-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb3eb-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb3eb-144">Пример</span><span class="sxs-lookup"><span data-stu-id="cb3eb-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb3eb-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb3eb-145">Request</span></span>
<span data-ttu-id="cb3eb-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb3eb-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cb3eb-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb3eb-147">Response</span></span>
<span data-ttu-id="cb3eb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb3eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





