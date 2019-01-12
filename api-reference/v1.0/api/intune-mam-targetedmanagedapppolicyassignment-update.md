---
title: Обновление объекта targetedManagedAppPolicyAssignment
description: Обновление свойств объекта targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5d20413017c9a1063204273574bb9b24e8ba31b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927767"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="50c42-103">Обновление объекта targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="50c42-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="50c42-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="50c42-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50c42-105">Обновление свойств объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="50c42-105">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50c42-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="50c42-106">Prerequisites</span></span>
<span data-ttu-id="50c42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50c42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50c42-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50c42-109">Permission type</span></span>|<span data-ttu-id="50c42-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50c42-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50c42-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50c42-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50c42-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50c42-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50c42-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50c42-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50c42-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50c42-114">Not supported.</span></span>|
|<span data-ttu-id="50c42-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50c42-115">Application</span></span>|<span data-ttu-id="50c42-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50c42-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50c42-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50c42-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="50c42-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50c42-118">Request headers</span></span>
|<span data-ttu-id="50c42-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50c42-119">Header</span></span>|<span data-ttu-id="50c42-120">Значение</span><span class="sxs-lookup"><span data-stu-id="50c42-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50c42-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="50c42-121">Authorization</span></span>|<span data-ttu-id="50c42-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="50c42-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50c42-123">Accept</span><span class="sxs-lookup"><span data-stu-id="50c42-123">Accept</span></span>|<span data-ttu-id="50c42-124">application/json</span><span class="sxs-lookup"><span data-stu-id="50c42-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50c42-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50c42-125">Request body</span></span>
<span data-ttu-id="50c42-126">В теле запроса добавьте представление объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50c42-126">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="50c42-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="50c42-127">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="50c42-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="50c42-128">Property</span></span>|<span data-ttu-id="50c42-129">Тип</span><span class="sxs-lookup"><span data-stu-id="50c42-129">Type</span></span>|<span data-ttu-id="50c42-130">Описание</span><span class="sxs-lookup"><span data-stu-id="50c42-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50c42-131">id</span><span class="sxs-lookup"><span data-stu-id="50c42-131">id</span></span>|<span data-ttu-id="50c42-132">String</span><span class="sxs-lookup"><span data-stu-id="50c42-132">String</span></span>|<span data-ttu-id="50c42-133">Id</span><span class="sxs-lookup"><span data-stu-id="50c42-133">Id</span></span>|
|<span data-ttu-id="50c42-134">target</span><span class="sxs-lookup"><span data-stu-id="50c42-134">target</span></span>|[<span data-ttu-id="50c42-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="50c42-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="50c42-136">Идентификатор для развертывания группы или приложения</span><span class="sxs-lookup"><span data-stu-id="50c42-136">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="50c42-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="50c42-137">Response</span></span>
<span data-ttu-id="50c42-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="50c42-138">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50c42-139">Пример</span><span class="sxs-lookup"><span data-stu-id="50c42-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="50c42-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="50c42-140">Request</span></span>
<span data-ttu-id="50c42-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50c42-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="50c42-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="50c42-142">Response</span></span>
<span data-ttu-id="50c42-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="50c42-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



