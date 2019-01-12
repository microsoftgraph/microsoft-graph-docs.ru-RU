---
title: Список iosLobAppProvisioningConfigurationAssignments
description: Свойства списка и связей объектов iosLobAppProvisioningConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 048d48c55a387ce2ba53bdd6dca33c20611c04fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939982"
---
# <a name="list-ioslobappprovisioningconfigurationassignments"></a><span data-ttu-id="84458-103">Список iosLobAppProvisioningConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="84458-103">List iosLobAppProvisioningConfigurationAssignments</span></span>

> <span data-ttu-id="84458-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84458-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84458-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84458-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84458-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="84458-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84458-107">Свойства списка и связей объектов [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="84458-107">List properties and relationships of the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84458-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="84458-108">Prerequisites</span></span>
<span data-ttu-id="84458-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84458-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84458-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84458-111">Permission type</span></span>|<span data-ttu-id="84458-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84458-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84458-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84458-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84458-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="84458-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="84458-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84458-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84458-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84458-116">Not supported.</span></span>|
|<span data-ttu-id="84458-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84458-117">Application</span></span>|<span data-ttu-id="84458-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84458-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84458-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84458-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="84458-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84458-120">Request headers</span></span>
|<span data-ttu-id="84458-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84458-121">Header</span></span>|<span data-ttu-id="84458-122">Значение</span><span class="sxs-lookup"><span data-stu-id="84458-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84458-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84458-123">Authorization</span></span>|<span data-ttu-id="84458-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="84458-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84458-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84458-125">Accept</span></span>|<span data-ttu-id="84458-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84458-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84458-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84458-127">Request body</span></span>
<span data-ttu-id="84458-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84458-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84458-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="84458-129">Response</span></span>
<span data-ttu-id="84458-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="84458-130">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84458-131">Пример</span><span class="sxs-lookup"><span data-stu-id="84458-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="84458-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="84458-132">Request</span></span>
<span data-ttu-id="84458-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84458-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="84458-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="84458-134">Response</span></span>
<span data-ttu-id="84458-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="84458-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
      "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





