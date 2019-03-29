---
title: Перечисление объектов managedDeviceMobileAppConfigurationAssignment
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: edaf791c95839a43a37a52a30dfe97e8550b2fb2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983192"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="90ad5-103">Перечисление объектов managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="90ad5-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

> <span data-ttu-id="90ad5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ad5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90ad5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90ad5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90ad5-106">Список свойств и связей объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="90ad5-106">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90ad5-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="90ad5-107">Prerequisites</span></span>
<span data-ttu-id="90ad5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90ad5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90ad5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90ad5-110">Permission type</span></span>|<span data-ttu-id="90ad5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90ad5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90ad5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90ad5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90ad5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="90ad5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="90ad5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90ad5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90ad5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ad5-115">Not supported.</span></span>|
|<span data-ttu-id="90ad5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90ad5-116">Application</span></span>|<span data-ttu-id="90ad5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ad5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90ad5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90ad5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="90ad5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90ad5-119">Request headers</span></span>
|<span data-ttu-id="90ad5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90ad5-120">Header</span></span>|<span data-ttu-id="90ad5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="90ad5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90ad5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90ad5-122">Authorization</span></span>|<span data-ttu-id="90ad5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90ad5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90ad5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="90ad5-124">Accept</span></span>|<span data-ttu-id="90ad5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90ad5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90ad5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90ad5-126">Request body</span></span>
<span data-ttu-id="90ad5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90ad5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90ad5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="90ad5-128">Response</span></span>
<span data-ttu-id="90ad5-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90ad5-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90ad5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="90ad5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="90ad5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="90ad5-131">Request</span></span>
<span data-ttu-id="90ad5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90ad5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="90ad5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="90ad5-133">Response</span></span>
<span data-ttu-id="90ad5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90ad5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




