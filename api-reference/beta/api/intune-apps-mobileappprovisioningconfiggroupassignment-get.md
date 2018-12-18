---
title: Получение mobileAppProvisioningConfigGroupAssignment
description: Чтение свойства и связи объекта mobileAppProvisioningConfigGroupAssignment.
author: tfitzmac
ms.openlocfilehash: 836e1897e9ff38ef3ca3ef5c1ae55e8874897caa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330872"
---
# <a name="get-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="f4985-103">Получение mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f4985-103">Get mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="f4985-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f4985-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4985-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4985-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4985-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f4985-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4985-107">Чтение свойства и связи объекта [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f4985-107">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f4985-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f4985-108">Prerequisites</span></span>
<span data-ttu-id="f4985-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4985-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4985-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4985-111">Permission type</span></span>|<span data-ttu-id="f4985-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4985-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4985-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4985-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4985-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4985-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f4985-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4985-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4985-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4985-116">Not supported.</span></span>|
|<span data-ttu-id="f4985-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4985-117">Application</span></span>|<span data-ttu-id="f4985-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4985-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4985-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4985-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4985-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f4985-120">Optional query parameters</span></span>
<span data-ttu-id="f4985-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f4985-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f4985-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4985-122">Request headers</span></span>
|<span data-ttu-id="f4985-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4985-123">Header</span></span>|<span data-ttu-id="f4985-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f4985-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4985-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4985-125">Authorization</span></span>|<span data-ttu-id="f4985-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f4985-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4985-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f4985-127">Accept</span></span>|<span data-ttu-id="f4985-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f4985-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4985-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4985-129">Request body</span></span>
<span data-ttu-id="f4985-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4985-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4985-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4985-131">Response</span></span>
<span data-ttu-id="f4985-132">Успешно завершена, этот метод возвращает `200 OK` объект [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f4985-132">If successful, this method returns a `200 OK` response code and [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4985-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f4985-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4985-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4985-134">Request</span></span>
<span data-ttu-id="f4985-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4985-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="f4985-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4985-136">Response</span></span>
<span data-ttu-id="f4985-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f4985-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 203

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
    "targetGroupId": "Target Group Id value",
    "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
  }
}
```





