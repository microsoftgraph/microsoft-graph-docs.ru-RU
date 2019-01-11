---
title: Действие scheduleActionsForRules
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9516edaec94aaa62980f416d1ba5ccfc30bef743
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805238"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="75c7e-103">Действие scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="75c7e-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="75c7e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="75c7e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75c7e-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="75c7e-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="75c7e-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="75c7e-106">Prerequisites</span></span>
<span data-ttu-id="75c7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75c7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75c7e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75c7e-109">Permission type</span></span>|<span data-ttu-id="75c7e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75c7e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75c7e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75c7e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75c7e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75c7e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75c7e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75c7e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75c7e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75c7e-114">Not supported.</span></span>|
|<span data-ttu-id="75c7e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75c7e-115">Application</span></span>|<span data-ttu-id="75c7e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75c7e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75c7e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75c7e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="75c7e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75c7e-118">Request headers</span></span>
|<span data-ttu-id="75c7e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75c7e-119">Header</span></span>|<span data-ttu-id="75c7e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="75c7e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75c7e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="75c7e-121">Authorization</span></span>|<span data-ttu-id="75c7e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="75c7e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75c7e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="75c7e-123">Accept</span></span>|<span data-ttu-id="75c7e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="75c7e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75c7e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75c7e-125">Request body</span></span>
<span data-ttu-id="75c7e-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75c7e-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="75c7e-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="75c7e-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="75c7e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="75c7e-128">Property</span></span>|<span data-ttu-id="75c7e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="75c7e-129">Type</span></span>|<span data-ttu-id="75c7e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="75c7e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75c7e-131">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="75c7e-131">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="75c7e-132">Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="75c7e-132">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="75c7e-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="75c7e-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="75c7e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="75c7e-134">Response</span></span>
<span data-ttu-id="75c7e-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="75c7e-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="75c7e-136">Пример</span><span class="sxs-lookup"><span data-stu-id="75c7e-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="75c7e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="75c7e-137">Request</span></span>
<span data-ttu-id="75c7e-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75c7e-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules

Content-type: application/json
Content-length: 242

{
  "deviceComplianceScheduledActionForRules": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
      "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
      "ruleName": "Rule Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="75c7e-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="75c7e-139">Response</span></span>
<span data-ttu-id="75c7e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="75c7e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



