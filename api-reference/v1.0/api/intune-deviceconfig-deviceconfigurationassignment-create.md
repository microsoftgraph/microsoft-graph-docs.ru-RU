---
title: Создание объекта deviceConfigurationAssignment
description: Создание объекта deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f16992e3052f9f7017e3177bbfdf2539fe0cfd0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017639"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="9a142-103">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9a142-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="9a142-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a142-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a142-105">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9a142-105">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a142-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9a142-106">Prerequisites</span></span>
<span data-ttu-id="9a142-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a142-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a142-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a142-109">Permission type</span></span>|<span data-ttu-id="9a142-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a142-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a142-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a142-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9a142-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a142-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a142-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a142-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a142-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a142-114">Not supported.</span></span>|
|<span data-ttu-id="9a142-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a142-115">Application</span></span>|<span data-ttu-id="9a142-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a142-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a142-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a142-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9a142-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a142-118">Request headers</span></span>
|<span data-ttu-id="9a142-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a142-119">Header</span></span>|<span data-ttu-id="9a142-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9a142-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a142-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a142-121">Authorization</span></span>|<span data-ttu-id="9a142-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a142-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a142-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9a142-123">Accept</span></span>|<span data-ttu-id="9a142-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9a142-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a142-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a142-125">Request body</span></span>
<span data-ttu-id="9a142-126">В тексте запроса добавьте представление объекта deviceConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a142-126">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="9a142-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="9a142-127">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="9a142-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a142-128">Property</span></span>|<span data-ttu-id="9a142-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9a142-129">Type</span></span>|<span data-ttu-id="9a142-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9a142-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a142-131">id</span><span class="sxs-lookup"><span data-stu-id="9a142-131">id</span></span>|<span data-ttu-id="9a142-132">String</span><span class="sxs-lookup"><span data-stu-id="9a142-132">String</span></span>|<span data-ttu-id="9a142-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="9a142-133">The key of the assignment.</span></span>|
|<span data-ttu-id="9a142-134">target</span><span class="sxs-lookup"><span data-stu-id="9a142-134">target</span></span>|[<span data-ttu-id="9a142-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9a142-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9a142-136">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="9a142-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="9a142-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a142-137">Response</span></span>
<span data-ttu-id="9a142-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a142-138">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a142-139">Пример</span><span class="sxs-lookup"><span data-stu-id="9a142-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a142-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a142-140">Request</span></span>
<span data-ttu-id="9a142-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a142-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="9a142-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a142-142">Response</span></span>
<span data-ttu-id="9a142-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a142-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



