---
title: Перечисление объектов managedAppConfiguration
description: Список свойств и связей объектов managedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f9028ca08a11d17839a7d9292b4473ea8a7179f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875007"
---
# <a name="list-managedappconfigurations"></a><span data-ttu-id="1af72-103">Перечисление объектов managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1af72-103">List managedAppConfigurations</span></span>

> <span data-ttu-id="1af72-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1af72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1af72-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1af72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1af72-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1af72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1af72-107">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1af72-107">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1af72-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1af72-108">Prerequisites</span></span>
<span data-ttu-id="1af72-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1af72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1af72-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1af72-111">Permission type</span></span>|<span data-ttu-id="1af72-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1af72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1af72-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1af72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1af72-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1af72-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1af72-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1af72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1af72-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1af72-116">Not supported.</span></span>|
|<span data-ttu-id="1af72-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1af72-117">Application</span></span>|<span data-ttu-id="1af72-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1af72-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1af72-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1af72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="1af72-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1af72-120">Request headers</span></span>
|<span data-ttu-id="1af72-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1af72-121">Header</span></span>|<span data-ttu-id="1af72-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1af72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1af72-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1af72-123">Authorization</span></span>|<span data-ttu-id="1af72-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1af72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1af72-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1af72-125">Accept</span></span>|<span data-ttu-id="1af72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1af72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1af72-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1af72-127">Request body</span></span>
<span data-ttu-id="1af72-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1af72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1af72-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1af72-129">Response</span></span>
<span data-ttu-id="1af72-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1af72-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1af72-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1af72-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1af72-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1af72-132">Request</span></span>
<span data-ttu-id="1af72-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1af72-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="1af72-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1af72-134">Response</span></span>
<span data-ttu-id="1af72-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1af72-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppConfiguration",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "2ed27cb5-7cb5-2ed2-b57c-d22eb57cd22e",
      "version": "Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```





