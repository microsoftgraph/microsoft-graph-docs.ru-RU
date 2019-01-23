---
title: Обновление объекта targetedManagedAppPolicyAssignment
description: Обновление свойств объекта targetedManagedAppPolicyAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: da22dcaa56691e3e248664ca32941e29eaa9100a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401497"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="511aa-103">Обновление объекта targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="511aa-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="511aa-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="511aa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="511aa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="511aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="511aa-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="511aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="511aa-107">Обновление свойств объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="511aa-107">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="511aa-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="511aa-108">Prerequisites</span></span>
<span data-ttu-id="511aa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="511aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="511aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="511aa-111">Permission type</span></span>|<span data-ttu-id="511aa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="511aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="511aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="511aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="511aa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="511aa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="511aa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="511aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="511aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="511aa-116">Not supported.</span></span>|
|<span data-ttu-id="511aa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="511aa-117">Application</span></span>|<span data-ttu-id="511aa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="511aa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="511aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="511aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="511aa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="511aa-120">Request headers</span></span>
|<span data-ttu-id="511aa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="511aa-121">Header</span></span>|<span data-ttu-id="511aa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="511aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="511aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="511aa-123">Authorization</span></span>|<span data-ttu-id="511aa-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="511aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="511aa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="511aa-125">Accept</span></span>|<span data-ttu-id="511aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="511aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="511aa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="511aa-127">Request body</span></span>
<span data-ttu-id="511aa-128">В теле запроса добавьте представление объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="511aa-128">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="511aa-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="511aa-129">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="511aa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="511aa-130">Property</span></span>|<span data-ttu-id="511aa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="511aa-131">Type</span></span>|<span data-ttu-id="511aa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="511aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="511aa-133">id</span><span class="sxs-lookup"><span data-stu-id="511aa-133">id</span></span>|<span data-ttu-id="511aa-134">String</span><span class="sxs-lookup"><span data-stu-id="511aa-134">String</span></span>|<span data-ttu-id="511aa-135">Id</span><span class="sxs-lookup"><span data-stu-id="511aa-135">Id</span></span>|
|<span data-ttu-id="511aa-136">target</span><span class="sxs-lookup"><span data-stu-id="511aa-136">target</span></span>|[<span data-ttu-id="511aa-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="511aa-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="511aa-138">Идентификатор для развертывания группы или приложения</span><span class="sxs-lookup"><span data-stu-id="511aa-138">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="511aa-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="511aa-139">Response</span></span>
<span data-ttu-id="511aa-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="511aa-140">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="511aa-141">Пример</span><span class="sxs-lookup"><span data-stu-id="511aa-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="511aa-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="511aa-142">Request</span></span>
<span data-ttu-id="511aa-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="511aa-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="511aa-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="511aa-144">Response</span></span>
<span data-ttu-id="511aa-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="511aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




