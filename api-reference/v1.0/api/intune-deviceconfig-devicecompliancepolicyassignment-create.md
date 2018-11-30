---
title: Создание объекта deviceCompliancePolicyAssignment
description: Создание объекта deviceCompliancePolicyAssignment.
ms.openlocfilehash: 3830c2d42a69d9efa89303b4230df533a3b2c186
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026726"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="41e39-103">Создание объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="41e39-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="41e39-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="41e39-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41e39-105">Создание объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="41e39-105">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41e39-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="41e39-106">Prerequisites</span></span>
<span data-ttu-id="41e39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41e39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41e39-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41e39-109">Permission type</span></span>|<span data-ttu-id="41e39-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="41e39-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41e39-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41e39-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41e39-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41e39-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41e39-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41e39-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41e39-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41e39-114">Not supported.</span></span>|
|<span data-ttu-id="41e39-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41e39-115">Application</span></span>|<span data-ttu-id="41e39-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41e39-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41e39-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41e39-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="41e39-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41e39-118">Request headers</span></span>
|<span data-ttu-id="41e39-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41e39-119">Header</span></span>|<span data-ttu-id="41e39-120">Значение</span><span class="sxs-lookup"><span data-stu-id="41e39-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41e39-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="41e39-121">Authorization</span></span>|<span data-ttu-id="41e39-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="41e39-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41e39-123">Accept</span><span class="sxs-lookup"><span data-stu-id="41e39-123">Accept</span></span>|<span data-ttu-id="41e39-124">application/json</span><span class="sxs-lookup"><span data-stu-id="41e39-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41e39-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41e39-125">Request body</span></span>
<span data-ttu-id="41e39-126">В тексте запроса добавьте представление объекта deviceCompliancePolicyAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41e39-126">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="41e39-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="41e39-127">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="41e39-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="41e39-128">Property</span></span>|<span data-ttu-id="41e39-129">Тип</span><span class="sxs-lookup"><span data-stu-id="41e39-129">Type</span></span>|<span data-ttu-id="41e39-130">Описание</span><span class="sxs-lookup"><span data-stu-id="41e39-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41e39-131">id</span><span class="sxs-lookup"><span data-stu-id="41e39-131">id</span></span>|<span data-ttu-id="41e39-132">String</span><span class="sxs-lookup"><span data-stu-id="41e39-132">String</span></span>|<span data-ttu-id="41e39-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="41e39-133">Key of the entity.</span></span>|
|<span data-ttu-id="41e39-134">target</span><span class="sxs-lookup"><span data-stu-id="41e39-134">target</span></span>|[<span data-ttu-id="41e39-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="41e39-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="41e39-136">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="41e39-136">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="41e39-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="41e39-137">Response</span></span>
<span data-ttu-id="41e39-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41e39-138">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41e39-139">Пример</span><span class="sxs-lookup"><span data-stu-id="41e39-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="41e39-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="41e39-140">Request</span></span>
<span data-ttu-id="41e39-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41e39-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="41e39-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="41e39-142">Response</span></span>
<span data-ttu-id="41e39-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="41e39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



