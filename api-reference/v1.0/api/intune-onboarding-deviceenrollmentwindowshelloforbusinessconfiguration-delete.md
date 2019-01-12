---
title: Удаление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Удаляет объект deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c2c6592f716a3c8c5a8dc4a8c2b3a4ec4c58184f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920851"
---
# <a name="delete-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="8d0b3-103">Удаление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d0b3-103">Delete deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="8d0b3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8d0b3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d0b3-105">Удаляет объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d0b3-105">Deletes a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d0b3-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d0b3-106">Prerequisites</span></span>
<span data-ttu-id="8d0b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d0b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d0b3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d0b3-109">Permission type</span></span>|<span data-ttu-id="8d0b3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d0b3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d0b3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d0b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8d0b3-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d0b3-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8d0b3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d0b3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d0b3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d0b3-114">Not supported.</span></span>|
|<span data-ttu-id="8d0b3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d0b3-115">Application</span></span>|<span data-ttu-id="8d0b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d0b3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d0b3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d0b3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8d0b3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d0b3-118">Request headers</span></span>
|<span data-ttu-id="8d0b3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d0b3-119">Header</span></span>|<span data-ttu-id="8d0b3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8d0b3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d0b3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d0b3-121">Authorization</span></span>|<span data-ttu-id="8d0b3-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8d0b3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d0b3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8d0b3-123">Accept</span></span>|<span data-ttu-id="8d0b3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8d0b3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d0b3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d0b3-125">Request body</span></span>
<span data-ttu-id="8d0b3-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d0b3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d0b3-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d0b3-127">Response</span></span>
<span data-ttu-id="8d0b3-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8d0b3-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8d0b3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8d0b3-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d0b3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d0b3-130">Request</span></span>
<span data-ttu-id="8d0b3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d0b3-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8d0b3-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d0b3-132">Response</span></span>
<span data-ttu-id="8d0b3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8d0b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



