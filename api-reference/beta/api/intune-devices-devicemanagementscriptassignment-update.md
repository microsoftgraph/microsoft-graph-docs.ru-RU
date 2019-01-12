---
title: Обновление deviceManagementScriptAssignment
description: Обновление свойства объекта deviceManagementScriptAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 552dffca7adf6825a77e4edb65cf0ceef8fcaa83
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921586"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="21dcd-103">Обновление deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="21dcd-103">Update deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="21dcd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="21dcd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21dcd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21dcd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21dcd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="21dcd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21dcd-107">Обновление свойства объекта [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="21dcd-107">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21dcd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="21dcd-108">Prerequisites</span></span>
<span data-ttu-id="21dcd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21dcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21dcd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21dcd-111">Permission type</span></span>|<span data-ttu-id="21dcd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21dcd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21dcd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21dcd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21dcd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21dcd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="21dcd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21dcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21dcd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21dcd-116">Not supported.</span></span>|
|<span data-ttu-id="21dcd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21dcd-117">Application</span></span>|<span data-ttu-id="21dcd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21dcd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21dcd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21dcd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="21dcd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21dcd-120">Request headers</span></span>
|<span data-ttu-id="21dcd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21dcd-121">Header</span></span>|<span data-ttu-id="21dcd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="21dcd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21dcd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21dcd-123">Authorization</span></span>|<span data-ttu-id="21dcd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="21dcd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21dcd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21dcd-125">Accept</span></span>|<span data-ttu-id="21dcd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21dcd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21dcd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="21dcd-127">Request body</span></span>
<span data-ttu-id="21dcd-128">В тексте запроса укажите представление JSON для объекта [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="21dcd-128">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="21dcd-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="21dcd-129">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="21dcd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="21dcd-130">Property</span></span>|<span data-ttu-id="21dcd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="21dcd-131">Type</span></span>|<span data-ttu-id="21dcd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="21dcd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21dcd-133">id</span><span class="sxs-lookup"><span data-stu-id="21dcd-133">id</span></span>|<span data-ttu-id="21dcd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="21dcd-134">String</span></span>|<span data-ttu-id="21dcd-135">Ключ объекта назначения группы, сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="21dcd-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="21dcd-136">target</span><span class="sxs-lookup"><span data-stu-id="21dcd-136">target</span></span>|[<span data-ttu-id="21dcd-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="21dcd-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="21dcd-138">Идентификатор группы Azure Active Directory мы ориентация сценария.</span><span class="sxs-lookup"><span data-stu-id="21dcd-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="21dcd-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="21dcd-139">Response</span></span>
<span data-ttu-id="21dcd-140">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="21dcd-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21dcd-141">Пример</span><span class="sxs-lookup"><span data-stu-id="21dcd-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="21dcd-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="21dcd-142">Request</span></span>
<span data-ttu-id="21dcd-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21dcd-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="21dcd-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="21dcd-144">Response</span></span>
<span data-ttu-id="21dcd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="21dcd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





