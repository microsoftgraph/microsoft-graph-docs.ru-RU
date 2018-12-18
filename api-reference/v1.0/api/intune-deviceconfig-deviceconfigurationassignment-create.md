---
title: Создание объекта deviceConfigurationAssignment
description: Создание объекта deviceConfigurationAssignment.
author: tfitzmac
ms.openlocfilehash: d278c04f0372869bf6b79e63a68d27766ef36485
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329108"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="0d978-103">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0d978-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="0d978-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0d978-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d978-105">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0d978-105">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0d978-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0d978-106">Prerequisites</span></span>
<span data-ttu-id="0d978-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d978-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d978-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d978-109">Permission type</span></span>|<span data-ttu-id="0d978-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d978-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d978-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d978-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0d978-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d978-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d978-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d978-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d978-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d978-114">Not supported.</span></span>|
|<span data-ttu-id="0d978-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d978-115">Application</span></span>|<span data-ttu-id="0d978-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d978-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d978-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d978-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0d978-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d978-118">Request headers</span></span>
|<span data-ttu-id="0d978-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d978-119">Header</span></span>|<span data-ttu-id="0d978-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0d978-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d978-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d978-121">Authorization</span></span>|<span data-ttu-id="0d978-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0d978-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d978-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0d978-123">Accept</span></span>|<span data-ttu-id="0d978-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0d978-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d978-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d978-125">Request body</span></span>
<span data-ttu-id="0d978-126">В тексте запроса добавьте представление объекта deviceConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d978-126">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="0d978-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="0d978-127">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="0d978-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d978-128">Property</span></span>|<span data-ttu-id="0d978-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0d978-129">Type</span></span>|<span data-ttu-id="0d978-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0d978-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d978-131">id</span><span class="sxs-lookup"><span data-stu-id="0d978-131">id</span></span>|<span data-ttu-id="0d978-132">String</span><span class="sxs-lookup"><span data-stu-id="0d978-132">String</span></span>|<span data-ttu-id="0d978-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="0d978-133">The key of the assignment.</span></span>|
|<span data-ttu-id="0d978-134">target</span><span class="sxs-lookup"><span data-stu-id="0d978-134">target</span></span>|[<span data-ttu-id="0d978-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0d978-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0d978-136">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="0d978-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="0d978-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d978-137">Response</span></span>
<span data-ttu-id="0d978-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d978-138">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d978-139">Пример</span><span class="sxs-lookup"><span data-stu-id="0d978-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d978-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d978-140">Request</span></span>
<span data-ttu-id="0d978-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d978-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d978-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d978-142">Response</span></span>
<span data-ttu-id="0d978-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0d978-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



