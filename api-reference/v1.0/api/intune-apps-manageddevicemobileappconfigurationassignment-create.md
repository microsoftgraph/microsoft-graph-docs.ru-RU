---
title: Создание объекта managedDeviceMobileAppConfigurationAssignment
description: Создание объекта managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75529eecc0fcfaf9df78ccec4e8caec3199e59af
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961408"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="76438-103">Создание объекта managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="76438-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="76438-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76438-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76438-105">Создание объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="76438-105">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76438-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="76438-106">Prerequisites</span></span>
<span data-ttu-id="76438-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76438-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76438-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76438-109">Permission type</span></span>|<span data-ttu-id="76438-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="76438-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76438-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76438-111">Delegated (work or school account)</span></span>|<span data-ttu-id="76438-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76438-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="76438-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76438-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76438-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76438-114">Not supported.</span></span>|
|<span data-ttu-id="76438-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76438-115">Application</span></span>|<span data-ttu-id="76438-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76438-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76438-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76438-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="76438-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76438-118">Request headers</span></span>
|<span data-ttu-id="76438-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76438-119">Header</span></span>|<span data-ttu-id="76438-120">Значение</span><span class="sxs-lookup"><span data-stu-id="76438-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76438-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76438-121">Authorization</span></span>|<span data-ttu-id="76438-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76438-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76438-123">Accept</span><span class="sxs-lookup"><span data-stu-id="76438-123">Accept</span></span>|<span data-ttu-id="76438-124">application/json</span><span class="sxs-lookup"><span data-stu-id="76438-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76438-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76438-125">Request body</span></span>
<span data-ttu-id="76438-126">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76438-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="76438-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="76438-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="76438-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="76438-128">Property</span></span>|<span data-ttu-id="76438-129">Тип</span><span class="sxs-lookup"><span data-stu-id="76438-129">Type</span></span>|<span data-ttu-id="76438-130">Описание</span><span class="sxs-lookup"><span data-stu-id="76438-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76438-131">id</span><span class="sxs-lookup"><span data-stu-id="76438-131">id</span></span>|<span data-ttu-id="76438-132">String</span><span class="sxs-lookup"><span data-stu-id="76438-132">String</span></span>|<span data-ttu-id="76438-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="76438-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="76438-134">target</span><span class="sxs-lookup"><span data-stu-id="76438-134">target</span></span>|[<span data-ttu-id="76438-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="76438-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="76438-136">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="76438-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="76438-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="76438-137">Response</span></span>
<span data-ttu-id="76438-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76438-138">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76438-139">Пример</span><span class="sxs-lookup"><span data-stu-id="76438-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="76438-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="76438-140">Request</span></span>
<span data-ttu-id="76438-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76438-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="76438-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="76438-142">Response</span></span>
<span data-ttu-id="76438-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76438-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



