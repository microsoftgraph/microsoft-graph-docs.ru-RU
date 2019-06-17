---
title: Создание объекта deviceCompliancePolicyAssignment
description: Создание объекта deviceCompliancePolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b46228d5f891b2fd38fde0eacd2936096530fff7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968436"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="d34bc-103">Создание объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d34bc-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="d34bc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d34bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d34bc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d34bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d34bc-106">Создание объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d34bc-106">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d34bc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d34bc-107">Prerequisites</span></span>
<span data-ttu-id="d34bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d34bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d34bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d34bc-110">Permission type</span></span>|<span data-ttu-id="d34bc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d34bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d34bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d34bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d34bc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d34bc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d34bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d34bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d34bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d34bc-115">Not supported.</span></span>|
|<span data-ttu-id="d34bc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d34bc-116">Application</span></span>|<span data-ttu-id="d34bc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d34bc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d34bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d34bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d34bc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d34bc-119">Request headers</span></span>
|<span data-ttu-id="d34bc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d34bc-120">Header</span></span>|<span data-ttu-id="d34bc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d34bc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d34bc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d34bc-122">Authorization</span></span>|<span data-ttu-id="d34bc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d34bc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d34bc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d34bc-124">Accept</span></span>|<span data-ttu-id="d34bc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d34bc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d34bc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d34bc-126">Request body</span></span>
<span data-ttu-id="d34bc-127">В тексте запроса добавьте представление объекта deviceCompliancePolicyAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d34bc-127">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="d34bc-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="d34bc-128">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="d34bc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d34bc-129">Property</span></span>|<span data-ttu-id="d34bc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d34bc-130">Type</span></span>|<span data-ttu-id="d34bc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d34bc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d34bc-132">id</span><span class="sxs-lookup"><span data-stu-id="d34bc-132">id</span></span>|<span data-ttu-id="d34bc-133">String</span><span class="sxs-lookup"><span data-stu-id="d34bc-133">String</span></span>|<span data-ttu-id="d34bc-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d34bc-134">Key of the entity.</span></span>|
|<span data-ttu-id="d34bc-135">target</span><span class="sxs-lookup"><span data-stu-id="d34bc-135">target</span></span>|[<span data-ttu-id="d34bc-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d34bc-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d34bc-137">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="d34bc-137">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="d34bc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d34bc-138">Response</span></span>
<span data-ttu-id="d34bc-139">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d34bc-139">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d34bc-140">Пример</span><span class="sxs-lookup"><span data-stu-id="d34bc-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d34bc-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="d34bc-141">Request</span></span>
<span data-ttu-id="d34bc-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d34bc-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d34bc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d34bc-143">Response</span></span>
<span data-ttu-id="d34bc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d34bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





