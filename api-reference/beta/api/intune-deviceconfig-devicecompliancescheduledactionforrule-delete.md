---
title: Удаление объекта deviceComplianceScheduledActionForRule
description: Удаляет объект deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f09e4e691955928668215709b24326d3b52b1afc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144340"
---
# <a name="delete-devicecompliancescheduledactionforrule"></a><span data-ttu-id="b2121-103">Удаление объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="b2121-103">Delete deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="b2121-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2121-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2121-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2121-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2121-106">Удаляет объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="b2121-106">Deletes a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2121-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b2121-107">Prerequisites</span></span>
<span data-ttu-id="b2121-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b2121-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b2121-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2121-110">Permission type</span></span>|<span data-ttu-id="b2121-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2121-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2121-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2121-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2121-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2121-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2121-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2121-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2121-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2121-115">Not supported.</span></span>|
|<span data-ttu-id="b2121-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2121-116">Application</span></span>|<span data-ttu-id="b2121-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2121-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2121-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2121-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="b2121-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2121-119">Request headers</span></span>
|<span data-ttu-id="b2121-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2121-120">Header</span></span>|<span data-ttu-id="b2121-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b2121-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2121-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2121-122">Authorization</span></span>|<span data-ttu-id="b2121-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b2121-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2121-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b2121-124">Accept</span></span>|<span data-ttu-id="b2121-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2121-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2121-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2121-126">Request body</span></span>
<span data-ttu-id="b2121-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2121-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2121-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2121-128">Response</span></span>
<span data-ttu-id="b2121-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b2121-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b2121-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b2121-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2121-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2121-131">Request</span></span>
<span data-ttu-id="b2121-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2121-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

### <a name="response"></a><span data-ttu-id="b2121-133">Отклик
</span><span class="sxs-lookup"><span data-stu-id="b2121-133">Response</span></span>
<span data-ttu-id="b2121-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b2121-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




