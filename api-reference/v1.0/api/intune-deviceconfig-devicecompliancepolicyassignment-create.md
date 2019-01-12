---
title: Создание объекта deviceCompliancePolicyAssignment
description: Создание объекта deviceCompliancePolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 162ebaa0cb6bdbd09ae405fd4a29e549830ae4e3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972002"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="e3e9a-103">Создание объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e3e9a-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="e3e9a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e3e9a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3e9a-105">Создание объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e3e9a-105">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3e9a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e3e9a-106">Prerequisites</span></span>
<span data-ttu-id="e3e9a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3e9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3e9a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3e9a-109">Permission type</span></span>|<span data-ttu-id="e3e9a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3e9a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3e9a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3e9a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3e9a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3e9a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3e9a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3e9a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3e9a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3e9a-114">Not supported.</span></span>|
|<span data-ttu-id="e3e9a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3e9a-115">Application</span></span>|<span data-ttu-id="e3e9a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3e9a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3e9a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3e9a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e3e9a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3e9a-118">Request headers</span></span>
|<span data-ttu-id="e3e9a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3e9a-119">Header</span></span>|<span data-ttu-id="e3e9a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e3e9a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3e9a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3e9a-121">Authorization</span></span>|<span data-ttu-id="e3e9a-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e3e9a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3e9a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e3e9a-123">Accept</span></span>|<span data-ttu-id="e3e9a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e3e9a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3e9a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3e9a-125">Request body</span></span>
<span data-ttu-id="e3e9a-126">В тексте запроса добавьте представление объекта deviceCompliancePolicyAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3e9a-126">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="e3e9a-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="e3e9a-127">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="e3e9a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3e9a-128">Property</span></span>|<span data-ttu-id="e3e9a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e3e9a-129">Type</span></span>|<span data-ttu-id="e3e9a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e3e9a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3e9a-131">id</span><span class="sxs-lookup"><span data-stu-id="e3e9a-131">id</span></span>|<span data-ttu-id="e3e9a-132">Строка</span><span class="sxs-lookup"><span data-stu-id="e3e9a-132">String</span></span>|<span data-ttu-id="e3e9a-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e3e9a-133">Key of the entity.</span></span>|
|<span data-ttu-id="e3e9a-134">target</span><span class="sxs-lookup"><span data-stu-id="e3e9a-134">target</span></span>|[<span data-ttu-id="e3e9a-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e3e9a-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e3e9a-136">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="e3e9a-136">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="e3e9a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3e9a-137">Response</span></span>
<span data-ttu-id="e3e9a-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3e9a-138">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3e9a-139">Пример</span><span class="sxs-lookup"><span data-stu-id="e3e9a-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3e9a-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3e9a-140">Request</span></span>
<span data-ttu-id="e3e9a-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3e9a-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e3e9a-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3e9a-142">Response</span></span>
<span data-ttu-id="e3e9a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e3e9a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



