---
title: Удаление deviceCompliancePolicyPolicySetItem
description: Удаляет устройствоCompliancePolicyPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1d2323d19d3c5758cdd520fef4adef283b2e815a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125123"
---
# <a name="delete-devicecompliancepolicypolicysetitem"></a><span data-ttu-id="4f360-103">Удаление deviceCompliancePolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="4f360-103">Delete deviceCompliancePolicyPolicySetItem</span></span>

<span data-ttu-id="4f360-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f360-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f360-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f360-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f360-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f360-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f360-107">Удаляет [устройствоCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="4f360-107">Deletes a [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f360-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4f360-108">Prerequisites</span></span>
<span data-ttu-id="4f360-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f360-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f360-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f360-111">Permission type</span></span>|<span data-ttu-id="4f360-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f360-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f360-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f360-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f360-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f360-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f360-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f360-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f360-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f360-116">Not supported.</span></span>|
|<span data-ttu-id="4f360-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4f360-117">Application</span></span>|<span data-ttu-id="4f360-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f360-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f360-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f360-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="4f360-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f360-120">Request headers</span></span>
|<span data-ttu-id="4f360-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f360-121">Header</span></span>|<span data-ttu-id="4f360-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4f360-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f360-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f360-123">Authorization</span></span>|<span data-ttu-id="4f360-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f360-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f360-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4f360-125">Accept</span></span>|<span data-ttu-id="4f360-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f360-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f360-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f360-127">Request body</span></span>
<span data-ttu-id="4f360-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f360-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f360-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f360-129">Response</span></span>
<span data-ttu-id="4f360-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4f360-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4f360-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4f360-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f360-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f360-132">Request</span></span>
<span data-ttu-id="4f360-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f360-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="4f360-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f360-134">Response</span></span>
<span data-ttu-id="4f360-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f360-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




