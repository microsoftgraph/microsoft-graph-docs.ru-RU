---
title: Перечисление объектов deviceConfigurationUserStatus
description: Список свойств и связей объектов deviceConfigurationUserStatus.
author: tfitzmac
ms.openlocfilehash: e34fde4dda174927d7235d5ded4de918f142635d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316704"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="8318d-103">Перечисление объектов deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="8318d-103">List deviceConfigurationUserStatuses</span></span>

> <span data-ttu-id="8318d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8318d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8318d-105">Список свойств и связей объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="8318d-105">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8318d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8318d-106">Prerequisites</span></span>
<span data-ttu-id="8318d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8318d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8318d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8318d-109">Permission type</span></span>|<span data-ttu-id="8318d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8318d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8318d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8318d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8318d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8318d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8318d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8318d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8318d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8318d-114">Not supported.</span></span>|
|<span data-ttu-id="8318d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8318d-115">Application</span></span>|<span data-ttu-id="8318d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8318d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8318d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8318d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="8318d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8318d-118">Request headers</span></span>
|<span data-ttu-id="8318d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8318d-119">Header</span></span>|<span data-ttu-id="8318d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8318d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8318d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8318d-121">Authorization</span></span>|<span data-ttu-id="8318d-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8318d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8318d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8318d-123">Accept</span></span>|<span data-ttu-id="8318d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8318d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8318d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8318d-125">Request body</span></span>
<span data-ttu-id="8318d-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8318d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8318d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8318d-127">Response</span></span>
<span data-ttu-id="8318d-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8318d-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8318d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8318d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8318d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8318d-130">Request</span></span>
<span data-ttu-id="8318d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8318d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="8318d-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="8318d-132">Response</span></span>
<span data-ttu-id="8318d-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8318d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
      "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



