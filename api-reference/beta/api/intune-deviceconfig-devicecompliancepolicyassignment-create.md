---
title: Создание объекта deviceCompliancePolicyAssignment
description: Создание объекта deviceCompliancePolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3c181e7362528fe0231e2e744f59ac82d7ee333e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847959"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="3a00f-103">Создание объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="3a00f-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="3a00f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a00f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a00f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a00f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a00f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3a00f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a00f-107">Создание объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3a00f-107">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3a00f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3a00f-108">Prerequisites</span></span>
<span data-ttu-id="3a00f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a00f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a00f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a00f-111">Permission type</span></span>|<span data-ttu-id="3a00f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a00f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a00f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a00f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a00f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a00f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a00f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a00f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a00f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a00f-116">Not supported.</span></span>|
|<span data-ttu-id="3a00f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a00f-117">Application</span></span>|<span data-ttu-id="3a00f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a00f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a00f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a00f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="3a00f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a00f-120">Request headers</span></span>
|<span data-ttu-id="3a00f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a00f-121">Header</span></span>|<span data-ttu-id="3a00f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a00f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a00f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a00f-123">Authorization</span></span>|<span data-ttu-id="3a00f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3a00f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a00f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a00f-125">Accept</span></span>|<span data-ttu-id="3a00f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a00f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a00f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a00f-127">Request body</span></span>
<span data-ttu-id="3a00f-128">В тексте запроса добавьте представление объекта deviceCompliancePolicyAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a00f-128">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="3a00f-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="3a00f-129">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="3a00f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a00f-130">Property</span></span>|<span data-ttu-id="3a00f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3a00f-131">Type</span></span>|<span data-ttu-id="3a00f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3a00f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a00f-133">id</span><span class="sxs-lookup"><span data-stu-id="3a00f-133">id</span></span>|<span data-ttu-id="3a00f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3a00f-134">String</span></span>|<span data-ttu-id="3a00f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3a00f-135">Key of the entity.</span></span>|
|<span data-ttu-id="3a00f-136">target</span><span class="sxs-lookup"><span data-stu-id="3a00f-136">target</span></span>|[<span data-ttu-id="3a00f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3a00f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3a00f-138">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="3a00f-138">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="3a00f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a00f-139">Response</span></span>
<span data-ttu-id="3a00f-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a00f-140">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a00f-141">Пример</span><span class="sxs-lookup"><span data-stu-id="3a00f-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a00f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a00f-142">Request</span></span>
<span data-ttu-id="3a00f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a00f-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3a00f-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a00f-144">Response</span></span>
<span data-ttu-id="3a00f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3a00f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





