---
title: Delete deviceComplianceActionItem
description: Удаляет объект deviceComplianceActionItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 211d594e33e842177343a3937706ba608d0ec806
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155696"
---
# <a name="delete-devicecomplianceactionitem"></a><span data-ttu-id="bc9ca-103">Delete deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="bc9ca-103">Delete deviceComplianceActionItem</span></span>

<span data-ttu-id="bc9ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc9ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc9ca-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc9ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc9ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc9ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc9ca-107">Удаляет объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="bc9ca-107">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc9ca-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bc9ca-108">Prerequisites</span></span>
<span data-ttu-id="bc9ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc9ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc9ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc9ca-111">Permission type</span></span>|<span data-ttu-id="bc9ca-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc9ca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc9ca-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc9ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc9ca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc9ca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc9ca-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc9ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc9ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc9ca-116">Not supported.</span></span>|
|<span data-ttu-id="bc9ca-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bc9ca-117">Application</span></span>|<span data-ttu-id="bc9ca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc9ca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc9ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc9ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="bc9ca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bc9ca-120">Request headers</span></span>
|<span data-ttu-id="bc9ca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc9ca-121">Header</span></span>|<span data-ttu-id="bc9ca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bc9ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc9ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc9ca-123">Authorization</span></span>|<span data-ttu-id="bc9ca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc9ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc9ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bc9ca-125">Accept</span></span>|<span data-ttu-id="bc9ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc9ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc9ca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc9ca-127">Request body</span></span>
<span data-ttu-id="bc9ca-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc9ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc9ca-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc9ca-129">Response</span></span>
<span data-ttu-id="bc9ca-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bc9ca-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bc9ca-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bc9ca-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc9ca-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc9ca-132">Request</span></span>
<span data-ttu-id="bc9ca-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc9ca-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="bc9ca-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc9ca-134">Response</span></span>
<span data-ttu-id="bc9ca-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc9ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




