---
title: Получение iosLobAppProvisioningConfigurationAssignment
description: Чтение свойства и связи объекта iosLobAppProvisioningConfigurationAssignment.
ms.openlocfilehash: d2eb5ae3f68395bb4c33b7ec5f760e1f49cef5a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079279"
---
# <a name="get-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="7306d-103">Получение iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7306d-103">Get iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="7306d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7306d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7306d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7306d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7306d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7306d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7306d-107">Чтение свойства и связи объекта [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7306d-107">Read properties and relationships of the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7306d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7306d-108">Prerequisites</span></span>
<span data-ttu-id="7306d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7306d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7306d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7306d-111">Permission type</span></span>|<span data-ttu-id="7306d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7306d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7306d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7306d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7306d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7306d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7306d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7306d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7306d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7306d-116">Not supported.</span></span>|
|<span data-ttu-id="7306d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7306d-117">Application</span></span>|<span data-ttu-id="7306d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7306d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7306d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7306d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7306d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7306d-120">Optional query parameters</span></span>
<span data-ttu-id="7306d-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7306d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7306d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7306d-122">Request headers</span></span>
|<span data-ttu-id="7306d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7306d-123">Header</span></span>|<span data-ttu-id="7306d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7306d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7306d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7306d-125">Authorization</span></span>|<span data-ttu-id="7306d-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7306d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7306d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7306d-127">Accept</span></span>|<span data-ttu-id="7306d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7306d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7306d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7306d-129">Request body</span></span>
<span data-ttu-id="7306d-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7306d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7306d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7306d-131">Response</span></span>
<span data-ttu-id="7306d-132">Успешно завершена, этот метод возвращает `200 OK` объект [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7306d-132">If successful, this method returns a `200 OK` response code and [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7306d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7306d-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="7306d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7306d-134">Request</span></span>
<span data-ttu-id="7306d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7306d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="7306d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7306d-136">Response</span></span>
<span data-ttu-id="7306d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7306d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
    "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```





