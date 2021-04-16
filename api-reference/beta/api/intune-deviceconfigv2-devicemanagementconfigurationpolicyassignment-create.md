---
title: Создание deviceManagementConfigurationPolicyAssignment
description: Создание нового объекта deviceManagementConfigurationPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6e5a2d59c519de6184069296bf1e0cad3b812363
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864020"
---
# <a name="create-devicemanagementconfigurationpolicyassignment"></a><span data-ttu-id="1b725-103">Создание deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="1b725-103">Create deviceManagementConfigurationPolicyAssignment</span></span>

<span data-ttu-id="1b725-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b725-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b725-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b725-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b725-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b725-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b725-107">Создание нового [объекта deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1b725-107">Create a new [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b725-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1b725-108">Prerequisites</span></span>
<span data-ttu-id="1b725-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b725-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b725-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b725-111">Permission type</span></span>|<span data-ttu-id="1b725-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b725-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b725-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b725-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b725-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b725-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b725-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b725-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b725-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b725-116">Not supported.</span></span>|
|<span data-ttu-id="1b725-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1b725-117">Application</span></span>|<span data-ttu-id="1b725-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b725-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b725-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b725-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1b725-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1b725-120">Request headers</span></span>
|<span data-ttu-id="1b725-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b725-121">Header</span></span>|<span data-ttu-id="1b725-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1b725-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b725-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b725-123">Authorization</span></span>|<span data-ttu-id="1b725-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b725-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b725-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1b725-125">Accept</span></span>|<span data-ttu-id="1b725-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b725-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b725-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b725-127">Request body</span></span>
<span data-ttu-id="1b725-128">В теле запроса поставляем представление JSON для объекта deviceManagementConfigurationPolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="1b725-128">In the request body, supply a JSON representation for the deviceManagementConfigurationPolicyAssignment object.</span></span>

<span data-ttu-id="1b725-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementConfigurationPolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="1b725-129">The following table shows the properties that are required when you create the deviceManagementConfigurationPolicyAssignment.</span></span>

|<span data-ttu-id="1b725-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b725-130">Property</span></span>|<span data-ttu-id="1b725-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1b725-131">Type</span></span>|<span data-ttu-id="1b725-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1b725-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b725-133">id</span><span class="sxs-lookup"><span data-stu-id="1b725-133">id</span></span>|<span data-ttu-id="1b725-134">String</span><span class="sxs-lookup"><span data-stu-id="1b725-134">String</span></span>|<span data-ttu-id="1b725-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="1b725-135">The key of the assignment.</span></span>|
|<span data-ttu-id="1b725-136">target</span><span class="sxs-lookup"><span data-stu-id="1b725-136">target</span></span>|[<span data-ttu-id="1b725-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1b725-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1b725-138">Цель назначения для DeviceManagementConfigurationPolicy.</span><span class="sxs-lookup"><span data-stu-id="1b725-138">The assignment target for the DeviceManagementConfigurationPolicy.</span></span>|



## <a name="response"></a><span data-ttu-id="1b725-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b725-139">Response</span></span>
<span data-ttu-id="1b725-140">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1b725-140">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b725-141">Пример</span><span class="sxs-lookup"><span data-stu-id="1b725-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b725-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b725-142">Request</span></span>
<span data-ttu-id="1b725-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b725-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="1b725-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b725-144">Response</span></span>
<span data-ttu-id="1b725-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b725-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "id": "1f069921-9921-1f06-2199-061f2199061f",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




