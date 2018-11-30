---
title: Создание объекта deviceComplianceScheduledActionForRule
description: Создание объекта deviceComplianceScheduledActionForRule.
ms.openlocfilehash: 29a20c0fe1246c86abffe6b59e6fd325211a2e14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075542"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="ca4d8-103">Создание объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="ca4d8-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="ca4d8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ca4d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca4d8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca4d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca4d8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ca4d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca4d8-107">Создание объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="ca4d8-107">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca4d8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ca4d8-108">Prerequisites</span></span>
<span data-ttu-id="ca4d8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca4d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca4d8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca4d8-111">Permission type</span></span>|<span data-ttu-id="ca4d8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca4d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca4d8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca4d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca4d8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca4d8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca4d8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca4d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca4d8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca4d8-116">Not supported.</span></span>|
|<span data-ttu-id="ca4d8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca4d8-117">Application</span></span>|<span data-ttu-id="ca4d8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca4d8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca4d8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca4d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="ca4d8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca4d8-120">Request headers</span></span>
|<span data-ttu-id="ca4d8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca4d8-121">Header</span></span>|<span data-ttu-id="ca4d8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ca4d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca4d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca4d8-123">Authorization</span></span>|<span data-ttu-id="ca4d8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ca4d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca4d8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ca4d8-125">Accept</span></span>|<span data-ttu-id="ca4d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca4d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca4d8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ca4d8-127">Request body</span></span>
<span data-ttu-id="ca4d8-128">В теле запроса добавьте представление объекта deviceComplianceScheduledActionForRule в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca4d8-128">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="ca4d8-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="ca4d8-129">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="ca4d8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca4d8-130">Property</span></span>|<span data-ttu-id="ca4d8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ca4d8-131">Type</span></span>|<span data-ttu-id="ca4d8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ca4d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca4d8-133">id</span><span class="sxs-lookup"><span data-stu-id="ca4d8-133">id</span></span>|<span data-ttu-id="ca4d8-134">String</span><span class="sxs-lookup"><span data-stu-id="ca4d8-134">String</span></span>|<span data-ttu-id="ca4d8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ca4d8-135">Key of the entity.</span></span>|
|<span data-ttu-id="ca4d8-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="ca4d8-136">ruleName</span></span>|<span data-ttu-id="ca4d8-137">String</span><span class="sxs-lookup"><span data-stu-id="ca4d8-137">String</span></span>|<span data-ttu-id="ca4d8-138">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="ca4d8-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="ca4d8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca4d8-139">Response</span></span>
<span data-ttu-id="ca4d8-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ca4d8-140">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca4d8-141">Пример</span><span class="sxs-lookup"><span data-stu-id="ca4d8-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca4d8-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca4d8-142">Request</span></span>
<span data-ttu-id="ca4d8-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca4d8-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="ca4d8-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca4d8-144">Response</span></span>
<span data-ttu-id="ca4d8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ca4d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





