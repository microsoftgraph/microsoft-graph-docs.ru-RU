---
title: Обновление объекта managedDeviceMobileAppConfigurationAssignment
description: Обновление свойств объекта managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ec20c87f64a61da24188977715da1f0738b1b0f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887686"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="5dc38-103">Обновление объекта managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5dc38-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="5dc38-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5dc38-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5dc38-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5dc38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5dc38-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5dc38-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5dc38-107">Обновление свойств объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5dc38-107">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5dc38-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5dc38-108">Prerequisites</span></span>
<span data-ttu-id="5dc38-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dc38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dc38-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5dc38-111">Permission type</span></span>|<span data-ttu-id="5dc38-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5dc38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dc38-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5dc38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5dc38-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dc38-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5dc38-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5dc38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dc38-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5dc38-116">Not supported.</span></span>|
|<span data-ttu-id="5dc38-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5dc38-117">Application</span></span>|<span data-ttu-id="5dc38-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5dc38-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dc38-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5dc38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5dc38-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5dc38-120">Request headers</span></span>
|<span data-ttu-id="5dc38-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5dc38-121">Header</span></span>|<span data-ttu-id="5dc38-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5dc38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dc38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dc38-123">Authorization</span></span>|<span data-ttu-id="5dc38-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5dc38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5dc38-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5dc38-125">Accept</span></span>|<span data-ttu-id="5dc38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5dc38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dc38-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5dc38-127">Request body</span></span>
<span data-ttu-id="5dc38-128">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5dc38-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="5dc38-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5dc38-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="5dc38-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5dc38-130">Property</span></span>|<span data-ttu-id="5dc38-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5dc38-131">Type</span></span>|<span data-ttu-id="5dc38-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5dc38-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc38-133">id</span><span class="sxs-lookup"><span data-stu-id="5dc38-133">id</span></span>|<span data-ttu-id="5dc38-134">String</span><span class="sxs-lookup"><span data-stu-id="5dc38-134">String</span></span>|<span data-ttu-id="5dc38-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="5dc38-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5dc38-136">target</span><span class="sxs-lookup"><span data-stu-id="5dc38-136">target</span></span>|[<span data-ttu-id="5dc38-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5dc38-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5dc38-138">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="5dc38-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="5dc38-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5dc38-139">Response</span></span>
<span data-ttu-id="5dc38-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5dc38-140">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dc38-141">Пример</span><span class="sxs-lookup"><span data-stu-id="5dc38-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="5dc38-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5dc38-142">Request</span></span>
<span data-ttu-id="5dc38-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5dc38-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="5dc38-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="5dc38-144">Response</span></span>
<span data-ttu-id="5dc38-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5dc38-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





