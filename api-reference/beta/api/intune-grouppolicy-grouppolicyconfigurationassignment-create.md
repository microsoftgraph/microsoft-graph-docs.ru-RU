---
title: Создание groupPolicyConfigurationAssignment
description: Создание объекта groupPolicyConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d6fb517a5803c06144104116a55a26e3d246e68d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155029"
---
# <a name="create-grouppolicyconfigurationassignment"></a><span data-ttu-id="8d137-103">Создание groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8d137-103">Create groupPolicyConfigurationAssignment</span></span>

<span data-ttu-id="8d137-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d137-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d137-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d137-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d137-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d137-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d137-107">Создание объекта [groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8d137-107">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d137-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d137-108">Prerequisites</span></span>
<span data-ttu-id="8d137-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d137-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d137-111">Permission type</span></span>|<span data-ttu-id="8d137-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d137-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d137-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d137-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d137-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d137-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d137-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d137-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d137-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d137-116">Not supported.</span></span>|
|<span data-ttu-id="8d137-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d137-117">Application</span></span>|<span data-ttu-id="8d137-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d137-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d137-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d137-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8d137-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8d137-120">Request headers</span></span>
|<span data-ttu-id="8d137-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d137-121">Header</span></span>|<span data-ttu-id="8d137-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8d137-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d137-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d137-123">Authorization</span></span>|<span data-ttu-id="8d137-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d137-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d137-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8d137-125">Accept</span></span>|<span data-ttu-id="8d137-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d137-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d137-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d137-127">Request body</span></span>
<span data-ttu-id="8d137-128">В теле запроса предоставляем представление объекта groupPolicyConfigurationAssignment в JSON.</span><span class="sxs-lookup"><span data-stu-id="8d137-128">In the request body, supply a JSON representation for the groupPolicyConfigurationAssignment object.</span></span>

<span data-ttu-id="8d137-129">В следующей таблице показаны свойства, необходимые при создании объекта groupPolicyConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="8d137-129">The following table shows the properties that are required when you create the groupPolicyConfigurationAssignment.</span></span>

|<span data-ttu-id="8d137-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d137-130">Property</span></span>|<span data-ttu-id="8d137-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8d137-131">Type</span></span>|<span data-ttu-id="8d137-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8d137-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d137-133">id</span><span class="sxs-lookup"><span data-stu-id="8d137-133">id</span></span>|<span data-ttu-id="8d137-134">String</span><span class="sxs-lookup"><span data-stu-id="8d137-134">String</span></span>|<span data-ttu-id="8d137-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8d137-135">Key of the entity.</span></span>|
|<span data-ttu-id="8d137-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d137-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8d137-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d137-137">DateTimeOffset</span></span>|<span data-ttu-id="8d137-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8d137-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="8d137-139">target</span><span class="sxs-lookup"><span data-stu-id="8d137-139">target</span></span>|[<span data-ttu-id="8d137-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8d137-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8d137-141">Тип групп, нацеленных на конфигурацию групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8d137-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="8d137-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d137-142">Response</span></span>
<span data-ttu-id="8d137-143">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d137-143">If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d137-144">Пример</span><span class="sxs-lookup"><span data-stu-id="8d137-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d137-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d137-145">Request</span></span>
<span data-ttu-id="8d137-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d137-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
Content-type: application/json
Content-length: 393

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="8d137-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d137-147">Response</span></span>
<span data-ttu-id="8d137-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d137-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 506

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




