---
title: Создание объекта mobileAppAssignment
description: Создание объекта mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8ceae2f0bacac3d83532a6aa9b338c32573d6332
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874657"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="b4187-103">Создание объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="b4187-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="b4187-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b4187-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4187-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4187-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4187-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b4187-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4187-107">Создание объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b4187-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4187-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b4187-108">Prerequisites</span></span>
<span data-ttu-id="b4187-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4187-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4187-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4187-111">Permission type</span></span>|<span data-ttu-id="b4187-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4187-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4187-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4187-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4187-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4187-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4187-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4187-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4187-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4187-116">Not supported.</span></span>|
|<span data-ttu-id="b4187-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4187-117">Application</span></span>|<span data-ttu-id="b4187-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4187-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4187-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4187-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b4187-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4187-120">Request headers</span></span>
|<span data-ttu-id="b4187-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4187-121">Header</span></span>|<span data-ttu-id="b4187-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b4187-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4187-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4187-123">Authorization</span></span>|<span data-ttu-id="b4187-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b4187-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4187-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b4187-125">Accept</span></span>|<span data-ttu-id="b4187-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4187-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4187-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4187-127">Request body</span></span>
<span data-ttu-id="b4187-128">В тексте запроса добавьте представление объекта mobileAppAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4187-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="b4187-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="b4187-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="b4187-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4187-130">Property</span></span>|<span data-ttu-id="b4187-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b4187-131">Type</span></span>|<span data-ttu-id="b4187-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b4187-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4187-133">id</span><span class="sxs-lookup"><span data-stu-id="b4187-133">id</span></span>|<span data-ttu-id="b4187-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b4187-134">String</span></span>|<span data-ttu-id="b4187-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b4187-135">Key of the entity.</span></span>|
|<span data-ttu-id="b4187-136">intent</span><span class="sxs-lookup"><span data-stu-id="b4187-136">intent</span></span>|[<span data-ttu-id="b4187-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="b4187-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="b4187-138">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="b4187-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="b4187-139">target</span><span class="sxs-lookup"><span data-stu-id="b4187-139">target</span></span>|[<span data-ttu-id="b4187-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b4187-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b4187-141">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="b4187-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="b4187-142">settings</span><span class="sxs-lookup"><span data-stu-id="b4187-142">settings</span></span>|[<span data-ttu-id="b4187-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="b4187-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="b4187-144">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="b4187-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="b4187-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4187-145">Response</span></span>
<span data-ttu-id="b4187-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4187-146">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4187-147">Пример</span><span class="sxs-lookup"><span data-stu-id="b4187-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4187-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4187-148">Request</span></span>
<span data-ttu-id="b4187-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4187-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="b4187-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4187-150">Response</span></span>
<span data-ttu-id="b4187-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b4187-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```





