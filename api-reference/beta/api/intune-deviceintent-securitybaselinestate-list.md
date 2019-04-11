---
title: Список Секуритибаселинестатес
description: Список свойств и связей объектов Секуритибаселинестате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d1c334b5f377d4fd31e2209bf6940fc2bf65a76
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783495"
---
# <a name="list-securitybaselinestates"></a><span data-ttu-id="d399c-103">Список Секуритибаселинестатес</span><span class="sxs-lookup"><span data-stu-id="d399c-103">List securityBaselineStates</span></span>

> <span data-ttu-id="d399c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d399c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d399c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d399c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d399c-106">Список свойств и связей объектов [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md) .</span><span class="sxs-lookup"><span data-stu-id="d399c-106">List properties and relationships of the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d399c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d399c-107">Prerequisites</span></span>
<span data-ttu-id="d399c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d399c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d399c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d399c-110">Permission type</span></span>|<span data-ttu-id="d399c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d399c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d399c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d399c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d399c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d399c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d399c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d399c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d399c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d399c-115">Not supported.</span></span>|
|<span data-ttu-id="d399c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d399c-116">Application</span></span>|<span data-ttu-id="d399c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d399c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d399c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d399c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
```

## <a name="request-headers"></a><span data-ttu-id="d399c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d399c-119">Request headers</span></span>
|<span data-ttu-id="d399c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d399c-120">Header</span></span>|<span data-ttu-id="d399c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d399c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d399c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d399c-122">Authorization</span></span>|<span data-ttu-id="d399c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d399c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d399c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d399c-124">Accept</span></span>|<span data-ttu-id="d399c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d399c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d399c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d399c-126">Request body</span></span>
<span data-ttu-id="d399c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d399c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d399c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d399c-128">Response</span></span>
<span data-ttu-id="d399c-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d399c-129">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d399c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d399c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d399c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d399c-131">Request</span></span>
<span data-ttu-id="d399c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d399c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
```

### <a name="response"></a><span data-ttu-id="d399c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d399c-133">Response</span></span>
<span data-ttu-id="d399c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d399c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineState",
      "id": "23dc2503-2503-23dc-0325-dc230325dc23",
      "securityBaselineTemplateId": "Security Baseline Template Id value",
      "displayName": "Display Name value"
    }
  ]
}
```



