---
title: Перечисление объектов managedMobileApp
description: Список свойств и связей объектов managedMobileApp.
ms.openlocfilehash: 6ad8bd219e810c0ee276a9aa02de782acba3b563
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076531"
---
# <a name="list-managedmobileapps"></a><span data-ttu-id="21903-103">Перечисление объектов managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="21903-103">List managedMobileApps</span></span>

> <span data-ttu-id="21903-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="21903-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21903-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21903-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21903-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="21903-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21903-107">Список свойств и связей объектов [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21903-107">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21903-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="21903-108">Prerequisites</span></span>
<span data-ttu-id="21903-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21903-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21903-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21903-111">Permission type</span></span>|<span data-ttu-id="21903-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21903-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21903-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21903-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21903-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="21903-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="21903-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21903-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21903-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21903-116">Not supported.</span></span>|
|<span data-ttu-id="21903-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21903-117">Application</span></span>|<span data-ttu-id="21903-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21903-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21903-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21903-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="21903-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21903-120">Request headers</span></span>
|<span data-ttu-id="21903-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21903-121">Header</span></span>|<span data-ttu-id="21903-122">Значение</span><span class="sxs-lookup"><span data-stu-id="21903-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21903-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21903-123">Authorization</span></span>|<span data-ttu-id="21903-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="21903-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21903-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21903-125">Accept</span></span>|<span data-ttu-id="21903-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21903-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21903-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21903-127">Request body</span></span>
<span data-ttu-id="21903-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21903-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21903-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="21903-129">Response</span></span>
<span data-ttu-id="21903-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="21903-130">If successful, this method returns a `200 OK` response code and a collection of [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21903-131">Пример</span><span class="sxs-lookup"><span data-stu-id="21903-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="21903-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="21903-132">Request</span></span>
<span data-ttu-id="21903-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21903-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
```

### <a name="response"></a><span data-ttu-id="21903-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="21903-134">Response</span></span>
<span data-ttu-id="21903-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="21903-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```





