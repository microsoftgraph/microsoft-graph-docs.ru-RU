---
title: Перечисление объектов windows10SecureAssessmentConfiguration
description: Список свойств и связей объектов windows10SecureAssessmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 94103ff601f76a246d540cb53d8327af86f8617f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862799"
---
# <a name="list-windows10secureassessmentconfigurations"></a><span data-ttu-id="1e0d6-103">Перечисление объектов windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e0d6-103">List windows10SecureAssessmentConfigurations</span></span>

> <span data-ttu-id="1e0d6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e0d6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e0d6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e0d6-107">Список свойств и связей объектов [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e0d6-107">List properties and relationships of the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e0d6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1e0d6-108">Prerequisites</span></span>
<span data-ttu-id="1e0d6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e0d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e0d6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e0d6-111">Permission type</span></span>|<span data-ttu-id="1e0d6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e0d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e0d6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e0d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e0d6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e0d6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1e0d6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e0d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e0d6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-116">Not supported.</span></span>|
|<span data-ttu-id="1e0d6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e0d6-117">Application</span></span>|<span data-ttu-id="1e0d6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e0d6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e0d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1e0d6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e0d6-120">Request headers</span></span>
|<span data-ttu-id="1e0d6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e0d6-121">Header</span></span>|<span data-ttu-id="1e0d6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1e0d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e0d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e0d6-123">Authorization</span></span>|<span data-ttu-id="1e0d6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1e0d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e0d6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e0d6-125">Accept</span></span>|<span data-ttu-id="1e0d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e0d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e0d6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1e0d6-127">Request body</span></span>
<span data-ttu-id="1e0d6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e0d6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e0d6-129">Response</span></span>
<span data-ttu-id="1e0d6-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-130">If successful, this method returns a `200 OK` response code and a collection of [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e0d6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1e0d6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e0d6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e0d6-132">Request</span></span>
<span data-ttu-id="1e0d6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1e0d6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e0d6-134">Response</span></span>
<span data-ttu-id="1e0d6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 772

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
      "id": "f60d71be-71be-f60d-be71-0df6be710df6",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "launchUri": "Launch Uri value",
      "configurationAccount": "Configuration Account value",
      "configurationAccountType": "domainAccount",
      "allowPrinting": true,
      "allowScreenCapture": true,
      "allowTextSuggestion": true
    }
  ]
}
```





