---
title: Создание deviceManagementScriptGroupAssignment
description: Создание нового объекта deviceManagementScriptGroupAssignment.
ms.openlocfilehash: 3a92632ad1ab900ddff8371ce37bedb4f16f6d55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075449"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="04c99-103">Создание deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="04c99-103">Create deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="04c99-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="04c99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04c99-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04c99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04c99-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="04c99-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04c99-107">Создание нового объекта [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="04c99-107">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04c99-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="04c99-108">Prerequisites</span></span>
<span data-ttu-id="04c99-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04c99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04c99-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04c99-111">Permission type</span></span>|<span data-ttu-id="04c99-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04c99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04c99-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04c99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04c99-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04c99-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="04c99-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04c99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04c99-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04c99-116">Not supported.</span></span>|
|<span data-ttu-id="04c99-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04c99-117">Application</span></span>|<span data-ttu-id="04c99-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04c99-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04c99-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04c99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="04c99-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04c99-120">Request headers</span></span>
|<span data-ttu-id="04c99-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04c99-121">Header</span></span>|<span data-ttu-id="04c99-122">Значение</span><span class="sxs-lookup"><span data-stu-id="04c99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04c99-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04c99-123">Authorization</span></span>|<span data-ttu-id="04c99-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="04c99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04c99-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04c99-125">Accept</span></span>|<span data-ttu-id="04c99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04c99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04c99-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04c99-127">Request body</span></span>
<span data-ttu-id="04c99-128">В тексте запроса укажите представление JSON для объекта deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="04c99-128">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="04c99-129">В следующей таблице показаны свойства, которые необходимы для создания deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="04c99-129">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="04c99-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="04c99-130">Property</span></span>|<span data-ttu-id="04c99-131">Тип</span><span class="sxs-lookup"><span data-stu-id="04c99-131">Type</span></span>|<span data-ttu-id="04c99-132">Описание</span><span class="sxs-lookup"><span data-stu-id="04c99-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04c99-133">id</span><span class="sxs-lookup"><span data-stu-id="04c99-133">id</span></span>|<span data-ttu-id="04c99-134">String</span><span class="sxs-lookup"><span data-stu-id="04c99-134">String</span></span>|<span data-ttu-id="04c99-135">Ключ объекта назначения группы, сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="04c99-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="04c99-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="04c99-136">targetGroupId</span></span>|<span data-ttu-id="04c99-137">String</span><span class="sxs-lookup"><span data-stu-id="04c99-137">String</span></span>|<span data-ttu-id="04c99-138">Идентификатор группы Azure Active Directory мы ориентация сценария.</span><span class="sxs-lookup"><span data-stu-id="04c99-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="04c99-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="04c99-139">Response</span></span>
<span data-ttu-id="04c99-140">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="04c99-140">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04c99-141">Пример</span><span class="sxs-lookup"><span data-stu-id="04c99-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="04c99-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="04c99-142">Request</span></span>
<span data-ttu-id="04c99-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04c99-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="04c99-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="04c99-144">Response</span></span>
<span data-ttu-id="04c99-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="04c99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```





