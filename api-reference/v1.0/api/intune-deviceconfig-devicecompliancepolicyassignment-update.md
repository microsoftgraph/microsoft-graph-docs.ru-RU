---
title: Обновление объекта deviceCompliancePolicyAssignment
description: Обновление свойств объекта deviceCompliancePolicyAssignment.
author: tfitzmac
ms.openlocfilehash: 9319b3b429e9ddff67ee66ecb93e7111e5732db6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319112"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="546fb-103">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="546fb-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="546fb-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="546fb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="546fb-105">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="546fb-105">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="546fb-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="546fb-106">Prerequisites</span></span>
<span data-ttu-id="546fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="546fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="546fb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="546fb-109">Permission type</span></span>|<span data-ttu-id="546fb-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="546fb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="546fb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="546fb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="546fb-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="546fb-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="546fb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="546fb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="546fb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="546fb-114">Not supported.</span></span>|
|<span data-ttu-id="546fb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="546fb-115">Application</span></span>|<span data-ttu-id="546fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="546fb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="546fb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="546fb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="546fb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="546fb-118">Request headers</span></span>
|<span data-ttu-id="546fb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="546fb-119">Header</span></span>|<span data-ttu-id="546fb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="546fb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="546fb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="546fb-121">Authorization</span></span>|<span data-ttu-id="546fb-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="546fb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="546fb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="546fb-123">Accept</span></span>|<span data-ttu-id="546fb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="546fb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="546fb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="546fb-125">Request body</span></span>
<span data-ttu-id="546fb-126">В тексте запроса добавьте представление объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="546fb-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="546fb-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="546fb-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="546fb-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="546fb-128">Property</span></span>|<span data-ttu-id="546fb-129">Тип</span><span class="sxs-lookup"><span data-stu-id="546fb-129">Type</span></span>|<span data-ttu-id="546fb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="546fb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="546fb-131">id</span><span class="sxs-lookup"><span data-stu-id="546fb-131">id</span></span>|<span data-ttu-id="546fb-132">Строка</span><span class="sxs-lookup"><span data-stu-id="546fb-132">String</span></span>|<span data-ttu-id="546fb-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="546fb-133">Key of the entity.</span></span>|
|<span data-ttu-id="546fb-134">target</span><span class="sxs-lookup"><span data-stu-id="546fb-134">target</span></span>|[<span data-ttu-id="546fb-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="546fb-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="546fb-136">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="546fb-136">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="546fb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="546fb-137">Response</span></span>
<span data-ttu-id="546fb-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="546fb-138">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="546fb-139">Пример</span><span class="sxs-lookup"><span data-stu-id="546fb-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="546fb-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="546fb-140">Request</span></span>
<span data-ttu-id="546fb-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="546fb-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="546fb-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="546fb-142">Response</span></span>
<span data-ttu-id="546fb-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="546fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



