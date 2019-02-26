---
title: Удаление managedDeviceMobileAppConfigurationDeviceStatus
description: Удаляет объект managedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eedec45296884829a476cd5a8acc051d6af62d6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264150"
---
# <a name="delete-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="b4b99-103">Удаление managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b4b99-103">Delete managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="b4b99-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4b99-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4b99-105">Удаляет объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b4b99-105">Deletes a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4b99-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b4b99-106">Prerequisites</span></span>
<span data-ttu-id="b4b99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4b99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b4b99-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4b99-109">Permission type</span></span>|<span data-ttu-id="b4b99-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4b99-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4b99-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4b99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b4b99-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4b99-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4b99-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4b99-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4b99-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4b99-114">Not supported.</span></span>|
|<span data-ttu-id="b4b99-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4b99-115">Application</span></span>|<span data-ttu-id="b4b99-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4b99-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4b99-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4b99-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b4b99-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4b99-118">Request headers</span></span>
|<span data-ttu-id="b4b99-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4b99-119">Header</span></span>|<span data-ttu-id="b4b99-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b4b99-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4b99-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4b99-121">Authorization</span></span>|<span data-ttu-id="b4b99-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b4b99-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4b99-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b4b99-123">Accept</span></span>|<span data-ttu-id="b4b99-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b4b99-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4b99-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4b99-125">Request body</span></span>
<span data-ttu-id="b4b99-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4b99-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4b99-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4b99-127">Response</span></span>
<span data-ttu-id="b4b99-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b4b99-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4b99-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b4b99-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4b99-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4b99-130">Request</span></span>
<span data-ttu-id="b4b99-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4b99-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="b4b99-132">Отклик
</span><span class="sxs-lookup"><span data-stu-id="b4b99-132">Response</span></span>
<span data-ttu-id="b4b99-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b4b99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



