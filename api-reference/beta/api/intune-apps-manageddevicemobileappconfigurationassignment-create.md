---
title: Создание объекта managedDeviceMobileAppConfigurationAssignment
description: Создание объекта managedDeviceMobileAppConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d91c42d5d012953417de2e25518c45011effcea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961681"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="7e75c-103">Создание объекта managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7e75c-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="7e75c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e75c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e75c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e75c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e75c-106">Создание объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7e75c-106">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e75c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7e75c-107">Prerequisites</span></span>
<span data-ttu-id="7e75c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e75c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e75c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e75c-110">Permission type</span></span>|<span data-ttu-id="7e75c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e75c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e75c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e75c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e75c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e75c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7e75c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e75c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e75c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e75c-115">Not supported.</span></span>|
|<span data-ttu-id="7e75c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e75c-116">Application</span></span>|<span data-ttu-id="7e75c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e75c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e75c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e75c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7e75c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e75c-119">Request headers</span></span>
|<span data-ttu-id="7e75c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e75c-120">Header</span></span>|<span data-ttu-id="7e75c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7e75c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e75c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e75c-122">Authorization</span></span>|<span data-ttu-id="7e75c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e75c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e75c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7e75c-124">Accept</span></span>|<span data-ttu-id="7e75c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7e75c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e75c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e75c-126">Request body</span></span>
<span data-ttu-id="7e75c-127">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e75c-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="7e75c-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="7e75c-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="7e75c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e75c-129">Property</span></span>|<span data-ttu-id="7e75c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7e75c-130">Type</span></span>|<span data-ttu-id="7e75c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7e75c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e75c-132">id</span><span class="sxs-lookup"><span data-stu-id="7e75c-132">id</span></span>|<span data-ttu-id="7e75c-133">String</span><span class="sxs-lookup"><span data-stu-id="7e75c-133">String</span></span>|<span data-ttu-id="7e75c-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="7e75c-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7e75c-135">target</span><span class="sxs-lookup"><span data-stu-id="7e75c-135">target</span></span>|[<span data-ttu-id="7e75c-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7e75c-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7e75c-137">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="7e75c-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="7e75c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e75c-138">Response</span></span>
<span data-ttu-id="7e75c-139">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e75c-139">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e75c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="7e75c-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e75c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e75c-141">Request</span></span>
<span data-ttu-id="7e75c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e75c-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="7e75c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e75c-143">Response</span></span>
<span data-ttu-id="7e75c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e75c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





