---
title: Создание Девицеаппманажементтаск
description: Создание нового объекта Девицеаппманажементтаск.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6589ac7e13e59653e5b4f85c4dfe78c2e71c617
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001834"
---
# <a name="create-deviceappmanagementtask"></a><span data-ttu-id="95e2a-103">Создание Девицеаппманажементтаск</span><span class="sxs-lookup"><span data-stu-id="95e2a-103">Create deviceAppManagementTask</span></span>

> <span data-ttu-id="95e2a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95e2a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95e2a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95e2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95e2a-106">Создание нового объекта [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .</span><span class="sxs-lookup"><span data-stu-id="95e2a-106">Create a new [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95e2a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="95e2a-107">Prerequisites</span></span>
<span data-ttu-id="95e2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95e2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95e2a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95e2a-110">Permission type</span></span>|<span data-ttu-id="95e2a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95e2a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95e2a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95e2a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95e2a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e2a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95e2a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95e2a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95e2a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95e2a-115">Not supported.</span></span>|
|<span data-ttu-id="95e2a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95e2a-116">Application</span></span>|<span data-ttu-id="95e2a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95e2a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95e2a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95e2a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="95e2a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95e2a-119">Request headers</span></span>
|<span data-ttu-id="95e2a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95e2a-120">Header</span></span>|<span data-ttu-id="95e2a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="95e2a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95e2a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95e2a-122">Authorization</span></span>|<span data-ttu-id="95e2a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95e2a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95e2a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="95e2a-124">Accept</span></span>|<span data-ttu-id="95e2a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95e2a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95e2a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="95e2a-126">Request body</span></span>
<span data-ttu-id="95e2a-127">В тексте запроса добавьте представление объекта Девицеаппманажементтаск в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95e2a-127">In the request body, supply a JSON representation for the deviceAppManagementTask object.</span></span>

<span data-ttu-id="95e2a-128">В следующей таблице приведены свойства, необходимые при создании Девицеаппманажементтаск.</span><span class="sxs-lookup"><span data-stu-id="95e2a-128">The following table shows the properties that are required when you create the deviceAppManagementTask.</span></span>

|<span data-ttu-id="95e2a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="95e2a-129">Property</span></span>|<span data-ttu-id="95e2a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="95e2a-130">Type</span></span>|<span data-ttu-id="95e2a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="95e2a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95e2a-132">id</span><span class="sxs-lookup"><span data-stu-id="95e2a-132">id</span></span>|<span data-ttu-id="95e2a-133">String</span><span class="sxs-lookup"><span data-stu-id="95e2a-133">String</span></span>|<span data-ttu-id="95e2a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="95e2a-134">The entity key.</span></span>|
|<span data-ttu-id="95e2a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="95e2a-135">displayName</span></span>|<span data-ttu-id="95e2a-136">Строка</span><span class="sxs-lookup"><span data-stu-id="95e2a-136">String</span></span>|<span data-ttu-id="95e2a-137">Имя.</span><span class="sxs-lookup"><span data-stu-id="95e2a-137">The name.</span></span>|
|<span data-ttu-id="95e2a-138">description</span><span class="sxs-lookup"><span data-stu-id="95e2a-138">description</span></span>|<span data-ttu-id="95e2a-139">String</span><span class="sxs-lookup"><span data-stu-id="95e2a-139">String</span></span>|<span data-ttu-id="95e2a-140">Описание.</span><span class="sxs-lookup"><span data-stu-id="95e2a-140">The description.</span></span>|
|<span data-ttu-id="95e2a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95e2a-141">createdDateTime</span></span>|<span data-ttu-id="95e2a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95e2a-142">DateTimeOffset</span></span>|<span data-ttu-id="95e2a-143">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="95e2a-143">The created date.</span></span>|
|<span data-ttu-id="95e2a-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="95e2a-144">dueDateTime</span></span>|<span data-ttu-id="95e2a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95e2a-145">DateTimeOffset</span></span>|<span data-ttu-id="95e2a-146">Дата выполнения.</span><span class="sxs-lookup"><span data-stu-id="95e2a-146">The due date.</span></span>|
|<span data-ttu-id="95e2a-147">category</span><span class="sxs-lookup"><span data-stu-id="95e2a-147">category</span></span>|[<span data-ttu-id="95e2a-148">Девицеаппманажементтасккатегори</span><span class="sxs-lookup"><span data-stu-id="95e2a-148">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="95e2a-149">Категория.</span><span class="sxs-lookup"><span data-stu-id="95e2a-149">The category.</span></span> <span data-ttu-id="95e2a-150">Возможные значения: `unknown`, `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="95e2a-150">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="95e2a-151">priority</span><span class="sxs-lookup"><span data-stu-id="95e2a-151">priority</span></span>|[<span data-ttu-id="95e2a-152">Девицеаппманажементтаскприорити</span><span class="sxs-lookup"><span data-stu-id="95e2a-152">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="95e2a-153">Приоритет.</span><span class="sxs-lookup"><span data-stu-id="95e2a-153">The priority.</span></span> <span data-ttu-id="95e2a-154">Возможные значения: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="95e2a-154">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="95e2a-155">модуль</span><span class="sxs-lookup"><span data-stu-id="95e2a-155">creator</span></span>|<span data-ttu-id="95e2a-156">String</span><span class="sxs-lookup"><span data-stu-id="95e2a-156">String</span></span>|<span data-ttu-id="95e2a-157">Адрес электронной почты создателя.</span><span class="sxs-lookup"><span data-stu-id="95e2a-157">The email address of the creator.</span></span>|
|<span data-ttu-id="95e2a-158">Креаторнотес</span><span class="sxs-lookup"><span data-stu-id="95e2a-158">creatorNotes</span></span>|<span data-ttu-id="95e2a-159">String</span><span class="sxs-lookup"><span data-stu-id="95e2a-159">String</span></span>|<span data-ttu-id="95e2a-160">Заметки автора.</span><span class="sxs-lookup"><span data-stu-id="95e2a-160">Notes from the creator.</span></span>|
|<span data-ttu-id="95e2a-161">assignedTo</span><span class="sxs-lookup"><span data-stu-id="95e2a-161">assignedTo</span></span>|<span data-ttu-id="95e2a-162">String</span><span class="sxs-lookup"><span data-stu-id="95e2a-162">String</span></span>|<span data-ttu-id="95e2a-163">Имя или электронная почта администратора, которому назначена эта задача.</span><span class="sxs-lookup"><span data-stu-id="95e2a-163">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="95e2a-164">status</span><span class="sxs-lookup"><span data-stu-id="95e2a-164">status</span></span>|[<span data-ttu-id="95e2a-165">Девицеаппманажементтаскстатус</span><span class="sxs-lookup"><span data-stu-id="95e2a-165">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="95e2a-166">Состояние.</span><span class="sxs-lookup"><span data-stu-id="95e2a-166">The status.</span></span> <span data-ttu-id="95e2a-167">Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="95e2a-167">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="95e2a-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="95e2a-168">Response</span></span>
<span data-ttu-id="95e2a-169">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95e2a-169">If successful, this method returns a `201 Created` response code and a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95e2a-170">Пример</span><span class="sxs-lookup"><span data-stu-id="95e2a-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="95e2a-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="95e2a-171">Request</span></span>
<span data-ttu-id="95e2a-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95e2a-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="95e2a-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="95e2a-173">Response</span></span>
<span data-ttu-id="95e2a-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95e2a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





