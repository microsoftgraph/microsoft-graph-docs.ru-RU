---
title: Обновление объекта deviceConfigurationAssignment
description: Обновление свойств объекта deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0057545bef8312795f78a5e1859621853d879896
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017614"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="37664-103">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="37664-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="37664-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37664-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37664-105">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="37664-105">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37664-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="37664-106">Prerequisites</span></span>
<span data-ttu-id="37664-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37664-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37664-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37664-109">Permission type</span></span>|<span data-ttu-id="37664-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37664-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37664-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37664-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37664-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37664-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37664-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37664-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37664-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37664-114">Not supported.</span></span>|
|<span data-ttu-id="37664-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37664-115">Application</span></span>|<span data-ttu-id="37664-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37664-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37664-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37664-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="37664-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37664-118">Request headers</span></span>
|<span data-ttu-id="37664-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37664-119">Header</span></span>|<span data-ttu-id="37664-120">Значение</span><span class="sxs-lookup"><span data-stu-id="37664-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37664-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37664-121">Authorization</span></span>|<span data-ttu-id="37664-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37664-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37664-123">Accept</span><span class="sxs-lookup"><span data-stu-id="37664-123">Accept</span></span>|<span data-ttu-id="37664-124">application/json</span><span class="sxs-lookup"><span data-stu-id="37664-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37664-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="37664-125">Request body</span></span>
<span data-ttu-id="37664-126">В тексте запроса добавьте представление объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37664-126">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="37664-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="37664-127">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="37664-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="37664-128">Property</span></span>|<span data-ttu-id="37664-129">Тип</span><span class="sxs-lookup"><span data-stu-id="37664-129">Type</span></span>|<span data-ttu-id="37664-130">Описание</span><span class="sxs-lookup"><span data-stu-id="37664-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37664-131">id</span><span class="sxs-lookup"><span data-stu-id="37664-131">id</span></span>|<span data-ttu-id="37664-132">String</span><span class="sxs-lookup"><span data-stu-id="37664-132">String</span></span>|<span data-ttu-id="37664-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="37664-133">The key of the assignment.</span></span>|
|<span data-ttu-id="37664-134">target</span><span class="sxs-lookup"><span data-stu-id="37664-134">target</span></span>|[<span data-ttu-id="37664-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="37664-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="37664-136">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="37664-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="37664-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="37664-137">Response</span></span>
<span data-ttu-id="37664-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37664-138">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37664-139">Пример</span><span class="sxs-lookup"><span data-stu-id="37664-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="37664-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="37664-140">Request</span></span>
<span data-ttu-id="37664-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37664-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37664-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="37664-142">Response</span></span>
<span data-ttu-id="37664-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37664-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



