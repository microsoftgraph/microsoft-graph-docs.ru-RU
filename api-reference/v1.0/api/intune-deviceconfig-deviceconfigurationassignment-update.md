---
title: Обновление объекта deviceConfigurationAssignment
description: Обновление свойств объекта deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c39a50f5cfba40cf4b41f654e75cd84e69b7f8cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894357"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="c06cf-103">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c06cf-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="c06cf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c06cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c06cf-105">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c06cf-105">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c06cf-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c06cf-106">Prerequisites</span></span>
<span data-ttu-id="c06cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c06cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c06cf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c06cf-109">Permission type</span></span>|<span data-ttu-id="c06cf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c06cf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c06cf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c06cf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c06cf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c06cf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c06cf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c06cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c06cf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c06cf-114">Not supported.</span></span>|
|<span data-ttu-id="c06cf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c06cf-115">Application</span></span>|<span data-ttu-id="c06cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c06cf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c06cf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c06cf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c06cf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c06cf-118">Request headers</span></span>
|<span data-ttu-id="c06cf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c06cf-119">Header</span></span>|<span data-ttu-id="c06cf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c06cf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c06cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c06cf-121">Authorization</span></span>|<span data-ttu-id="c06cf-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c06cf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c06cf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c06cf-123">Accept</span></span>|<span data-ttu-id="c06cf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c06cf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c06cf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c06cf-125">Request body</span></span>
<span data-ttu-id="c06cf-126">В тексте запроса добавьте представление объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c06cf-126">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="c06cf-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c06cf-127">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="c06cf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c06cf-128">Property</span></span>|<span data-ttu-id="c06cf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c06cf-129">Type</span></span>|<span data-ttu-id="c06cf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c06cf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c06cf-131">id</span><span class="sxs-lookup"><span data-stu-id="c06cf-131">id</span></span>|<span data-ttu-id="c06cf-132">String</span><span class="sxs-lookup"><span data-stu-id="c06cf-132">String</span></span>|<span data-ttu-id="c06cf-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="c06cf-133">The key of the assignment.</span></span>|
|<span data-ttu-id="c06cf-134">target</span><span class="sxs-lookup"><span data-stu-id="c06cf-134">target</span></span>|[<span data-ttu-id="c06cf-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c06cf-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c06cf-136">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="c06cf-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="c06cf-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c06cf-137">Response</span></span>
<span data-ttu-id="c06cf-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c06cf-138">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c06cf-139">Пример</span><span class="sxs-lookup"><span data-stu-id="c06cf-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="c06cf-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="c06cf-140">Request</span></span>
<span data-ttu-id="c06cf-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c06cf-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c06cf-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="c06cf-142">Response</span></span>
<span data-ttu-id="c06cf-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c06cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



