---
title: Обновление объекта deviceConfigurationAssignment
description: Обновление свойств объекта deviceConfigurationAssignment.
ms.openlocfilehash: 7bf756193ef2ce60ccf992b0ee5feb7644a461a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025771"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="9d0ef-103">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9d0ef-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="9d0ef-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9d0ef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d0ef-105">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9d0ef-105">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d0ef-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9d0ef-106">Prerequisites</span></span>
<span data-ttu-id="9d0ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d0ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d0ef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d0ef-109">Permission type</span></span>|<span data-ttu-id="9d0ef-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d0ef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d0ef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d0ef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9d0ef-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d0ef-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d0ef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d0ef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d0ef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d0ef-114">Not supported.</span></span>|
|<span data-ttu-id="9d0ef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d0ef-115">Application</span></span>|<span data-ttu-id="9d0ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d0ef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d0ef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d0ef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9d0ef-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d0ef-118">Request headers</span></span>
|<span data-ttu-id="9d0ef-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d0ef-119">Header</span></span>|<span data-ttu-id="9d0ef-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9d0ef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d0ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d0ef-121">Authorization</span></span>|<span data-ttu-id="9d0ef-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9d0ef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d0ef-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9d0ef-123">Accept</span></span>|<span data-ttu-id="9d0ef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9d0ef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d0ef-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d0ef-125">Request body</span></span>
<span data-ttu-id="9d0ef-126">В тексте запроса добавьте представление объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d0ef-126">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="9d0ef-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9d0ef-127">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="9d0ef-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d0ef-128">Property</span></span>|<span data-ttu-id="9d0ef-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9d0ef-129">Type</span></span>|<span data-ttu-id="9d0ef-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9d0ef-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d0ef-131">id</span><span class="sxs-lookup"><span data-stu-id="9d0ef-131">id</span></span>|<span data-ttu-id="9d0ef-132">String</span><span class="sxs-lookup"><span data-stu-id="9d0ef-132">String</span></span>|<span data-ttu-id="9d0ef-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="9d0ef-133">The key of the assignment.</span></span>|
|<span data-ttu-id="9d0ef-134">target</span><span class="sxs-lookup"><span data-stu-id="9d0ef-134">target</span></span>|[<span data-ttu-id="9d0ef-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9d0ef-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9d0ef-136">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="9d0ef-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="9d0ef-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d0ef-137">Response</span></span>
<span data-ttu-id="9d0ef-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d0ef-138">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d0ef-139">Пример</span><span class="sxs-lookup"><span data-stu-id="9d0ef-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d0ef-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d0ef-140">Request</span></span>
<span data-ttu-id="9d0ef-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d0ef-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="9d0ef-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d0ef-142">Response</span></span>
<span data-ttu-id="9d0ef-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9d0ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



