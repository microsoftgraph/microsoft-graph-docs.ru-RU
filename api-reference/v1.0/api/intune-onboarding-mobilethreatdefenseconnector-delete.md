---
title: Удаление объекта mobileThreatDefenseConnector
description: Удаляет объект mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf42335b51231de73657f433506c5e5748b1a553
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976742"
---
# <a name="delete-mobilethreatdefenseconnector"></a><span data-ttu-id="9f1a9-103">Удаление объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="9f1a9-103">Delete mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="9f1a9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f1a9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f1a9-105">Удаляет объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="9f1a9-105">Deletes a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f1a9-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f1a9-106">Prerequisites</span></span>
<span data-ttu-id="9f1a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f1a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f1a9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f1a9-109">Permission type</span></span>|<span data-ttu-id="9f1a9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f1a9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f1a9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f1a9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f1a9-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f1a9-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9f1a9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f1a9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f1a9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f1a9-114">Not supported.</span></span>|
|<span data-ttu-id="9f1a9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f1a9-115">Application</span></span>|<span data-ttu-id="9f1a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f1a9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f1a9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f1a9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="9f1a9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f1a9-118">Request headers</span></span>
|<span data-ttu-id="9f1a9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f1a9-119">Header</span></span>|<span data-ttu-id="9f1a9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9f1a9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f1a9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f1a9-121">Authorization</span></span>|<span data-ttu-id="9f1a9-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f1a9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f1a9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9f1a9-123">Accept</span></span>|<span data-ttu-id="9f1a9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9f1a9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f1a9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f1a9-125">Request body</span></span>
<span data-ttu-id="9f1a9-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f1a9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f1a9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f1a9-127">Response</span></span>
<span data-ttu-id="9f1a9-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9f1a9-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9f1a9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9f1a9-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f1a9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f1a9-130">Request</span></span>
<span data-ttu-id="9f1a9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f1a9-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="9f1a9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f1a9-132">Response</span></span>
<span data-ttu-id="9f1a9-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f1a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



