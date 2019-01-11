---
title: Удаление объекта deviceComplianceSettingState
description: Удаляет объект deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a98227d69cfb9c8e6eaa48815a3d9f47707ffdd5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866593"
---
# <a name="delete-devicecompliancesettingstate"></a><span data-ttu-id="ede68-103">Удаление объекта deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="ede68-103">Delete deviceComplianceSettingState</span></span>

> <span data-ttu-id="ede68-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ede68-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ede68-105">Удаляет объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="ede68-105">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ede68-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ede68-106">Prerequisites</span></span>
<span data-ttu-id="ede68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ede68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ede68-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ede68-109">Permission type</span></span>|<span data-ttu-id="ede68-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ede68-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ede68-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ede68-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ede68-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ede68-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ede68-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ede68-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ede68-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ede68-114">Not supported.</span></span>|
|<span data-ttu-id="ede68-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ede68-115">Application</span></span>|<span data-ttu-id="ede68-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ede68-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ede68-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ede68-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="ede68-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ede68-118">Request headers</span></span>
|<span data-ttu-id="ede68-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ede68-119">Header</span></span>|<span data-ttu-id="ede68-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ede68-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ede68-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ede68-121">Authorization</span></span>|<span data-ttu-id="ede68-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ede68-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ede68-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ede68-123">Accept</span></span>|<span data-ttu-id="ede68-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ede68-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ede68-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ede68-125">Request body</span></span>
<span data-ttu-id="ede68-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ede68-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ede68-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="ede68-127">Response</span></span>
<span data-ttu-id="ede68-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ede68-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ede68-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ede68-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ede68-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ede68-130">Request</span></span>
<span data-ttu-id="ede68-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ede68-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="ede68-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ede68-132">Response</span></span>
<span data-ttu-id="ede68-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ede68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



