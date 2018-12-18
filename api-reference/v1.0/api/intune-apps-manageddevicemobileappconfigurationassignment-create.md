---
title: Создание объекта managedDeviceMobileAppConfigurationAssignment
description: Создание объекта managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
ms.openlocfilehash: 998ba77acbd34a9aed605502ad833b708a79977d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330123"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="453f9-103">Создание объекта managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="453f9-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="453f9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="453f9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="453f9-105">Создание объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="453f9-105">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="453f9-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="453f9-106">Prerequisites</span></span>
<span data-ttu-id="453f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="453f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="453f9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="453f9-109">Permission type</span></span>|<span data-ttu-id="453f9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="453f9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="453f9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="453f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="453f9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="453f9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="453f9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="453f9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="453f9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="453f9-114">Not supported.</span></span>|
|<span data-ttu-id="453f9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="453f9-115">Application</span></span>|<span data-ttu-id="453f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="453f9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="453f9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="453f9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="453f9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="453f9-118">Request headers</span></span>
|<span data-ttu-id="453f9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="453f9-119">Header</span></span>|<span data-ttu-id="453f9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="453f9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="453f9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="453f9-121">Authorization</span></span>|<span data-ttu-id="453f9-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="453f9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="453f9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="453f9-123">Accept</span></span>|<span data-ttu-id="453f9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="453f9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="453f9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="453f9-125">Request body</span></span>
<span data-ttu-id="453f9-126">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="453f9-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="453f9-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="453f9-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="453f9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="453f9-128">Property</span></span>|<span data-ttu-id="453f9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="453f9-129">Type</span></span>|<span data-ttu-id="453f9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="453f9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="453f9-131">id</span><span class="sxs-lookup"><span data-stu-id="453f9-131">id</span></span>|<span data-ttu-id="453f9-132">String</span><span class="sxs-lookup"><span data-stu-id="453f9-132">String</span></span>|<span data-ttu-id="453f9-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="453f9-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="453f9-134">target</span><span class="sxs-lookup"><span data-stu-id="453f9-134">target</span></span>|[<span data-ttu-id="453f9-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="453f9-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="453f9-136">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="453f9-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="453f9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="453f9-137">Response</span></span>
<span data-ttu-id="453f9-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="453f9-138">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="453f9-139">Пример</span><span class="sxs-lookup"><span data-stu-id="453f9-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="453f9-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="453f9-140">Request</span></span>
<span data-ttu-id="453f9-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="453f9-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="453f9-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="453f9-142">Response</span></span>
<span data-ttu-id="453f9-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="453f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



