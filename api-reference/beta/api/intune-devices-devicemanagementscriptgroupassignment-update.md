---
title: Обновление deviceManagementScriptGroupAssignment
description: Обновление свойства объекта deviceManagementScriptGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d6988bec87e9470e3c46a7c47c483529ca1e2c86
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869239"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="36dcd-103">Обновление deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="36dcd-103">Update deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="36dcd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="36dcd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36dcd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36dcd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36dcd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="36dcd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36dcd-107">Обновление свойства объекта [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="36dcd-107">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36dcd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="36dcd-108">Prerequisites</span></span>
<span data-ttu-id="36dcd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36dcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36dcd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36dcd-111">Permission type</span></span>|<span data-ttu-id="36dcd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36dcd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36dcd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36dcd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36dcd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36dcd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="36dcd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36dcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36dcd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36dcd-116">Not supported.</span></span>|
|<span data-ttu-id="36dcd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36dcd-117">Application</span></span>|<span data-ttu-id="36dcd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36dcd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36dcd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36dcd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="36dcd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36dcd-120">Request headers</span></span>
|<span data-ttu-id="36dcd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36dcd-121">Header</span></span>|<span data-ttu-id="36dcd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="36dcd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36dcd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36dcd-123">Authorization</span></span>|<span data-ttu-id="36dcd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="36dcd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36dcd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36dcd-125">Accept</span></span>|<span data-ttu-id="36dcd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36dcd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36dcd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36dcd-127">Request body</span></span>
<span data-ttu-id="36dcd-128">В тексте запроса укажите представление JSON для объекта [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="36dcd-128">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="36dcd-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="36dcd-129">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="36dcd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="36dcd-130">Property</span></span>|<span data-ttu-id="36dcd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="36dcd-131">Type</span></span>|<span data-ttu-id="36dcd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="36dcd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36dcd-133">id</span><span class="sxs-lookup"><span data-stu-id="36dcd-133">id</span></span>|<span data-ttu-id="36dcd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="36dcd-134">String</span></span>|<span data-ttu-id="36dcd-135">Ключ объекта назначения группы, сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="36dcd-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="36dcd-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="36dcd-136">targetGroupId</span></span>|<span data-ttu-id="36dcd-137">Строка</span><span class="sxs-lookup"><span data-stu-id="36dcd-137">String</span></span>|<span data-ttu-id="36dcd-138">Идентификатор группы Azure Active Directory мы ориентация сценария.</span><span class="sxs-lookup"><span data-stu-id="36dcd-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="36dcd-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="36dcd-139">Response</span></span>
<span data-ttu-id="36dcd-140">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="36dcd-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36dcd-141">Пример</span><span class="sxs-lookup"><span data-stu-id="36dcd-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="36dcd-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="36dcd-142">Request</span></span>
<span data-ttu-id="36dcd-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36dcd-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 48

{
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="36dcd-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="36dcd-144">Response</span></span>
<span data-ttu-id="36dcd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="36dcd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```





