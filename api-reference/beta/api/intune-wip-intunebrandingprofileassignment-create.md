---
title: Создание Интунебрандингпрофилеассигнмент
description: Создание нового объекта Интунебрандингпрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eab148c53ac7fc313daf5e90345bd66160b5323b
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178404"
---
# <a name="create-intunebrandingprofileassignment"></a><span data-ttu-id="5a36b-103">Создание Интунебрандингпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="5a36b-103">Create intuneBrandingProfileAssignment</span></span>

<span data-ttu-id="5a36b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a36b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a36b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a36b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a36b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a36b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a36b-107">Создание нового объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5a36b-107">Create a new [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a36b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5a36b-108">Prerequisites</span></span>
<span data-ttu-id="5a36b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a36b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a36b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a36b-111">Permission type</span></span>|<span data-ttu-id="5a36b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a36b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a36b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a36b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a36b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a36b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5a36b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a36b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a36b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a36b-116">Not supported.</span></span>|
|<span data-ttu-id="5a36b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a36b-117">Application</span></span>|<span data-ttu-id="5a36b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a36b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a36b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a36b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="5a36b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5a36b-120">Request headers</span></span>
|<span data-ttu-id="5a36b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a36b-121">Header</span></span>|<span data-ttu-id="5a36b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5a36b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a36b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a36b-123">Authorization</span></span>|<span data-ttu-id="5a36b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a36b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a36b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5a36b-125">Accept</span></span>|<span data-ttu-id="5a36b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a36b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a36b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a36b-127">Request body</span></span>
<span data-ttu-id="5a36b-128">В тексте запроса добавьте представление объекта Интунебрандингпрофилеассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a36b-128">In the request body, supply a JSON representation for the intuneBrandingProfileAssignment object.</span></span>

<span data-ttu-id="5a36b-129">В следующей таблице приведены свойства, необходимые при создании Интунебрандингпрофилеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="5a36b-129">The following table shows the properties that are required when you create the intuneBrandingProfileAssignment.</span></span>

|<span data-ttu-id="5a36b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a36b-130">Property</span></span>|<span data-ttu-id="5a36b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5a36b-131">Type</span></span>|<span data-ttu-id="5a36b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5a36b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a36b-133">id</span><span class="sxs-lookup"><span data-stu-id="5a36b-133">id</span></span>|<span data-ttu-id="5a36b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5a36b-134">String</span></span>|<span data-ttu-id="5a36b-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="5a36b-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5a36b-136">target</span><span class="sxs-lookup"><span data-stu-id="5a36b-136">target</span></span>|[<span data-ttu-id="5a36b-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5a36b-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5a36b-138">Цель назначения, которой назначен профиль фирменной символики.</span><span class="sxs-lookup"><span data-stu-id="5a36b-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="5a36b-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a36b-139">Response</span></span>
<span data-ttu-id="5a36b-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a36b-140">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a36b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="5a36b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a36b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a36b-142">Request</span></span>
<span data-ttu-id="5a36b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a36b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="5a36b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a36b-144">Response</span></span>
<span data-ttu-id="5a36b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a36b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 208

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```



