---
title: Обновление intuneBrandingProfileAssignment
description: Обновление свойства объекта intuneBrandingProfileAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7bfdba766221fc27dde6a8b71212620b744c4fc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430615"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="8a0b8-103">Обновление intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="8a0b8-103">Update intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="8a0b8-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8a0b8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a0b8-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a0b8-107">Обновление свойства объекта [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8a0b8-107">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a0b8-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="8a0b8-108">Prerequisites</span></span>
<span data-ttu-id="8a0b8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8a0b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8a0b8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a0b8-111">Permission type</span></span>|<span data-ttu-id="8a0b8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a0b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a0b8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a0b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a0b8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a0b8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8a0b8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a0b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a0b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-116">Not supported.</span></span>|
|<span data-ttu-id="8a0b8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a0b8-117">Application</span></span>|<span data-ttu-id="8a0b8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a0b8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a0b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8a0b8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a0b8-120">Request headers</span></span>
|<span data-ttu-id="8a0b8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a0b8-121">Header</span></span>|<span data-ttu-id="8a0b8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8a0b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a0b8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a0b8-123">Authorization</span></span>|<span data-ttu-id="8a0b8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8a0b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a0b8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8a0b8-125">Accept</span></span>|<span data-ttu-id="8a0b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a0b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a0b8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a0b8-127">Request body</span></span>
<span data-ttu-id="8a0b8-128">В тексте запроса укажите представление JSON для объекта [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8a0b8-128">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="8a0b8-129">В следующей таблице показаны свойства, которые необходимы для создания [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8a0b8-129">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="8a0b8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a0b8-130">Property</span></span>|<span data-ttu-id="8a0b8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8a0b8-131">Type</span></span>|<span data-ttu-id="8a0b8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8a0b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a0b8-133">id</span><span class="sxs-lookup"><span data-stu-id="8a0b8-133">id</span></span>|<span data-ttu-id="8a0b8-134">String</span><span class="sxs-lookup"><span data-stu-id="8a0b8-134">String</span></span>|<span data-ttu-id="8a0b8-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="8a0b8-136">target</span><span class="sxs-lookup"><span data-stu-id="8a0b8-136">target</span></span>|[<span data-ttu-id="8a0b8-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8a0b8-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8a0b8-138">Целевой объект назначения, назначенная фирменной настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="8a0b8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a0b8-139">Response</span></span>
<span data-ttu-id="8a0b8-140">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-140">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a0b8-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8a0b8-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a0b8-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a0b8-142">Request</span></span>
<span data-ttu-id="8a0b8-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="8a0b8-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a0b8-144">Response</span></span>
<span data-ttu-id="8a0b8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 220

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




