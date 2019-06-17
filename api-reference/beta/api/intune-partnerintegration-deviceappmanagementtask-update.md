---
title: Обновление Девицеаппманажементтаск
description: Обновление свойств объекта Девицеаппманажементтаск.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c79868e1c618dfd3aaec3dfd9a47e2e572fca280
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002303"
---
# <a name="update-deviceappmanagementtask"></a><span data-ttu-id="0b943-103">Обновление Девицеаппманажементтаск</span><span class="sxs-lookup"><span data-stu-id="0b943-103">Update deviceAppManagementTask</span></span>

> <span data-ttu-id="0b943-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b943-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b943-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b943-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b943-106">Обновление свойств объекта [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .</span><span class="sxs-lookup"><span data-stu-id="0b943-106">Update the properties of a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b943-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0b943-107">Prerequisites</span></span>
<span data-ttu-id="0b943-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b943-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b943-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b943-110">Permission type</span></span>|<span data-ttu-id="0b943-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b943-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b943-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b943-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b943-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b943-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0b943-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b943-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b943-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b943-115">Not supported.</span></span>|
|<span data-ttu-id="0b943-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b943-116">Application</span></span>|<span data-ttu-id="0b943-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b943-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b943-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b943-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="0b943-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b943-119">Request headers</span></span>
|<span data-ttu-id="0b943-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b943-120">Header</span></span>|<span data-ttu-id="0b943-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0b943-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b943-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b943-122">Authorization</span></span>|<span data-ttu-id="0b943-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b943-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b943-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0b943-124">Accept</span></span>|<span data-ttu-id="0b943-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b943-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b943-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0b943-126">Request body</span></span>
<span data-ttu-id="0b943-127">В тексте запроса добавьте представление объекта [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b943-127">In the request body, supply a JSON representation for the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

<span data-ttu-id="0b943-128">В следующей таблице приведены свойства, необходимые при создании [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="0b943-128">The following table shows the properties that are required when you create the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span>

|<span data-ttu-id="0b943-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b943-129">Property</span></span>|<span data-ttu-id="0b943-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0b943-130">Type</span></span>|<span data-ttu-id="0b943-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0b943-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b943-132">id</span><span class="sxs-lookup"><span data-stu-id="0b943-132">id</span></span>|<span data-ttu-id="0b943-133">String</span><span class="sxs-lookup"><span data-stu-id="0b943-133">String</span></span>|<span data-ttu-id="0b943-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0b943-134">The entity key.</span></span>|
|<span data-ttu-id="0b943-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0b943-135">displayName</span></span>|<span data-ttu-id="0b943-136">Строка</span><span class="sxs-lookup"><span data-stu-id="0b943-136">String</span></span>|<span data-ttu-id="0b943-137">Имя.</span><span class="sxs-lookup"><span data-stu-id="0b943-137">The name.</span></span>|
|<span data-ttu-id="0b943-138">description</span><span class="sxs-lookup"><span data-stu-id="0b943-138">description</span></span>|<span data-ttu-id="0b943-139">String</span><span class="sxs-lookup"><span data-stu-id="0b943-139">String</span></span>|<span data-ttu-id="0b943-140">Описание.</span><span class="sxs-lookup"><span data-stu-id="0b943-140">The description.</span></span>|
|<span data-ttu-id="0b943-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b943-141">createdDateTime</span></span>|<span data-ttu-id="0b943-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b943-142">DateTimeOffset</span></span>|<span data-ttu-id="0b943-143">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="0b943-143">The created date.</span></span>|
|<span data-ttu-id="0b943-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="0b943-144">dueDateTime</span></span>|<span data-ttu-id="0b943-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b943-145">DateTimeOffset</span></span>|<span data-ttu-id="0b943-146">Дата выполнения.</span><span class="sxs-lookup"><span data-stu-id="0b943-146">The due date.</span></span>|
|<span data-ttu-id="0b943-147">category</span><span class="sxs-lookup"><span data-stu-id="0b943-147">category</span></span>|[<span data-ttu-id="0b943-148">Девицеаппманажементтасккатегори</span><span class="sxs-lookup"><span data-stu-id="0b943-148">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="0b943-149">Категория.</span><span class="sxs-lookup"><span data-stu-id="0b943-149">The category.</span></span> <span data-ttu-id="0b943-150">Возможные значения: `unknown`, `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="0b943-150">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="0b943-151">priority</span><span class="sxs-lookup"><span data-stu-id="0b943-151">priority</span></span>|[<span data-ttu-id="0b943-152">Девицеаппманажементтаскприорити</span><span class="sxs-lookup"><span data-stu-id="0b943-152">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="0b943-153">Приоритет.</span><span class="sxs-lookup"><span data-stu-id="0b943-153">The priority.</span></span> <span data-ttu-id="0b943-154">Возможные значения: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="0b943-154">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="0b943-155">модуль</span><span class="sxs-lookup"><span data-stu-id="0b943-155">creator</span></span>|<span data-ttu-id="0b943-156">String</span><span class="sxs-lookup"><span data-stu-id="0b943-156">String</span></span>|<span data-ttu-id="0b943-157">Адрес электронной почты создателя.</span><span class="sxs-lookup"><span data-stu-id="0b943-157">The email address of the creator.</span></span>|
|<span data-ttu-id="0b943-158">Креаторнотес</span><span class="sxs-lookup"><span data-stu-id="0b943-158">creatorNotes</span></span>|<span data-ttu-id="0b943-159">String</span><span class="sxs-lookup"><span data-stu-id="0b943-159">String</span></span>|<span data-ttu-id="0b943-160">Заметки автора.</span><span class="sxs-lookup"><span data-stu-id="0b943-160">Notes from the creator.</span></span>|
|<span data-ttu-id="0b943-161">assignedTo</span><span class="sxs-lookup"><span data-stu-id="0b943-161">assignedTo</span></span>|<span data-ttu-id="0b943-162">String</span><span class="sxs-lookup"><span data-stu-id="0b943-162">String</span></span>|<span data-ttu-id="0b943-163">Имя или электронная почта администратора, которому назначена эта задача.</span><span class="sxs-lookup"><span data-stu-id="0b943-163">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="0b943-164">status</span><span class="sxs-lookup"><span data-stu-id="0b943-164">status</span></span>|[<span data-ttu-id="0b943-165">Девицеаппманажементтаскстатус</span><span class="sxs-lookup"><span data-stu-id="0b943-165">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="0b943-166">Состояние.</span><span class="sxs-lookup"><span data-stu-id="0b943-166">The status.</span></span> <span data-ttu-id="0b943-167">Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="0b943-167">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="0b943-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b943-168">Response</span></span>
<span data-ttu-id="0b943-169">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0b943-169">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b943-170">Пример</span><span class="sxs-lookup"><span data-stu-id="0b943-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b943-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b943-171">Request</span></span>
<span data-ttu-id="0b943-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b943-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
Content-type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="0b943-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b943-173">Response</span></span>
<span data-ttu-id="0b943-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b943-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "814545cc-45cc-8145-cc45-4581cc454581",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending"
}
```





