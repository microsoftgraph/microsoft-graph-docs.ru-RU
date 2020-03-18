---
title: Создание Граупполициконфигуратионассигнмент
description: Создание нового объекта Граупполициконфигуратионассигнмент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6db5c38bd96a01ffc8bf360acedc815e26302f0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804473"
---
# <a name="create-grouppolicyconfigurationassignment"></a><span data-ttu-id="8edaf-103">Создание Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="8edaf-103">Create groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="8edaf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8edaf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8edaf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8edaf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8edaf-106">Создание нового объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8edaf-106">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8edaf-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8edaf-107">Prerequisites</span></span>
<span data-ttu-id="8edaf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8edaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8edaf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8edaf-110">Permission type</span></span>|<span data-ttu-id="8edaf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8edaf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8edaf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8edaf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8edaf-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8edaf-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8edaf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8edaf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8edaf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8edaf-115">Not supported.</span></span>|
|<span data-ttu-id="8edaf-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8edaf-116">Application</span></span>|<span data-ttu-id="8edaf-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8edaf-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8edaf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8edaf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8edaf-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8edaf-119">Request headers</span></span>
|<span data-ttu-id="8edaf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8edaf-120">Header</span></span>|<span data-ttu-id="8edaf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8edaf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8edaf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8edaf-122">Authorization</span></span>|<span data-ttu-id="8edaf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8edaf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8edaf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8edaf-124">Accept</span></span>|<span data-ttu-id="8edaf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8edaf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8edaf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8edaf-126">Request body</span></span>
<span data-ttu-id="8edaf-127">В тексте запроса добавьте представление объекта Граупполициконфигуратионассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8edaf-127">In the request body, supply a JSON representation for the groupPolicyConfigurationAssignment object.</span></span>

<span data-ttu-id="8edaf-128">В следующей таблице приведены свойства, необходимые при создании Граупполициконфигуратионассигнмент.</span><span class="sxs-lookup"><span data-stu-id="8edaf-128">The following table shows the properties that are required when you create the groupPolicyConfigurationAssignment.</span></span>

|<span data-ttu-id="8edaf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8edaf-129">Property</span></span>|<span data-ttu-id="8edaf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8edaf-130">Type</span></span>|<span data-ttu-id="8edaf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8edaf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8edaf-132">id</span><span class="sxs-lookup"><span data-stu-id="8edaf-132">id</span></span>|<span data-ttu-id="8edaf-133">String</span><span class="sxs-lookup"><span data-stu-id="8edaf-133">String</span></span>|<span data-ttu-id="8edaf-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8edaf-134">Key of the entity.</span></span>|
|<span data-ttu-id="8edaf-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8edaf-135">lastModifiedDateTime</span></span>|<span data-ttu-id="8edaf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8edaf-136">DateTimeOffset</span></span>|<span data-ttu-id="8edaf-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8edaf-137">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="8edaf-138">target</span><span class="sxs-lookup"><span data-stu-id="8edaf-138">target</span></span>|[<span data-ttu-id="8edaf-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8edaf-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8edaf-140">Тип групп, нацеленных на конфигурацию групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8edaf-140">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="8edaf-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8edaf-141">Response</span></span>
<span data-ttu-id="8edaf-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8edaf-142">If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8edaf-143">Пример</span><span class="sxs-lookup"><span data-stu-id="8edaf-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8edaf-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="8edaf-144">Request</span></span>
<span data-ttu-id="8edaf-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8edaf-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="8edaf-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8edaf-146">Response</span></span>
<span data-ttu-id="8edaf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8edaf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




