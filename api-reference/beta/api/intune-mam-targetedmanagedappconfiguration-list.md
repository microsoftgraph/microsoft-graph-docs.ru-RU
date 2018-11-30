---
title: Перечисление объектов targetedManagedAppConfiguration
description: Список свойств и связей объектов targetedManagedAppConfiguration.
ms.openlocfilehash: d3d943285604e8fc6764479059935caa73fddfc1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079191"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="7eb58-103">Перечисление объектов targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7eb58-103">List targetedManagedAppConfigurations</span></span>

> <span data-ttu-id="7eb58-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7eb58-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7eb58-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7eb58-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7eb58-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7eb58-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7eb58-107">Список свойств и связей объектов [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7eb58-107">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7eb58-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7eb58-108">Prerequisites</span></span>
<span data-ttu-id="7eb58-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7eb58-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7eb58-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7eb58-111">Permission type</span></span>|<span data-ttu-id="7eb58-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7eb58-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7eb58-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7eb58-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7eb58-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7eb58-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7eb58-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7eb58-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7eb58-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7eb58-116">Not supported.</span></span>|
|<span data-ttu-id="7eb58-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7eb58-117">Application</span></span>|<span data-ttu-id="7eb58-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7eb58-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7eb58-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7eb58-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7eb58-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7eb58-120">Request headers</span></span>
|<span data-ttu-id="7eb58-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7eb58-121">Header</span></span>|<span data-ttu-id="7eb58-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7eb58-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7eb58-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7eb58-123">Authorization</span></span>|<span data-ttu-id="7eb58-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7eb58-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7eb58-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7eb58-125">Accept</span></span>|<span data-ttu-id="7eb58-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7eb58-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7eb58-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7eb58-127">Request body</span></span>
<span data-ttu-id="7eb58-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7eb58-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7eb58-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7eb58-129">Response</span></span>
<span data-ttu-id="7eb58-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7eb58-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7eb58-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7eb58-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7eb58-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7eb58-132">Request</span></span>
<span data-ttu-id="7eb58-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7eb58-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="7eb58-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="7eb58-134">Response</span></span>
<span data-ttu-id="7eb58-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7eb58-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 657

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "2444e029-e029-2444-29e0-442429e04424",
      "version": "Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "isAssigned": true
    }
  ]
}
```





