---
title: Создание Иослобапппровисионингконфигуратионассигнмент
description: Создание нового объекта Иослобапппровисионингконфигуратионассигнмент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68005d3f8682b61417a9b1a768b62a8ff5cf235e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32496088"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="a229b-103">Создание Иослобапппровисионингконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="a229b-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="a229b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a229b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a229b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a229b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a229b-106">Создание нового объекта [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a229b-106">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a229b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a229b-107">Prerequisites</span></span>
<span data-ttu-id="a229b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a229b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a229b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a229b-110">Permission type</span></span>|<span data-ttu-id="a229b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a229b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a229b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a229b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a229b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a229b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a229b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a229b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a229b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a229b-115">Not supported.</span></span>|
|<span data-ttu-id="a229b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a229b-116">Application</span></span>|<span data-ttu-id="a229b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a229b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a229b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a229b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a229b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a229b-119">Request headers</span></span>
|<span data-ttu-id="a229b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a229b-120">Header</span></span>|<span data-ttu-id="a229b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a229b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a229b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a229b-122">Authorization</span></span>|<span data-ttu-id="a229b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a229b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a229b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a229b-124">Accept</span></span>|<span data-ttu-id="a229b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a229b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a229b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a229b-126">Request body</span></span>
<span data-ttu-id="a229b-127">В тексте запроса добавьте представление объекта Иослобапппровисионингконфигуратионассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a229b-127">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="a229b-128">В следующей таблице приведены свойства, необходимые при создании Иослобапппровисионингконфигуратионассигнмент.</span><span class="sxs-lookup"><span data-stu-id="a229b-128">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="a229b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a229b-129">Property</span></span>|<span data-ttu-id="a229b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a229b-130">Type</span></span>|<span data-ttu-id="a229b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a229b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a229b-132">id</span><span class="sxs-lookup"><span data-stu-id="a229b-132">id</span></span>|<span data-ttu-id="a229b-133">String</span><span class="sxs-lookup"><span data-stu-id="a229b-133">String</span></span>|<span data-ttu-id="a229b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a229b-134">Key of the entity.</span></span>|
|<span data-ttu-id="a229b-135">target</span><span class="sxs-lookup"><span data-stu-id="a229b-135">target</span></span>|[<span data-ttu-id="a229b-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a229b-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a229b-137">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="a229b-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="a229b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a229b-138">Response</span></span>
<span data-ttu-id="a229b-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a229b-139">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a229b-140">Пример</span><span class="sxs-lookup"><span data-stu-id="a229b-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a229b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a229b-141">Request</span></span>
<span data-ttu-id="a229b-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a229b-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a229b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a229b-143">Response</span></span>
<span data-ttu-id="a229b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a229b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





