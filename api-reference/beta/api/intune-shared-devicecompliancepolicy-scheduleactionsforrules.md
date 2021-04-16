---
title: Действие scheduleActionsForRules
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c0e3760ab800e8f341c47a8b416461e7061212ba
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863347"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="2c165-103">Действие scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="2c165-103">scheduleActionsForRules action</span></span>

<span data-ttu-id="2c165-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c165-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c165-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c165-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c165-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c165-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c165-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2c165-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c165-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2c165-108">Prerequisites</span></span>
<span data-ttu-id="2c165-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c165-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c165-111">Permission type</span></span>|<span data-ttu-id="2c165-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c165-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c165-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c165-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2c165-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="2c165-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2c165-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c165-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c165-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c165-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c165-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c165-117">Not supported.</span></span>|
|<span data-ttu-id="2c165-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2c165-118">Application</span></span>||
| <span data-ttu-id="2c165-119">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="2c165-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2c165-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c165-120">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c165-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c165-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="2c165-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2c165-122">Request headers</span></span>
|<span data-ttu-id="2c165-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c165-123">Header</span></span>|<span data-ttu-id="2c165-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2c165-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c165-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c165-125">Authorization</span></span>|<span data-ttu-id="2c165-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c165-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c165-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2c165-127">Accept</span></span>|<span data-ttu-id="2c165-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2c165-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c165-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c165-129">Request body</span></span>
<span data-ttu-id="2c165-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c165-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2c165-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2c165-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2c165-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c165-132">Property</span></span>|<span data-ttu-id="2c165-133">Тип</span><span class="sxs-lookup"><span data-stu-id="2c165-133">Type</span></span>|<span data-ttu-id="2c165-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2c165-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c165-135">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="2c165-135">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="2c165-136">Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="2c165-136">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="2c165-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2c165-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2c165-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c165-138">Response</span></span>
<span data-ttu-id="2c165-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2c165-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2c165-140">Пример</span><span class="sxs-lookup"><span data-stu-id="2c165-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c165-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c165-141">Request</span></span>
<span data-ttu-id="2c165-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c165-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2c165-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c165-143">Response</span></span>
<span data-ttu-id="2c165-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c165-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







