---
title: Создание iosLobAppProvisioningConfigurationAssignment
description: Создание нового объекта iosLobAppProvisioningConfigurationAssignment.
ms.openlocfilehash: 5d3a51aab8560e4922d74e48675aa95c25be5c72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075256"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="0a6d1-103">Создание iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0a6d1-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="0a6d1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a6d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a6d1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a6d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a6d1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0a6d1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a6d1-107">Создание нового объекта [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="0a6d1-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a6d1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0a6d1-108">Prerequisites</span></span>
<span data-ttu-id="0a6d1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a6d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a6d1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a6d1-111">Permission type</span></span>|<span data-ttu-id="0a6d1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a6d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a6d1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a6d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a6d1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a6d1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0a6d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a6d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a6d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a6d1-116">Not supported.</span></span>|
|<span data-ttu-id="0a6d1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a6d1-117">Application</span></span>|<span data-ttu-id="0a6d1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a6d1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a6d1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a6d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0a6d1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a6d1-120">Request headers</span></span>
|<span data-ttu-id="0a6d1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a6d1-121">Header</span></span>|<span data-ttu-id="0a6d1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0a6d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a6d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a6d1-123">Authorization</span></span>|<span data-ttu-id="0a6d1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0a6d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a6d1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a6d1-125">Accept</span></span>|<span data-ttu-id="0a6d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a6d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a6d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a6d1-127">Request body</span></span>
<span data-ttu-id="0a6d1-128">В тексте запроса укажите представление JSON для объекта iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="0a6d1-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="0a6d1-129">В следующей таблице показаны свойства, которые необходимы для создания iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="0a6d1-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="0a6d1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a6d1-130">Property</span></span>|<span data-ttu-id="0a6d1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0a6d1-131">Type</span></span>|<span data-ttu-id="0a6d1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0a6d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a6d1-133">id</span><span class="sxs-lookup"><span data-stu-id="0a6d1-133">id</span></span>|<span data-ttu-id="0a6d1-134">String</span><span class="sxs-lookup"><span data-stu-id="0a6d1-134">String</span></span>|<span data-ttu-id="0a6d1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0a6d1-135">Key of the entity.</span></span>|
|<span data-ttu-id="0a6d1-136">target</span><span class="sxs-lookup"><span data-stu-id="0a6d1-136">target</span></span>|[<span data-ttu-id="0a6d1-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0a6d1-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0a6d1-138">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="0a6d1-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="0a6d1-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a6d1-139">Response</span></span>
<span data-ttu-id="0a6d1-140">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0a6d1-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a6d1-141">Пример</span><span class="sxs-lookup"><span data-stu-id="0a6d1-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a6d1-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a6d1-142">Request</span></span>
<span data-ttu-id="0a6d1-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a6d1-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0a6d1-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a6d1-144">Response</span></span>
<span data-ttu-id="0a6d1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0a6d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





