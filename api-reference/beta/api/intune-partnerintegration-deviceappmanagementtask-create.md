---
title: Создание Девицеаппманажементтаск
description: Создание нового объекта Девицеаппманажементтаск.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 81771048e4a1c8868358a0a9d5eb66bd3843fec3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49285305"
---
# <a name="create-deviceappmanagementtask"></a><span data-ttu-id="c7af0-103">Создание Девицеаппманажементтаск</span><span class="sxs-lookup"><span data-stu-id="c7af0-103">Create deviceAppManagementTask</span></span>

<span data-ttu-id="c7af0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7af0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7af0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7af0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7af0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7af0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7af0-107">Создание нового объекта [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .</span><span class="sxs-lookup"><span data-stu-id="c7af0-107">Create a new [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7af0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c7af0-108">Prerequisites</span></span>
<span data-ttu-id="c7af0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7af0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7af0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7af0-111">Permission type</span></span>|<span data-ttu-id="c7af0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7af0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7af0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7af0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7af0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7af0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c7af0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7af0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7af0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7af0-116">Not supported.</span></span>|
|<span data-ttu-id="c7af0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7af0-117">Application</span></span>|<span data-ttu-id="c7af0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7af0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7af0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7af0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="c7af0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c7af0-120">Request headers</span></span>
|<span data-ttu-id="c7af0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7af0-121">Header</span></span>|<span data-ttu-id="c7af0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7af0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7af0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7af0-123">Authorization</span></span>|<span data-ttu-id="c7af0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7af0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7af0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7af0-125">Accept</span></span>|<span data-ttu-id="c7af0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7af0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7af0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7af0-127">Request body</span></span>
<span data-ttu-id="c7af0-128">В тексте запроса добавьте представление объекта Девицеаппманажементтаск в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7af0-128">In the request body, supply a JSON representation for the deviceAppManagementTask object.</span></span>

<span data-ttu-id="c7af0-129">В следующей таблице приведены свойства, необходимые при создании Девицеаппманажементтаск.</span><span class="sxs-lookup"><span data-stu-id="c7af0-129">The following table shows the properties that are required when you create the deviceAppManagementTask.</span></span>

|<span data-ttu-id="c7af0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7af0-130">Property</span></span>|<span data-ttu-id="c7af0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c7af0-131">Type</span></span>|<span data-ttu-id="c7af0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c7af0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7af0-133">id</span><span class="sxs-lookup"><span data-stu-id="c7af0-133">id</span></span>|<span data-ttu-id="c7af0-134">String</span><span class="sxs-lookup"><span data-stu-id="c7af0-134">String</span></span>|<span data-ttu-id="c7af0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c7af0-135">The entity key.</span></span>|
|<span data-ttu-id="c7af0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c7af0-136">displayName</span></span>|<span data-ttu-id="c7af0-137">String</span><span class="sxs-lookup"><span data-stu-id="c7af0-137">String</span></span>|<span data-ttu-id="c7af0-138">Имя.</span><span class="sxs-lookup"><span data-stu-id="c7af0-138">The name.</span></span>|
|<span data-ttu-id="c7af0-139">description</span><span class="sxs-lookup"><span data-stu-id="c7af0-139">description</span></span>|<span data-ttu-id="c7af0-140">String</span><span class="sxs-lookup"><span data-stu-id="c7af0-140">String</span></span>|<span data-ttu-id="c7af0-141">Описание.</span><span class="sxs-lookup"><span data-stu-id="c7af0-141">The description.</span></span>|
|<span data-ttu-id="c7af0-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7af0-142">createdDateTime</span></span>|<span data-ttu-id="c7af0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7af0-143">DateTimeOffset</span></span>|<span data-ttu-id="c7af0-144">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="c7af0-144">The created date.</span></span>|
|<span data-ttu-id="c7af0-145">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="c7af0-145">dueDateTime</span></span>|<span data-ttu-id="c7af0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7af0-146">DateTimeOffset</span></span>|<span data-ttu-id="c7af0-147">Дата выполнения.</span><span class="sxs-lookup"><span data-stu-id="c7af0-147">The due date.</span></span>|
|<span data-ttu-id="c7af0-148">category</span><span class="sxs-lookup"><span data-stu-id="c7af0-148">category</span></span>|[<span data-ttu-id="c7af0-149">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="c7af0-149">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="c7af0-150">Категория.</span><span class="sxs-lookup"><span data-stu-id="c7af0-150">The category.</span></span> <span data-ttu-id="c7af0-151">Возможные значения: `unknown`, `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="c7af0-151">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="c7af0-152">priority</span><span class="sxs-lookup"><span data-stu-id="c7af0-152">priority</span></span>|[<span data-ttu-id="c7af0-153">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="c7af0-153">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="c7af0-154">Приоритет.</span><span class="sxs-lookup"><span data-stu-id="c7af0-154">The priority.</span></span> <span data-ttu-id="c7af0-155">Возможные значения: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="c7af0-155">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="c7af0-156">creator</span><span class="sxs-lookup"><span data-stu-id="c7af0-156">creator</span></span>|<span data-ttu-id="c7af0-157">String</span><span class="sxs-lookup"><span data-stu-id="c7af0-157">String</span></span>|<span data-ttu-id="c7af0-158">Адрес электронной почты создателя.</span><span class="sxs-lookup"><span data-stu-id="c7af0-158">The email address of the creator.</span></span>|
|<span data-ttu-id="c7af0-159">креаторнотес</span><span class="sxs-lookup"><span data-stu-id="c7af0-159">creatorNotes</span></span>|<span data-ttu-id="c7af0-160">String</span><span class="sxs-lookup"><span data-stu-id="c7af0-160">String</span></span>|<span data-ttu-id="c7af0-161">Заметки автора.</span><span class="sxs-lookup"><span data-stu-id="c7af0-161">Notes from the creator.</span></span>|
|<span data-ttu-id="c7af0-162">assignedTo</span><span class="sxs-lookup"><span data-stu-id="c7af0-162">assignedTo</span></span>|<span data-ttu-id="c7af0-163">String</span><span class="sxs-lookup"><span data-stu-id="c7af0-163">String</span></span>|<span data-ttu-id="c7af0-164">Имя или электронная почта администратора, которому назначена эта задача.</span><span class="sxs-lookup"><span data-stu-id="c7af0-164">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="c7af0-165">status</span><span class="sxs-lookup"><span data-stu-id="c7af0-165">status</span></span>|[<span data-ttu-id="c7af0-166">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="c7af0-166">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="c7af0-167">Состояние.</span><span class="sxs-lookup"><span data-stu-id="c7af0-167">The status.</span></span> <span data-ttu-id="c7af0-168">Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="c7af0-168">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="c7af0-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7af0-169">Response</span></span>
<span data-ttu-id="c7af0-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7af0-170">If successful, this method returns a `201 Created` response code and a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7af0-171">Пример</span><span class="sxs-lookup"><span data-stu-id="c7af0-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7af0-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7af0-172">Request</span></span>
<span data-ttu-id="c7af0-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7af0-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c7af0-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7af0-174">Response</span></span>
<span data-ttu-id="c7af0-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7af0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




