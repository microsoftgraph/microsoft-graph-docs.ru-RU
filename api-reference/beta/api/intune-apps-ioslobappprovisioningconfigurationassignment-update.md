---
title: Обновление iosLobAppProvisioningConfigurationAssignment
description: Обновление свойства объекта iosLobAppProvisioningConfigurationAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f80f07feb9027054b5b88f1fa4fdcf868e0b3f84
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397619"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="fa59d-103">Обновление iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="fa59d-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="fa59d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa59d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fa59d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa59d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa59d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa59d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa59d-107">Обновление свойства объекта [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fa59d-107">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa59d-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="fa59d-108">Prerequisites</span></span>
<span data-ttu-id="fa59d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa59d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fa59d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa59d-111">Permission type</span></span>|<span data-ttu-id="fa59d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa59d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa59d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa59d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa59d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa59d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fa59d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa59d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa59d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa59d-116">Not supported.</span></span>|
|<span data-ttu-id="fa59d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa59d-117">Application</span></span>|<span data-ttu-id="fa59d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa59d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa59d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa59d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="fa59d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa59d-120">Request headers</span></span>
|<span data-ttu-id="fa59d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa59d-121">Header</span></span>|<span data-ttu-id="fa59d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fa59d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa59d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa59d-123">Authorization</span></span>|<span data-ttu-id="fa59d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fa59d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa59d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa59d-125">Accept</span></span>|<span data-ttu-id="fa59d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa59d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa59d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa59d-127">Request body</span></span>
<span data-ttu-id="fa59d-128">В тексте запроса укажите представление JSON для объекта [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fa59d-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="fa59d-129">В следующей таблице показаны свойства, которые необходимы для создания [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fa59d-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="fa59d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa59d-130">Property</span></span>|<span data-ttu-id="fa59d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fa59d-131">Type</span></span>|<span data-ttu-id="fa59d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fa59d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa59d-133">id</span><span class="sxs-lookup"><span data-stu-id="fa59d-133">id</span></span>|<span data-ttu-id="fa59d-134">String</span><span class="sxs-lookup"><span data-stu-id="fa59d-134">String</span></span>|<span data-ttu-id="fa59d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fa59d-135">Key of the entity.</span></span>|
|<span data-ttu-id="fa59d-136">target</span><span class="sxs-lookup"><span data-stu-id="fa59d-136">target</span></span>|[<span data-ttu-id="fa59d-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fa59d-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fa59d-138">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="fa59d-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="fa59d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa59d-139">Response</span></span>
<span data-ttu-id="fa59d-140">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fa59d-140">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa59d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="fa59d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa59d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa59d-142">Request</span></span>
<span data-ttu-id="fa59d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa59d-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fa59d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa59d-144">Response</span></span>
<span data-ttu-id="fa59d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fa59d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




