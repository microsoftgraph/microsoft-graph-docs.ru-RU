---
title: Перечисление объектов targetedManagedAppConfiguration
description: Список свойств и связей объектов targetedManagedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d58516c9e6b72f8412f3a75be53092f18b9fe2f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970011"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="7870b-103">Перечисление объектов targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7870b-103">List targetedManagedAppConfigurations</span></span>

> <span data-ttu-id="7870b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7870b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7870b-105">Список свойств и связей объектов [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7870b-105">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7870b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7870b-106">Prerequisites</span></span>
<span data-ttu-id="7870b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7870b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7870b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7870b-109">Permission type</span></span>|<span data-ttu-id="7870b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7870b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7870b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7870b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7870b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7870b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7870b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7870b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7870b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7870b-114">Not supported.</span></span>|
|<span data-ttu-id="7870b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7870b-115">Application</span></span>|<span data-ttu-id="7870b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7870b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7870b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7870b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7870b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7870b-118">Request headers</span></span>
|<span data-ttu-id="7870b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7870b-119">Header</span></span>|<span data-ttu-id="7870b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7870b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7870b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7870b-121">Authorization</span></span>|<span data-ttu-id="7870b-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7870b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7870b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7870b-123">Accept</span></span>|<span data-ttu-id="7870b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7870b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7870b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7870b-125">Request body</span></span>
<span data-ttu-id="7870b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7870b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7870b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7870b-127">Response</span></span>
<span data-ttu-id="7870b-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7870b-128">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7870b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7870b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7870b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7870b-130">Request</span></span>
<span data-ttu-id="7870b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7870b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="7870b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7870b-132">Response</span></span>
<span data-ttu-id="7870b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7870b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



