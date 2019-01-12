---
title: Перечисление объектов windows10SecureAssessmentConfiguration
description: Список свойств и связей объектов windows10SecureAssessmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f5fce067d9e0fbba58395ed05138d253fe5d6d8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955690"
---
# <a name="list-windows10secureassessmentconfigurations"></a><span data-ttu-id="05bee-103">Перечисление объектов windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="05bee-103">List windows10SecureAssessmentConfigurations</span></span>

> <span data-ttu-id="05bee-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="05bee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05bee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05bee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05bee-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="05bee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05bee-107">Список свойств и связей объектов [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05bee-107">List properties and relationships of the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05bee-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="05bee-108">Prerequisites</span></span>
<span data-ttu-id="05bee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05bee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05bee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05bee-111">Permission type</span></span>|<span data-ttu-id="05bee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05bee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05bee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05bee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05bee-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="05bee-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="05bee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05bee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05bee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05bee-116">Not supported.</span></span>|
|<span data-ttu-id="05bee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05bee-117">Application</span></span>|<span data-ttu-id="05bee-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05bee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05bee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05bee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="05bee-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05bee-120">Request headers</span></span>
|<span data-ttu-id="05bee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05bee-121">Header</span></span>|<span data-ttu-id="05bee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="05bee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05bee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05bee-123">Authorization</span></span>|<span data-ttu-id="05bee-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="05bee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05bee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05bee-125">Accept</span></span>|<span data-ttu-id="05bee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05bee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05bee-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05bee-127">Request body</span></span>
<span data-ttu-id="05bee-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05bee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05bee-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="05bee-129">Response</span></span>
<span data-ttu-id="05bee-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="05bee-130">If successful, this method returns a `200 OK` response code and a collection of [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05bee-131">Пример</span><span class="sxs-lookup"><span data-stu-id="05bee-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="05bee-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="05bee-132">Request</span></span>
<span data-ttu-id="05bee-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05bee-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="05bee-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="05bee-134">Response</span></span>
<span data-ttu-id="05bee-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="05bee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





