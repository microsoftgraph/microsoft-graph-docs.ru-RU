---
title: Создание объекта deviceComplianceScheduledActionForRule
description: Создание объекта deviceComplianceScheduledActionForRule.
author: tfitzmac
ms.openlocfilehash: 2bf76bc65fe139d41364c9fc1a162d2eadaedec4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327085"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="d1558-103">Создание объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="d1558-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="d1558-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d1558-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1558-105">Создание объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="d1558-105">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d1558-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d1558-106">Prerequisites</span></span>
<span data-ttu-id="d1558-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1558-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1558-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1558-109">Permission type</span></span>|<span data-ttu-id="d1558-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1558-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1558-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1558-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d1558-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1558-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1558-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1558-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1558-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1558-114">Not supported.</span></span>|
|<span data-ttu-id="d1558-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1558-115">Application</span></span>|<span data-ttu-id="d1558-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1558-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1558-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1558-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="d1558-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1558-118">Request headers</span></span>
|<span data-ttu-id="d1558-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1558-119">Header</span></span>|<span data-ttu-id="d1558-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d1558-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1558-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1558-121">Authorization</span></span>|<span data-ttu-id="d1558-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d1558-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1558-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d1558-123">Accept</span></span>|<span data-ttu-id="d1558-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d1558-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1558-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1558-125">Request body</span></span>
<span data-ttu-id="d1558-126">В теле запроса добавьте представление объекта deviceComplianceScheduledActionForRule в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1558-126">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="d1558-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="d1558-127">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="d1558-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1558-128">Property</span></span>|<span data-ttu-id="d1558-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d1558-129">Type</span></span>|<span data-ttu-id="d1558-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d1558-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1558-131">id</span><span class="sxs-lookup"><span data-stu-id="d1558-131">id</span></span>|<span data-ttu-id="d1558-132">Строка</span><span class="sxs-lookup"><span data-stu-id="d1558-132">String</span></span>|<span data-ttu-id="d1558-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d1558-133">Key of the entity.</span></span>|
|<span data-ttu-id="d1558-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="d1558-134">ruleName</span></span>|<span data-ttu-id="d1558-135">String</span><span class="sxs-lookup"><span data-stu-id="d1558-135">String</span></span>|<span data-ttu-id="d1558-136">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="d1558-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="d1558-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1558-137">Response</span></span>
<span data-ttu-id="d1558-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d1558-138">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1558-139">Пример</span><span class="sxs-lookup"><span data-stu-id="d1558-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="d1558-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1558-140">Request</span></span>
<span data-ttu-id="d1558-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1558-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="d1558-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1558-142">Response</span></span>
<span data-ttu-id="d1558-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d1558-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



