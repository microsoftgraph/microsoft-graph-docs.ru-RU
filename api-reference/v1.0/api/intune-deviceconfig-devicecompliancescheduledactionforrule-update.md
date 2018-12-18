---
title: Обновление объекта deviceComplianceScheduledActionForRule
description: Обновление свойств объекта deviceComplianceScheduledActionForRule.
author: tfitzmac
ms.openlocfilehash: e63602cf39aa89bfdcda2db900d993d8e0a56d9d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301661"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="3c3b0-103">Обновление объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="3c3b0-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="3c3b0-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3c3b0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c3b0-105">Обновление свойств объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="3c3b0-105">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c3b0-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3c3b0-106">Prerequisites</span></span>
<span data-ttu-id="3c3b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c3b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c3b0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c3b0-109">Permission type</span></span>|<span data-ttu-id="3c3b0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c3b0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c3b0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c3b0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3c3b0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c3b0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c3b0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c3b0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c3b0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c3b0-114">Not supported.</span></span>|
|<span data-ttu-id="3c3b0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c3b0-115">Application</span></span>|<span data-ttu-id="3c3b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c3b0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c3b0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c3b0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="3c3b0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c3b0-118">Request headers</span></span>
|<span data-ttu-id="3c3b0-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c3b0-119">Header</span></span>|<span data-ttu-id="3c3b0-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3c3b0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c3b0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c3b0-121">Authorization</span></span>|<span data-ttu-id="3c3b0-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3c3b0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c3b0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3c3b0-123">Accept</span></span>|<span data-ttu-id="3c3b0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3c3b0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c3b0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c3b0-125">Request body</span></span>
<span data-ttu-id="3c3b0-126">В тексте запроса добавьте представление объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c3b0-126">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="3c3b0-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="3c3b0-127">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="3c3b0-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c3b0-128">Property</span></span>|<span data-ttu-id="3c3b0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3c3b0-129">Type</span></span>|<span data-ttu-id="3c3b0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3c3b0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c3b0-131">id</span><span class="sxs-lookup"><span data-stu-id="3c3b0-131">id</span></span>|<span data-ttu-id="3c3b0-132">Строка</span><span class="sxs-lookup"><span data-stu-id="3c3b0-132">String</span></span>|<span data-ttu-id="3c3b0-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3c3b0-133">Key of the entity.</span></span>|
|<span data-ttu-id="3c3b0-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="3c3b0-134">ruleName</span></span>|<span data-ttu-id="3c3b0-135">String</span><span class="sxs-lookup"><span data-stu-id="3c3b0-135">String</span></span>|<span data-ttu-id="3c3b0-136">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="3c3b0-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="3c3b0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c3b0-137">Response</span></span>
<span data-ttu-id="3c3b0-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c3b0-138">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c3b0-139">Пример</span><span class="sxs-lookup"><span data-stu-id="3c3b0-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c3b0-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c3b0-140">Request</span></span>
<span data-ttu-id="3c3b0-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c3b0-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="3c3b0-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c3b0-142">Response</span></span>
<span data-ttu-id="3c3b0-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3c3b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```



