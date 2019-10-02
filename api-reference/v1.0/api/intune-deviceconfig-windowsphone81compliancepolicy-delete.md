---
title: Удаление объекта windowsPhone81CompliancePolicy
description: Удаляет объект windowsPhone81CompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8d00d9f76f0623959dfdc7dd32fd6a4e480cfd24
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364916"
---
# <a name="delete-windowsphone81compliancepolicy"></a><span data-ttu-id="6e313-103">Удаление объекта windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6e313-103">Delete windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="6e313-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e313-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e313-105">Удаляет объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e313-105">Deletes a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e313-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6e313-106">Prerequisites</span></span>
<span data-ttu-id="6e313-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e313-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e313-109">Permission type</span></span>|<span data-ttu-id="6e313-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e313-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e313-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e313-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6e313-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e313-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e313-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e313-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e313-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e313-114">Not supported.</span></span>|
|<span data-ttu-id="6e313-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e313-115">Application</span></span>|<span data-ttu-id="6e313-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e313-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e313-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e313-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6e313-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e313-118">Request headers</span></span>
|<span data-ttu-id="6e313-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e313-119">Header</span></span>|<span data-ttu-id="6e313-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6e313-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e313-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e313-121">Authorization</span></span>|<span data-ttu-id="6e313-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e313-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e313-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6e313-123">Accept</span></span>|<span data-ttu-id="6e313-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6e313-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e313-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e313-125">Request body</span></span>
<span data-ttu-id="6e313-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e313-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e313-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e313-127">Response</span></span>
<span data-ttu-id="6e313-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6e313-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6e313-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6e313-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e313-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e313-130">Request</span></span>
<span data-ttu-id="6e313-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e313-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="6e313-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e313-132">Response</span></span>
<span data-ttu-id="6e313-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e313-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




