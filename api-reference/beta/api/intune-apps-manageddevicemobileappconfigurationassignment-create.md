---
title: Создание объекта managedDeviceMobileAppConfigurationAssignment
description: Создание объекта managedDeviceMobileAppConfigurationAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 10eeb2cdaba8b9e1c855a8e94966ceb0b95c7317
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398046"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="f0100-103">Создание объекта managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f0100-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="f0100-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f0100-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f0100-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0100-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0100-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0100-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0100-107">Создание объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f0100-107">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0100-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0100-108">Prerequisites</span></span>
<span data-ttu-id="f0100-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f0100-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f0100-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0100-111">Permission type</span></span>|<span data-ttu-id="f0100-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0100-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0100-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0100-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0100-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0100-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f0100-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0100-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0100-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0100-116">Not supported.</span></span>|
|<span data-ttu-id="f0100-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0100-117">Application</span></span>|<span data-ttu-id="f0100-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0100-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0100-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0100-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f0100-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0100-120">Request headers</span></span>
|<span data-ttu-id="f0100-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0100-121">Header</span></span>|<span data-ttu-id="f0100-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f0100-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0100-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0100-123">Authorization</span></span>|<span data-ttu-id="f0100-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f0100-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0100-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0100-125">Accept</span></span>|<span data-ttu-id="f0100-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0100-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0100-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0100-127">Request body</span></span>
<span data-ttu-id="f0100-128">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0100-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="f0100-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="f0100-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="f0100-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0100-130">Property</span></span>|<span data-ttu-id="f0100-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f0100-131">Type</span></span>|<span data-ttu-id="f0100-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f0100-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0100-133">id</span><span class="sxs-lookup"><span data-stu-id="f0100-133">id</span></span>|<span data-ttu-id="f0100-134">String</span><span class="sxs-lookup"><span data-stu-id="f0100-134">String</span></span>|<span data-ttu-id="f0100-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="f0100-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="f0100-136">target</span><span class="sxs-lookup"><span data-stu-id="f0100-136">target</span></span>|[<span data-ttu-id="f0100-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f0100-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f0100-138">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="f0100-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="f0100-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0100-139">Response</span></span>
<span data-ttu-id="f0100-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0100-140">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0100-141">Пример</span><span class="sxs-lookup"><span data-stu-id="f0100-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0100-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0100-142">Request</span></span>
<span data-ttu-id="f0100-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0100-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f0100-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0100-144">Response</span></span>
<span data-ttu-id="f0100-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f0100-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




