---
title: Создание объекта deviceComplianceScheduledActionForRule
description: Создание объекта deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ecaff4ee51e8f2c8b764b641d924f695bd194140
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997675"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="16e65-103">Создание объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="16e65-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="16e65-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16e65-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16e65-105">Создание объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="16e65-105">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16e65-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="16e65-106">Prerequisites</span></span>
<span data-ttu-id="16e65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16e65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16e65-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16e65-109">Permission type</span></span>|<span data-ttu-id="16e65-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16e65-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16e65-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16e65-111">Delegated (work or school account)</span></span>|<span data-ttu-id="16e65-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e65-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16e65-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16e65-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16e65-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16e65-114">Not supported.</span></span>|
|<span data-ttu-id="16e65-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16e65-115">Application</span></span>|<span data-ttu-id="16e65-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16e65-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16e65-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16e65-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="16e65-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16e65-118">Request headers</span></span>
|<span data-ttu-id="16e65-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16e65-119">Header</span></span>|<span data-ttu-id="16e65-120">Значение</span><span class="sxs-lookup"><span data-stu-id="16e65-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16e65-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16e65-121">Authorization</span></span>|<span data-ttu-id="16e65-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16e65-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16e65-123">Accept</span><span class="sxs-lookup"><span data-stu-id="16e65-123">Accept</span></span>|<span data-ttu-id="16e65-124">application/json</span><span class="sxs-lookup"><span data-stu-id="16e65-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16e65-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="16e65-125">Request body</span></span>
<span data-ttu-id="16e65-126">В теле запроса добавьте представление объекта deviceComplianceScheduledActionForRule в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16e65-126">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="16e65-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="16e65-127">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="16e65-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="16e65-128">Property</span></span>|<span data-ttu-id="16e65-129">Тип</span><span class="sxs-lookup"><span data-stu-id="16e65-129">Type</span></span>|<span data-ttu-id="16e65-130">Описание</span><span class="sxs-lookup"><span data-stu-id="16e65-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16e65-131">id</span><span class="sxs-lookup"><span data-stu-id="16e65-131">id</span></span>|<span data-ttu-id="16e65-132">String</span><span class="sxs-lookup"><span data-stu-id="16e65-132">String</span></span>|<span data-ttu-id="16e65-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="16e65-133">Key of the entity.</span></span>|
|<span data-ttu-id="16e65-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="16e65-134">ruleName</span></span>|<span data-ttu-id="16e65-135">String</span><span class="sxs-lookup"><span data-stu-id="16e65-135">String</span></span>|<span data-ttu-id="16e65-136">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="16e65-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="16e65-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="16e65-137">Response</span></span>
<span data-ttu-id="16e65-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="16e65-138">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16e65-139">Пример</span><span class="sxs-lookup"><span data-stu-id="16e65-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="16e65-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="16e65-140">Request</span></span>
<span data-ttu-id="16e65-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16e65-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="16e65-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="16e65-142">Response</span></span>
<span data-ttu-id="16e65-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16e65-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```



