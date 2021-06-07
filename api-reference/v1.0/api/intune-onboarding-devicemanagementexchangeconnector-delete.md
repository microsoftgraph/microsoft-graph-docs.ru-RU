---
title: Удаление объекта deviceManagementExchangeConnector
description: Удаляет объект deviceManagementExchangeConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e81463268c27a50ff39f802662b25e2661f5ea8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754827"
---
# <a name="delete-devicemanagementexchangeconnector"></a><span data-ttu-id="2e308-103">Удаление объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="2e308-103">Delete deviceManagementExchangeConnector</span></span>

<span data-ttu-id="2e308-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e308-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e308-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e308-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e308-106">Удаляет объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="2e308-106">Deletes a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e308-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2e308-107">Prerequisites</span></span>
<span data-ttu-id="2e308-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e308-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e308-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e308-110">Permission type</span></span>|<span data-ttu-id="2e308-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e308-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e308-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e308-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e308-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e308-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2e308-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e308-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e308-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e308-115">Not supported.</span></span>|
|<span data-ttu-id="2e308-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2e308-116">Application</span></span>|<span data-ttu-id="2e308-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e308-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e308-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e308-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="2e308-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2e308-119">Request headers</span></span>
|<span data-ttu-id="2e308-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e308-120">Header</span></span>|<span data-ttu-id="2e308-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2e308-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e308-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e308-122">Authorization</span></span>|<span data-ttu-id="2e308-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e308-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e308-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2e308-124">Accept</span></span>|<span data-ttu-id="2e308-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e308-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e308-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e308-126">Request body</span></span>
<span data-ttu-id="2e308-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e308-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e308-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e308-128">Response</span></span>
<span data-ttu-id="2e308-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2e308-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2e308-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2e308-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e308-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e308-131">Request</span></span>
<span data-ttu-id="2e308-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e308-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

### <a name="response"></a><span data-ttu-id="2e308-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e308-133">Response</span></span>
<span data-ttu-id="2e308-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e308-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




