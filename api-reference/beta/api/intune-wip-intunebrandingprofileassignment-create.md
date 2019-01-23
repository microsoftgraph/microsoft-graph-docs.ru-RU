---
title: Создание intuneBrandingProfileAssignment
description: Создание нового объекта intuneBrandingProfileAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 17c6a6c1f06d383a6019c168b41187826cb63067
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430669"
---
# <a name="create-intunebrandingprofileassignment"></a><span data-ttu-id="9b1bd-103">Создание intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="9b1bd-103">Create intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="9b1bd-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9b1bd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9b1bd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b1bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b1bd-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b1bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b1bd-107">Создание нового объекта [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9b1bd-107">Create a new [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b1bd-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="9b1bd-108">Prerequisites</span></span>
<span data-ttu-id="9b1bd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9b1bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9b1bd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b1bd-111">Permission type</span></span>|<span data-ttu-id="9b1bd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b1bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b1bd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b1bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b1bd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b1bd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9b1bd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b1bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b1bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b1bd-116">Not supported.</span></span>|
|<span data-ttu-id="9b1bd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b1bd-117">Application</span></span>|<span data-ttu-id="9b1bd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b1bd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b1bd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b1bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9b1bd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b1bd-120">Request headers</span></span>
|<span data-ttu-id="9b1bd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b1bd-121">Header</span></span>|<span data-ttu-id="9b1bd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9b1bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b1bd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b1bd-123">Authorization</span></span>|<span data-ttu-id="9b1bd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9b1bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b1bd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9b1bd-125">Accept</span></span>|<span data-ttu-id="9b1bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b1bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b1bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b1bd-127">Request body</span></span>
<span data-ttu-id="9b1bd-128">В тексте запроса укажите представление JSON для объекта intuneBrandingProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="9b1bd-128">In the request body, supply a JSON representation for the intuneBrandingProfileAssignment object.</span></span>

<span data-ttu-id="9b1bd-129">В следующей таблице показаны свойства, которые необходимы для создания intuneBrandingProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="9b1bd-129">The following table shows the properties that are required when you create the intuneBrandingProfileAssignment.</span></span>

|<span data-ttu-id="9b1bd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b1bd-130">Property</span></span>|<span data-ttu-id="9b1bd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9b1bd-131">Type</span></span>|<span data-ttu-id="9b1bd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9b1bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b1bd-133">id</span><span class="sxs-lookup"><span data-stu-id="9b1bd-133">id</span></span>|<span data-ttu-id="9b1bd-134">String</span><span class="sxs-lookup"><span data-stu-id="9b1bd-134">String</span></span>|<span data-ttu-id="9b1bd-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="9b1bd-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="9b1bd-136">target</span><span class="sxs-lookup"><span data-stu-id="9b1bd-136">target</span></span>|[<span data-ttu-id="9b1bd-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9b1bd-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9b1bd-138">Целевой объект назначения, назначенная фирменной настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="9b1bd-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="9b1bd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b1bd-139">Response</span></span>
<span data-ttu-id="9b1bd-140">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9b1bd-140">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b1bd-141">Пример</span><span class="sxs-lookup"><span data-stu-id="9b1bd-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b1bd-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b1bd-142">Request</span></span>
<span data-ttu-id="9b1bd-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b1bd-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="9b1bd-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b1bd-144">Response</span></span>
<span data-ttu-id="9b1bd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9b1bd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




