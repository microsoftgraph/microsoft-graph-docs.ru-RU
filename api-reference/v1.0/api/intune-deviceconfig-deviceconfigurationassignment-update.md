---
title: Обновление объекта deviceConfigurationAssignment
description: Обновление свойств объекта deviceConfigurationAssignment.
author: tfitzmac
ms.openlocfilehash: 51b0269a72dbded4f8bdd157683bc321b55874d3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336479"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="b23af-103">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b23af-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="b23af-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b23af-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b23af-105">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b23af-105">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b23af-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b23af-106">Prerequisites</span></span>
<span data-ttu-id="b23af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b23af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b23af-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b23af-109">Permission type</span></span>|<span data-ttu-id="b23af-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b23af-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b23af-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b23af-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b23af-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b23af-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b23af-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b23af-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b23af-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b23af-114">Not supported.</span></span>|
|<span data-ttu-id="b23af-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b23af-115">Application</span></span>|<span data-ttu-id="b23af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b23af-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b23af-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b23af-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b23af-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b23af-118">Request headers</span></span>
|<span data-ttu-id="b23af-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b23af-119">Header</span></span>|<span data-ttu-id="b23af-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b23af-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b23af-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b23af-121">Authorization</span></span>|<span data-ttu-id="b23af-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b23af-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b23af-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b23af-123">Accept</span></span>|<span data-ttu-id="b23af-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b23af-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b23af-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b23af-125">Request body</span></span>
<span data-ttu-id="b23af-126">В тексте запроса добавьте представление объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b23af-126">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="b23af-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b23af-127">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="b23af-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b23af-128">Property</span></span>|<span data-ttu-id="b23af-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b23af-129">Type</span></span>|<span data-ttu-id="b23af-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b23af-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b23af-131">id</span><span class="sxs-lookup"><span data-stu-id="b23af-131">id</span></span>|<span data-ttu-id="b23af-132">String</span><span class="sxs-lookup"><span data-stu-id="b23af-132">String</span></span>|<span data-ttu-id="b23af-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="b23af-133">The key of the assignment.</span></span>|
|<span data-ttu-id="b23af-134">target</span><span class="sxs-lookup"><span data-stu-id="b23af-134">target</span></span>|[<span data-ttu-id="b23af-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b23af-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b23af-136">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="b23af-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="b23af-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b23af-137">Response</span></span>
<span data-ttu-id="b23af-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b23af-138">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b23af-139">Пример</span><span class="sxs-lookup"><span data-stu-id="b23af-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="b23af-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b23af-140">Request</span></span>
<span data-ttu-id="b23af-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b23af-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b23af-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="b23af-142">Response</span></span>
<span data-ttu-id="b23af-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b23af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



