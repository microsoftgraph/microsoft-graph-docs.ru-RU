---
title: Создание объекта deviceConfigurationAssignment
description: Создание объекта deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d66bd27a92df4490aa1d8fa2f7065d2f8fe2d38
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548483"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="bc772-103">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="bc772-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="bc772-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc772-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc772-105">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bc772-105">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc772-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bc772-106">Prerequisites</span></span>
<span data-ttu-id="bc772-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc772-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc772-109">Permission type</span></span>|<span data-ttu-id="bc772-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc772-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc772-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc772-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bc772-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc772-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc772-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc772-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc772-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc772-114">Not supported.</span></span>|
|<span data-ttu-id="bc772-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc772-115">Application</span></span>|<span data-ttu-id="bc772-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc772-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc772-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc772-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="bc772-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc772-118">Request headers</span></span>
|<span data-ttu-id="bc772-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc772-119">Header</span></span>|<span data-ttu-id="bc772-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bc772-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc772-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc772-121">Authorization</span></span>|<span data-ttu-id="bc772-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc772-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc772-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bc772-123">Accept</span></span>|<span data-ttu-id="bc772-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bc772-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc772-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc772-125">Request body</span></span>
<span data-ttu-id="bc772-126">В тексте запроса добавьте представление объекта deviceConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc772-126">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="bc772-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="bc772-127">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="bc772-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc772-128">Property</span></span>|<span data-ttu-id="bc772-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bc772-129">Type</span></span>|<span data-ttu-id="bc772-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bc772-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc772-131">id</span><span class="sxs-lookup"><span data-stu-id="bc772-131">id</span></span>|<span data-ttu-id="bc772-132">String</span><span class="sxs-lookup"><span data-stu-id="bc772-132">String</span></span>|<span data-ttu-id="bc772-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="bc772-133">The key of the assignment.</span></span>|
|<span data-ttu-id="bc772-134">target</span><span class="sxs-lookup"><span data-stu-id="bc772-134">target</span></span>|[<span data-ttu-id="bc772-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bc772-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bc772-136">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="bc772-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="bc772-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc772-137">Response</span></span>
<span data-ttu-id="bc772-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc772-138">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc772-139">Пример</span><span class="sxs-lookup"><span data-stu-id="bc772-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc772-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc772-140">Request</span></span>
<span data-ttu-id="bc772-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc772-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bc772-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc772-142">Response</span></span>
<span data-ttu-id="bc772-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc772-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



