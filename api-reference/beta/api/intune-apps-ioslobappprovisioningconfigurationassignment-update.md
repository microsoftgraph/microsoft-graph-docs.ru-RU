---
title: Обновление Иослобапппровисионингконфигуратионассигнмент
description: Обновление свойств объекта Иослобапппровисионингконфигуратионассигнмент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9ca12e3d799c666ad7b61d9a0aa400ae2b566ca
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171395"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="ce431-103">Обновление Иослобапппровисионингконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="ce431-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="ce431-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce431-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce431-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce431-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce431-106">Обновление свойств объекта [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ce431-106">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce431-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ce431-107">Prerequisites</span></span>
<span data-ttu-id="ce431-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce431-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ce431-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce431-110">Permission type</span></span>|<span data-ttu-id="ce431-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce431-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce431-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce431-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce431-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce431-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce431-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce431-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce431-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce431-115">Not supported.</span></span>|
|<span data-ttu-id="ce431-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce431-116">Application</span></span>|<span data-ttu-id="ce431-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce431-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce431-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce431-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ce431-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce431-119">Request headers</span></span>
|<span data-ttu-id="ce431-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce431-120">Header</span></span>|<span data-ttu-id="ce431-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ce431-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce431-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce431-122">Authorization</span></span>|<span data-ttu-id="ce431-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ce431-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce431-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ce431-124">Accept</span></span>|<span data-ttu-id="ce431-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce431-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce431-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce431-126">Request body</span></span>
<span data-ttu-id="ce431-127">В тексте запроса добавьте представление объекта [Иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce431-127">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="ce431-128">В следующей таблице приведены свойства, необходимые при создании [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ce431-128">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="ce431-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce431-129">Property</span></span>|<span data-ttu-id="ce431-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ce431-130">Type</span></span>|<span data-ttu-id="ce431-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ce431-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce431-132">id</span><span class="sxs-lookup"><span data-stu-id="ce431-132">id</span></span>|<span data-ttu-id="ce431-133">String</span><span class="sxs-lookup"><span data-stu-id="ce431-133">String</span></span>|<span data-ttu-id="ce431-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ce431-134">Key of the entity.</span></span>|
|<span data-ttu-id="ce431-135">target</span><span class="sxs-lookup"><span data-stu-id="ce431-135">target</span></span>|[<span data-ttu-id="ce431-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ce431-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ce431-137">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="ce431-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="ce431-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce431-138">Response</span></span>
<span data-ttu-id="ce431-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce431-139">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce431-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ce431-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce431-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce431-141">Request</span></span>
<span data-ttu-id="ce431-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce431-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ce431-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce431-143">Response</span></span>
<span data-ttu-id="ce431-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce431-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




