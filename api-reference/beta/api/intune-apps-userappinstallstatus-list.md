---
title: Список userAppInstallStatuses
description: Свойства списка и связей объектов userAppInstallStatus.
author: tfitzmac
ms.openlocfilehash: 0aeef4d97e63c42e11fefdb84a4dfb6138fdc6a3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325426"
---
# <a name="list-userappinstallstatuses"></a><span data-ttu-id="1598b-103">Список userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="1598b-103">List userAppInstallStatuses</span></span>

> <span data-ttu-id="1598b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1598b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1598b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1598b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1598b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1598b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1598b-107">Свойства списка и связей объектов [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="1598b-107">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1598b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1598b-108">Prerequisites</span></span>
<span data-ttu-id="1598b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1598b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1598b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1598b-111">Permission type</span></span>|<span data-ttu-id="1598b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1598b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1598b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1598b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1598b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1598b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1598b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1598b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1598b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1598b-116">Not supported.</span></span>|
|<span data-ttu-id="1598b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1598b-117">Application</span></span>|<span data-ttu-id="1598b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1598b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1598b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1598b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="1598b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1598b-120">Request headers</span></span>
|<span data-ttu-id="1598b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1598b-121">Header</span></span>|<span data-ttu-id="1598b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1598b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1598b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1598b-123">Authorization</span></span>|<span data-ttu-id="1598b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1598b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1598b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1598b-125">Accept</span></span>|<span data-ttu-id="1598b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1598b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1598b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1598b-127">Request body</span></span>
<span data-ttu-id="1598b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1598b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1598b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1598b-129">Response</span></span>
<span data-ttu-id="1598b-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1598b-130">If successful, this method returns a `200 OK` response code and a collection of [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1598b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1598b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1598b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1598b-132">Request</span></span>
<span data-ttu-id="1598b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1598b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="1598b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1598b-134">Response</span></span>
<span data-ttu-id="1598b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1598b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userAppInstallStatus",
      "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```





