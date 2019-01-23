---
title: Создание mobileAppProvisioningConfigGroupAssignment
description: Создание нового объекта mobileAppProvisioningConfigGroupAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 50b93e4858a7f986f5ebd25e8d2b09e204bae986
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417436"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="d74c7-103">Создание mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="d74c7-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="d74c7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d74c7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d74c7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d74c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d74c7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d74c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d74c7-107">Создание нового объекта [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d74c7-107">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d74c7-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="d74c7-108">Prerequisites</span></span>
<span data-ttu-id="d74c7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d74c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d74c7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d74c7-111">Permission type</span></span>|<span data-ttu-id="d74c7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d74c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d74c7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d74c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d74c7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d74c7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d74c7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d74c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d74c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d74c7-116">Not supported.</span></span>|
|<span data-ttu-id="d74c7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d74c7-117">Application</span></span>|<span data-ttu-id="d74c7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d74c7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d74c7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d74c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="d74c7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d74c7-120">Request headers</span></span>
|<span data-ttu-id="d74c7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d74c7-121">Header</span></span>|<span data-ttu-id="d74c7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d74c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d74c7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d74c7-123">Authorization</span></span>|<span data-ttu-id="d74c7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d74c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d74c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d74c7-125">Accept</span></span>|<span data-ttu-id="d74c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d74c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d74c7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d74c7-127">Request body</span></span>
<span data-ttu-id="d74c7-128">В тексте запроса укажите представление JSON для объекта mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="d74c7-128">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="d74c7-129">В следующей таблице показаны свойства, которые необходимы для создания mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="d74c7-129">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="d74c7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d74c7-130">Property</span></span>|<span data-ttu-id="d74c7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d74c7-131">Type</span></span>|<span data-ttu-id="d74c7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d74c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d74c7-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="d74c7-133">targetGroupId</span></span>|<span data-ttu-id="d74c7-134">String</span><span class="sxs-lookup"><span data-stu-id="d74c7-134">String</span></span>|<span data-ttu-id="d74c7-135">Идентификатор группы AAD целевого приложения подготовки конфигурации.</span><span class="sxs-lookup"><span data-stu-id="d74c7-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="d74c7-136">id</span><span class="sxs-lookup"><span data-stu-id="d74c7-136">id</span></span>|<span data-ttu-id="d74c7-137">String</span><span class="sxs-lookup"><span data-stu-id="d74c7-137">String</span></span>|<span data-ttu-id="d74c7-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d74c7-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="d74c7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d74c7-139">Response</span></span>
<span data-ttu-id="d74c7-140">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d74c7-140">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d74c7-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d74c7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d74c7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d74c7-142">Request</span></span>
<span data-ttu-id="d74c7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d74c7-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="d74c7-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d74c7-144">Response</span></span>
<span data-ttu-id="d74c7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d74c7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```




