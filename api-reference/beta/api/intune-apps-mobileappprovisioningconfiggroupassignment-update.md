---
title: Обновление mobileAppProvisioningConfigGroupAssignment
description: Обновление свойства объекта mobileAppProvisioningConfigGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b341de06c1bd5d504e4835ebef8fce2aa3a5aac7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848344"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="3acf1-103">Обновление mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3acf1-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="3acf1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3acf1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3acf1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3acf1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3acf1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3acf1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3acf1-107">Обновление свойства объекта [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3acf1-107">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3acf1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3acf1-108">Prerequisites</span></span>
<span data-ttu-id="3acf1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3acf1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3acf1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3acf1-111">Permission type</span></span>|<span data-ttu-id="3acf1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3acf1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3acf1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3acf1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3acf1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3acf1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3acf1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3acf1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3acf1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3acf1-116">Not supported.</span></span>|
|<span data-ttu-id="3acf1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3acf1-117">Application</span></span>|<span data-ttu-id="3acf1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3acf1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3acf1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3acf1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3acf1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3acf1-120">Request headers</span></span>
|<span data-ttu-id="3acf1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3acf1-121">Header</span></span>|<span data-ttu-id="3acf1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3acf1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3acf1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3acf1-123">Authorization</span></span>|<span data-ttu-id="3acf1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3acf1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3acf1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3acf1-125">Accept</span></span>|<span data-ttu-id="3acf1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3acf1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3acf1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3acf1-127">Request body</span></span>
<span data-ttu-id="3acf1-128">В тексте запроса укажите представление JSON для объекта [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3acf1-128">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="3acf1-129">В следующей таблице показаны свойства, которые необходимы для создания [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3acf1-129">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="3acf1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3acf1-130">Property</span></span>|<span data-ttu-id="3acf1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3acf1-131">Type</span></span>|<span data-ttu-id="3acf1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3acf1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3acf1-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="3acf1-133">targetGroupId</span></span>|<span data-ttu-id="3acf1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3acf1-134">String</span></span>|<span data-ttu-id="3acf1-135">Идентификатор группы AAD целевого приложения подготовки конфигурации.</span><span class="sxs-lookup"><span data-stu-id="3acf1-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="3acf1-136">id</span><span class="sxs-lookup"><span data-stu-id="3acf1-136">id</span></span>|<span data-ttu-id="3acf1-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3acf1-137">String</span></span>|<span data-ttu-id="3acf1-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3acf1-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="3acf1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3acf1-139">Response</span></span>
<span data-ttu-id="3acf1-140">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3acf1-140">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3acf1-141">Пример</span><span class="sxs-lookup"><span data-stu-id="3acf1-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="3acf1-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="3acf1-142">Request</span></span>
<span data-ttu-id="3acf1-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3acf1-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 48

{
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="3acf1-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="3acf1-144">Response</span></span>
<span data-ttu-id="3acf1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3acf1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```





