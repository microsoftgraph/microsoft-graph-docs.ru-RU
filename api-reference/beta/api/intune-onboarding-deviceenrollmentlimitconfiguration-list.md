---
title: Перечисление объектов deviceEnrollmentLimitConfiguration
description: Список свойств и связей объектов deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d16e262b905cf290069d7dab1778db6f50f51354
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978818"
---
# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="e0e04-103">Перечисление объектов deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0e04-103">List deviceEnrollmentLimitConfigurations</span></span>

> <span data-ttu-id="e0e04-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e0e04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0e04-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0e04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0e04-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e0e04-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0e04-107">Список свойств и связей объектов [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0e04-107">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0e04-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e0e04-108">Prerequisites</span></span>
<span data-ttu-id="e0e04-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0e04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0e04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0e04-111">Permission type</span></span>|<span data-ttu-id="e0e04-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0e04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0e04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0e04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0e04-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0e04-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e0e04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0e04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0e04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0e04-116">Not supported.</span></span>|
|<span data-ttu-id="e0e04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0e04-117">Application</span></span>|<span data-ttu-id="e0e04-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0e04-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0e04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0e04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e0e04-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0e04-120">Request headers</span></span>
|<span data-ttu-id="e0e04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0e04-121">Header</span></span>|<span data-ttu-id="e0e04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e0e04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0e04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0e04-123">Authorization</span></span>|<span data-ttu-id="e0e04-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e0e04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0e04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0e04-125">Accept</span></span>|<span data-ttu-id="e0e04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0e04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0e04-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0e04-127">Request body</span></span>
<span data-ttu-id="e0e04-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e0e04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0e04-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0e04-129">Response</span></span>
<span data-ttu-id="e0e04-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e0e04-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0e04-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e0e04-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0e04-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0e04-132">Request</span></span>
<span data-ttu-id="e0e04-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0e04-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="e0e04-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0e04-134">Response</span></span>
<span data-ttu-id="e0e04-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e0e04-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 446

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
      "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "limit": 5
    }
  ]
}
```





