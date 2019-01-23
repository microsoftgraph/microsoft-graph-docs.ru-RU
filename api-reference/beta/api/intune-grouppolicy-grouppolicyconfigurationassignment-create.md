---
title: Создание groupPolicyConfigurationAssignment
description: Создание нового объекта groupPolicyConfigurationAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: db4c96db45f5c54f70cf1216829834b453dbcd9f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430824"
---
# <a name="create-grouppolicyconfigurationassignment"></a><span data-ttu-id="3500d-103">Создание groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3500d-103">Create groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="3500d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3500d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3500d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3500d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3500d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3500d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3500d-107">Создание нового объекта [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3500d-107">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3500d-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="3500d-108">Prerequisites</span></span>
<span data-ttu-id="3500d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3500d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3500d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3500d-111">Permission type</span></span>|<span data-ttu-id="3500d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3500d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3500d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3500d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3500d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3500d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3500d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3500d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3500d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3500d-116">Not supported.</span></span>|
|<span data-ttu-id="3500d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3500d-117">Application</span></span>|<span data-ttu-id="3500d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3500d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3500d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3500d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="3500d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3500d-120">Request headers</span></span>
|<span data-ttu-id="3500d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3500d-121">Header</span></span>|<span data-ttu-id="3500d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3500d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3500d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3500d-123">Authorization</span></span>|<span data-ttu-id="3500d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3500d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3500d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3500d-125">Accept</span></span>|<span data-ttu-id="3500d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3500d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3500d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3500d-127">Request body</span></span>
<span data-ttu-id="3500d-128">В тексте запроса укажите представление JSON для объекта groupPolicyConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="3500d-128">In the request body, supply a JSON representation for the groupPolicyConfigurationAssignment object.</span></span>

<span data-ttu-id="3500d-129">В следующей таблице показаны свойства, которые необходимы для создания groupPolicyConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="3500d-129">The following table shows the properties that are required when you create the groupPolicyConfigurationAssignment.</span></span>

|<span data-ttu-id="3500d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3500d-130">Property</span></span>|<span data-ttu-id="3500d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3500d-131">Type</span></span>|<span data-ttu-id="3500d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3500d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3500d-133">id</span><span class="sxs-lookup"><span data-stu-id="3500d-133">id</span></span>|<span data-ttu-id="3500d-134">String</span><span class="sxs-lookup"><span data-stu-id="3500d-134">String</span></span>|<span data-ttu-id="3500d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3500d-135">Key of the entity.</span></span>|
|<span data-ttu-id="3500d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3500d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3500d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3500d-137">DateTimeOffset</span></span>|<span data-ttu-id="3500d-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3500d-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="3500d-139">target</span><span class="sxs-lookup"><span data-stu-id="3500d-139">target</span></span>|[<span data-ttu-id="3500d-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3500d-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3500d-141">Тип группы целевой параметры групповой политики.</span><span class="sxs-lookup"><span data-stu-id="3500d-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="3500d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3500d-142">Response</span></span>
<span data-ttu-id="3500d-143">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3500d-143">If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3500d-144">Пример</span><span class="sxs-lookup"><span data-stu-id="3500d-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="3500d-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3500d-145">Request</span></span>
<span data-ttu-id="3500d-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3500d-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="3500d-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="3500d-147">Response</span></span>
<span data-ttu-id="3500d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3500d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




