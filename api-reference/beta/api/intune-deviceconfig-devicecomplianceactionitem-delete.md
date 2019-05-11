---
title: Delete deviceComplianceActionItem
description: Удаляет объект deviceComplianceActionItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a8fba50e46a733ba3d565fd295817f20f7c3619
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928017"
---
# <a name="delete-devicecomplianceactionitem"></a><span data-ttu-id="6640c-103">Delete deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="6640c-103">Delete deviceComplianceActionItem</span></span>

> <span data-ttu-id="6640c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6640c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6640c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6640c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6640c-106">Удаляет объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="6640c-106">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6640c-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6640c-107">Prerequisites</span></span>
<span data-ttu-id="6640c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6640c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6640c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6640c-110">Permission type</span></span>|<span data-ttu-id="6640c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6640c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6640c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6640c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6640c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6640c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6640c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6640c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6640c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6640c-115">Not supported.</span></span>|
|<span data-ttu-id="6640c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6640c-116">Application</span></span>|<span data-ttu-id="6640c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6640c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6640c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6640c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="6640c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6640c-119">Request headers</span></span>
|<span data-ttu-id="6640c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6640c-120">Header</span></span>|<span data-ttu-id="6640c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6640c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6640c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6640c-122">Authorization</span></span>|<span data-ttu-id="6640c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6640c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6640c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6640c-124">Accept</span></span>|<span data-ttu-id="6640c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6640c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6640c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6640c-126">Request body</span></span>
<span data-ttu-id="6640c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6640c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6640c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6640c-128">Response</span></span>
<span data-ttu-id="6640c-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6640c-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6640c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6640c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6640c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6640c-131">Request</span></span>
<span data-ttu-id="6640c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6640c-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="6640c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6640c-133">Response</span></span>
<span data-ttu-id="6640c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6640c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




