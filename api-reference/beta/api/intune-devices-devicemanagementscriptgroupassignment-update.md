---
title: Обновление deviceManagementScriptGroupAssignment
description: Обновление свойства объекта deviceManagementScriptGroupAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bab2f5e2c363d56379e240eb6c26b95e7a0fc8b9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409981"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="85ea8-103">Обновление deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="85ea8-103">Update deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="85ea8-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="85ea8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="85ea8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85ea8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85ea8-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85ea8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85ea8-107">Обновление свойства объекта [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="85ea8-107">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85ea8-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="85ea8-108">Prerequisites</span></span>
<span data-ttu-id="85ea8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="85ea8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="85ea8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85ea8-111">Permission type</span></span>|<span data-ttu-id="85ea8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85ea8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85ea8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85ea8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85ea8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85ea8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="85ea8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85ea8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85ea8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85ea8-116">Not supported.</span></span>|
|<span data-ttu-id="85ea8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85ea8-117">Application</span></span>|<span data-ttu-id="85ea8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85ea8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85ea8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85ea8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="85ea8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85ea8-120">Request headers</span></span>
|<span data-ttu-id="85ea8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85ea8-121">Header</span></span>|<span data-ttu-id="85ea8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="85ea8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85ea8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85ea8-123">Authorization</span></span>|<span data-ttu-id="85ea8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="85ea8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85ea8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="85ea8-125">Accept</span></span>|<span data-ttu-id="85ea8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85ea8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85ea8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85ea8-127">Request body</span></span>
<span data-ttu-id="85ea8-128">В тексте запроса укажите представление JSON для объекта [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="85ea8-128">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="85ea8-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="85ea8-129">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="85ea8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="85ea8-130">Property</span></span>|<span data-ttu-id="85ea8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="85ea8-131">Type</span></span>|<span data-ttu-id="85ea8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="85ea8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85ea8-133">id</span><span class="sxs-lookup"><span data-stu-id="85ea8-133">id</span></span>|<span data-ttu-id="85ea8-134">String</span><span class="sxs-lookup"><span data-stu-id="85ea8-134">String</span></span>|<span data-ttu-id="85ea8-135">Ключ объекта назначения группы, сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="85ea8-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="85ea8-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="85ea8-136">targetGroupId</span></span>|<span data-ttu-id="85ea8-137">String</span><span class="sxs-lookup"><span data-stu-id="85ea8-137">String</span></span>|<span data-ttu-id="85ea8-138">Идентификатор группы Azure Active Directory мы ориентация сценария.</span><span class="sxs-lookup"><span data-stu-id="85ea8-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="85ea8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="85ea8-139">Response</span></span>
<span data-ttu-id="85ea8-140">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="85ea8-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85ea8-141">Пример</span><span class="sxs-lookup"><span data-stu-id="85ea8-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="85ea8-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="85ea8-142">Request</span></span>
<span data-ttu-id="85ea8-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85ea8-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="85ea8-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="85ea8-144">Response</span></span>
<span data-ttu-id="85ea8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="85ea8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




