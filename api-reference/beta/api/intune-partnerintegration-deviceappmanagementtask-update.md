---
title: Обновление устройстваAppManagementTask
description: Обновление свойств объекта deviceAppManagementTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c22587015dbf22b1537c7774244d551225e8690f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134881"
---
# <a name="update-deviceappmanagementtask"></a><span data-ttu-id="ad84b-103">Обновление устройстваAppManagementTask</span><span class="sxs-lookup"><span data-stu-id="ad84b-103">Update deviceAppManagementTask</span></span>

<span data-ttu-id="ad84b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad84b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad84b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad84b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad84b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad84b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad84b-107">Обновление свойств объекта [deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="ad84b-107">Update the properties of a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad84b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ad84b-108">Prerequisites</span></span>
<span data-ttu-id="ad84b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad84b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad84b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad84b-111">Permission type</span></span>|<span data-ttu-id="ad84b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad84b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad84b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad84b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad84b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad84b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ad84b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad84b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad84b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad84b-116">Not supported.</span></span>|
|<span data-ttu-id="ad84b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ad84b-117">Application</span></span>|<span data-ttu-id="ad84b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad84b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad84b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad84b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="ad84b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ad84b-120">Request headers</span></span>
|<span data-ttu-id="ad84b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad84b-121">Header</span></span>|<span data-ttu-id="ad84b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ad84b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad84b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad84b-123">Authorization</span></span>|<span data-ttu-id="ad84b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad84b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad84b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad84b-125">Accept</span></span>|<span data-ttu-id="ad84b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad84b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad84b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad84b-127">Request body</span></span>
<span data-ttu-id="ad84b-128">В теле запроса поставляем представление JSON для [объекта deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="ad84b-128">In the request body, supply a JSON representation for the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

<span data-ttu-id="ad84b-129">В следующей таблице показаны свойства, необходимые при создании [устройстваAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="ad84b-129">The following table shows the properties that are required when you create the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span>

|<span data-ttu-id="ad84b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad84b-130">Property</span></span>|<span data-ttu-id="ad84b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ad84b-131">Type</span></span>|<span data-ttu-id="ad84b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ad84b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad84b-133">id</span><span class="sxs-lookup"><span data-stu-id="ad84b-133">id</span></span>|<span data-ttu-id="ad84b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ad84b-134">String</span></span>|<span data-ttu-id="ad84b-135">Ключ сущности.</span><span class="sxs-lookup"><span data-stu-id="ad84b-135">The entity key.</span></span>|
|<span data-ttu-id="ad84b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ad84b-136">displayName</span></span>|<span data-ttu-id="ad84b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="ad84b-137">String</span></span>|<span data-ttu-id="ad84b-138">Имя.</span><span class="sxs-lookup"><span data-stu-id="ad84b-138">The name.</span></span>|
|<span data-ttu-id="ad84b-139">description</span><span class="sxs-lookup"><span data-stu-id="ad84b-139">description</span></span>|<span data-ttu-id="ad84b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="ad84b-140">String</span></span>|<span data-ttu-id="ad84b-141">Описание.</span><span class="sxs-lookup"><span data-stu-id="ad84b-141">The description.</span></span>|
|<span data-ttu-id="ad84b-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad84b-142">createdDateTime</span></span>|<span data-ttu-id="ad84b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad84b-143">DateTimeOffset</span></span>|<span data-ttu-id="ad84b-144">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="ad84b-144">The created date.</span></span>|
|<span data-ttu-id="ad84b-145">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="ad84b-145">dueDateTime</span></span>|<span data-ttu-id="ad84b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad84b-146">DateTimeOffset</span></span>|<span data-ttu-id="ad84b-147">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="ad84b-147">The due date.</span></span>|
|<span data-ttu-id="ad84b-148">category</span><span class="sxs-lookup"><span data-stu-id="ad84b-148">category</span></span>|[<span data-ttu-id="ad84b-149">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="ad84b-149">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="ad84b-150">Категория.</span><span class="sxs-lookup"><span data-stu-id="ad84b-150">The category.</span></span> <span data-ttu-id="ad84b-151">Возможные значения: `unknown`, `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="ad84b-151">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="ad84b-152">priority</span><span class="sxs-lookup"><span data-stu-id="ad84b-152">priority</span></span>|[<span data-ttu-id="ad84b-153">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="ad84b-153">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="ad84b-154">Приоритет.</span><span class="sxs-lookup"><span data-stu-id="ad84b-154">The priority.</span></span> <span data-ttu-id="ad84b-155">Возможные значения: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="ad84b-155">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="ad84b-156">creator</span><span class="sxs-lookup"><span data-stu-id="ad84b-156">creator</span></span>|<span data-ttu-id="ad84b-157">Строка</span><span class="sxs-lookup"><span data-stu-id="ad84b-157">String</span></span>|<span data-ttu-id="ad84b-158">Адрес электронной почты создателя.</span><span class="sxs-lookup"><span data-stu-id="ad84b-158">The email address of the creator.</span></span>|
|<span data-ttu-id="ad84b-159">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="ad84b-159">creatorNotes</span></span>|<span data-ttu-id="ad84b-160">Строка</span><span class="sxs-lookup"><span data-stu-id="ad84b-160">String</span></span>|<span data-ttu-id="ad84b-161">Заметки от создателя.</span><span class="sxs-lookup"><span data-stu-id="ad84b-161">Notes from the creator.</span></span>|
|<span data-ttu-id="ad84b-162">assignedTo</span><span class="sxs-lookup"><span data-stu-id="ad84b-162">assignedTo</span></span>|<span data-ttu-id="ad84b-163">String</span><span class="sxs-lookup"><span data-stu-id="ad84b-163">String</span></span>|<span data-ttu-id="ad84b-164">Имя или электронная почта администратора этой задачи назначены.</span><span class="sxs-lookup"><span data-stu-id="ad84b-164">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="ad84b-165">status</span><span class="sxs-lookup"><span data-stu-id="ad84b-165">status</span></span>|[<span data-ttu-id="ad84b-166">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="ad84b-166">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="ad84b-167">Состояние.</span><span class="sxs-lookup"><span data-stu-id="ad84b-167">The status.</span></span> <span data-ttu-id="ad84b-168">Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="ad84b-168">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="ad84b-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad84b-169">Response</span></span>
<span data-ttu-id="ad84b-170">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ad84b-170">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad84b-171">Пример</span><span class="sxs-lookup"><span data-stu-id="ad84b-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad84b-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad84b-172">Request</span></span>
<span data-ttu-id="ad84b-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad84b-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ad84b-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad84b-174">Response</span></span>
<span data-ttu-id="ad84b-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad84b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




