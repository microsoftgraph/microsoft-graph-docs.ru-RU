---
title: Действие scheduleActionsForRules
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 541a2038f1eb8d6f67ca86dad0664fbdec83c3cd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927799"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="15504-103">Действие scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="15504-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="15504-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15504-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15504-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15504-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15504-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="15504-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15504-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="15504-107">Prerequisites</span></span>
<span data-ttu-id="15504-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15504-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15504-110">Permission type</span></span>|<span data-ttu-id="15504-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15504-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15504-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15504-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15504-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15504-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15504-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15504-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15504-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15504-115">Not supported.</span></span>|
|<span data-ttu-id="15504-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15504-116">Application</span></span>|<span data-ttu-id="15504-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15504-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15504-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15504-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="15504-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15504-119">Request headers</span></span>
|<span data-ttu-id="15504-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15504-120">Header</span></span>|<span data-ttu-id="15504-121">Значение</span><span class="sxs-lookup"><span data-stu-id="15504-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15504-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15504-122">Authorization</span></span>|<span data-ttu-id="15504-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15504-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15504-124">Accept</span><span class="sxs-lookup"><span data-stu-id="15504-124">Accept</span></span>|<span data-ttu-id="15504-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15504-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15504-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="15504-126">Request body</span></span>
<span data-ttu-id="15504-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15504-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="15504-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="15504-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="15504-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="15504-129">Property</span></span>|<span data-ttu-id="15504-130">Тип</span><span class="sxs-lookup"><span data-stu-id="15504-130">Type</span></span>|<span data-ttu-id="15504-131">Описание</span><span class="sxs-lookup"><span data-stu-id="15504-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15504-132">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="15504-132">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="15504-133">Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="15504-133">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="15504-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="15504-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="15504-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="15504-135">Response</span></span>
<span data-ttu-id="15504-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="15504-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="15504-137">Пример</span><span class="sxs-lookup"><span data-stu-id="15504-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="15504-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="15504-138">Request</span></span>
<span data-ttu-id="15504-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15504-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules

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

### <a name="response"></a><span data-ttu-id="15504-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="15504-140">Response</span></span>
<span data-ttu-id="15504-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15504-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




