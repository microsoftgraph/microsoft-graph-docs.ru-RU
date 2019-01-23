---
title: Создание iosLobAppProvisioningConfigurationAssignment
description: Создание нового объекта iosLobAppProvisioningConfigurationAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d1ba6130224718c7c28c02f0866ae01144f4c66
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421531"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="04fce-103">Создание iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="04fce-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="04fce-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="04fce-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04fce-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04fce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04fce-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04fce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04fce-107">Создание нового объекта [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="04fce-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04fce-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="04fce-108">Prerequisites</span></span>
<span data-ttu-id="04fce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="04fce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="04fce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04fce-111">Permission type</span></span>|<span data-ttu-id="04fce-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04fce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04fce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04fce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04fce-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04fce-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04fce-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04fce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04fce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04fce-116">Not supported.</span></span>|
|<span data-ttu-id="04fce-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04fce-117">Application</span></span>|<span data-ttu-id="04fce-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04fce-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04fce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04fce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="04fce-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04fce-120">Request headers</span></span>
|<span data-ttu-id="04fce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04fce-121">Header</span></span>|<span data-ttu-id="04fce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="04fce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04fce-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04fce-123">Authorization</span></span>|<span data-ttu-id="04fce-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="04fce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04fce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04fce-125">Accept</span></span>|<span data-ttu-id="04fce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04fce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04fce-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04fce-127">Request body</span></span>
<span data-ttu-id="04fce-128">В тексте запроса укажите представление JSON для объекта iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="04fce-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="04fce-129">В следующей таблице показаны свойства, которые необходимы для создания iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="04fce-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="04fce-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="04fce-130">Property</span></span>|<span data-ttu-id="04fce-131">Тип</span><span class="sxs-lookup"><span data-stu-id="04fce-131">Type</span></span>|<span data-ttu-id="04fce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="04fce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04fce-133">id</span><span class="sxs-lookup"><span data-stu-id="04fce-133">id</span></span>|<span data-ttu-id="04fce-134">String</span><span class="sxs-lookup"><span data-stu-id="04fce-134">String</span></span>|<span data-ttu-id="04fce-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="04fce-135">Key of the entity.</span></span>|
|<span data-ttu-id="04fce-136">target</span><span class="sxs-lookup"><span data-stu-id="04fce-136">target</span></span>|[<span data-ttu-id="04fce-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="04fce-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="04fce-138">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="04fce-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="04fce-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="04fce-139">Response</span></span>
<span data-ttu-id="04fce-140">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="04fce-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04fce-141">Пример</span><span class="sxs-lookup"><span data-stu-id="04fce-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="04fce-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="04fce-142">Request</span></span>
<span data-ttu-id="04fce-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04fce-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="04fce-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="04fce-144">Response</span></span>
<span data-ttu-id="04fce-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="04fce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




