---
title: Создание Девицеаппманажементтаск
description: Создание нового объекта Девицеаппманажементтаск.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0559c055e47079ff0054c48dc049a920d98f6de1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941339"
---
# <a name="create-deviceappmanagementtask"></a><span data-ttu-id="84648-103">Создание Девицеаппманажементтаск</span><span class="sxs-lookup"><span data-stu-id="84648-103">Create deviceAppManagementTask</span></span>

> <span data-ttu-id="84648-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84648-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84648-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84648-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84648-106">Создание нового объекта [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .</span><span class="sxs-lookup"><span data-stu-id="84648-106">Create a new [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84648-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="84648-107">Prerequisites</span></span>
<span data-ttu-id="84648-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84648-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84648-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84648-110">Permission type</span></span>|<span data-ttu-id="84648-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84648-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84648-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84648-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84648-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84648-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="84648-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84648-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84648-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84648-115">Not supported.</span></span>|
|<span data-ttu-id="84648-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84648-116">Application</span></span>|<span data-ttu-id="84648-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84648-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84648-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84648-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="84648-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="84648-119">Request headers</span></span>
|<span data-ttu-id="84648-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84648-120">Header</span></span>|<span data-ttu-id="84648-121">Значение</span><span class="sxs-lookup"><span data-stu-id="84648-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84648-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84648-122">Authorization</span></span>|<span data-ttu-id="84648-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84648-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84648-124">Accept</span><span class="sxs-lookup"><span data-stu-id="84648-124">Accept</span></span>|<span data-ttu-id="84648-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84648-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84648-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84648-126">Request body</span></span>
<span data-ttu-id="84648-127">В тексте запроса добавьте представление объекта Девицеаппманажементтаск в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84648-127">In the request body, supply a JSON representation for the deviceAppManagementTask object.</span></span>

<span data-ttu-id="84648-128">В следующей таблице приведены свойства, необходимые при создании Девицеаппманажементтаск.</span><span class="sxs-lookup"><span data-stu-id="84648-128">The following table shows the properties that are required when you create the deviceAppManagementTask.</span></span>

|<span data-ttu-id="84648-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="84648-129">Property</span></span>|<span data-ttu-id="84648-130">Тип</span><span class="sxs-lookup"><span data-stu-id="84648-130">Type</span></span>|<span data-ttu-id="84648-131">Описание</span><span class="sxs-lookup"><span data-stu-id="84648-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84648-132">id</span><span class="sxs-lookup"><span data-stu-id="84648-132">id</span></span>|<span data-ttu-id="84648-133">Строка</span><span class="sxs-lookup"><span data-stu-id="84648-133">String</span></span>|<span data-ttu-id="84648-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="84648-134">The entity key.</span></span>|
|<span data-ttu-id="84648-135">displayName</span><span class="sxs-lookup"><span data-stu-id="84648-135">displayName</span></span>|<span data-ttu-id="84648-136">Строка</span><span class="sxs-lookup"><span data-stu-id="84648-136">String</span></span>|<span data-ttu-id="84648-137">Имя.</span><span class="sxs-lookup"><span data-stu-id="84648-137">The name.</span></span>|
|<span data-ttu-id="84648-138">description</span><span class="sxs-lookup"><span data-stu-id="84648-138">description</span></span>|<span data-ttu-id="84648-139">String</span><span class="sxs-lookup"><span data-stu-id="84648-139">String</span></span>|<span data-ttu-id="84648-140">Описание.</span><span class="sxs-lookup"><span data-stu-id="84648-140">The description.</span></span>|
|<span data-ttu-id="84648-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84648-141">createdDateTime</span></span>|<span data-ttu-id="84648-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84648-142">DateTimeOffset</span></span>|<span data-ttu-id="84648-143">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="84648-143">The created date.</span></span>|
|<span data-ttu-id="84648-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="84648-144">dueDateTime</span></span>|<span data-ttu-id="84648-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84648-145">DateTimeOffset</span></span>|<span data-ttu-id="84648-146">Дата выполнения.</span><span class="sxs-lookup"><span data-stu-id="84648-146">The due date.</span></span>|
|<span data-ttu-id="84648-147">category</span><span class="sxs-lookup"><span data-stu-id="84648-147">category</span></span>|[<span data-ttu-id="84648-148">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="84648-148">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="84648-149">Категория.</span><span class="sxs-lookup"><span data-stu-id="84648-149">The category.</span></span> <span data-ttu-id="84648-150">Возможные значения: `unknown`, `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="84648-150">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="84648-151">priority</span><span class="sxs-lookup"><span data-stu-id="84648-151">priority</span></span>|[<span data-ttu-id="84648-152">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="84648-152">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="84648-153">Приоритет.</span><span class="sxs-lookup"><span data-stu-id="84648-153">The priority.</span></span> <span data-ttu-id="84648-154">Возможные значения: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="84648-154">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="84648-155">модуль</span><span class="sxs-lookup"><span data-stu-id="84648-155">creator</span></span>|<span data-ttu-id="84648-156">Строка</span><span class="sxs-lookup"><span data-stu-id="84648-156">String</span></span>|<span data-ttu-id="84648-157">Адрес электронной почты создателя.</span><span class="sxs-lookup"><span data-stu-id="84648-157">The email address of the creator.</span></span>|
|<span data-ttu-id="84648-158">креаторнотес</span><span class="sxs-lookup"><span data-stu-id="84648-158">creatorNotes</span></span>|<span data-ttu-id="84648-159">Строка</span><span class="sxs-lookup"><span data-stu-id="84648-159">String</span></span>|<span data-ttu-id="84648-160">Заметки автора.</span><span class="sxs-lookup"><span data-stu-id="84648-160">Notes from the creator.</span></span>|
|<span data-ttu-id="84648-161">assignedTo</span><span class="sxs-lookup"><span data-stu-id="84648-161">assignedTo</span></span>|<span data-ttu-id="84648-162">String</span><span class="sxs-lookup"><span data-stu-id="84648-162">String</span></span>|<span data-ttu-id="84648-163">Имя или электронная почта администратора, которому назначена эта задача.</span><span class="sxs-lookup"><span data-stu-id="84648-163">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="84648-164">status</span><span class="sxs-lookup"><span data-stu-id="84648-164">status</span></span>|[<span data-ttu-id="84648-165">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="84648-165">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="84648-166">Состояние.</span><span class="sxs-lookup"><span data-stu-id="84648-166">The status.</span></span> <span data-ttu-id="84648-167">Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="84648-167">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="84648-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="84648-168">Response</span></span>
<span data-ttu-id="84648-169">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84648-169">If successful, this method returns a `201 Created` response code and a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84648-170">Пример</span><span class="sxs-lookup"><span data-stu-id="84648-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="84648-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="84648-171">Request</span></span>
<span data-ttu-id="84648-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84648-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
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

### <a name="response"></a><span data-ttu-id="84648-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="84648-173">Response</span></span>
<span data-ttu-id="84648-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84648-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





