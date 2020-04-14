---
title: Обновление Девицеконфигуратионусерстатесуммари
description: Обновление свойств объекта Девицеконфигуратионусерстатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b34fb42e43a9d427516dc2b2e6712933a524ef3f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433289"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="455d2-103">Обновление Девицеконфигуратионусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="455d2-103">Update deviceConfigurationUserStateSummary</span></span>

<span data-ttu-id="455d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="455d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="455d2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="455d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="455d2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="455d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="455d2-107">Обновление свойств объекта [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="455d2-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="455d2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="455d2-108">Prerequisites</span></span>
<span data-ttu-id="455d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="455d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="455d2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="455d2-111">Permission type</span></span>|<span data-ttu-id="455d2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="455d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="455d2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="455d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="455d2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="455d2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="455d2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="455d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="455d2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="455d2-116">Not supported.</span></span>|
|<span data-ttu-id="455d2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="455d2-117">Application</span></span>|<span data-ttu-id="455d2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="455d2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="455d2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="455d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="455d2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="455d2-120">Request headers</span></span>
|<span data-ttu-id="455d2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="455d2-121">Header</span></span>|<span data-ttu-id="455d2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="455d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="455d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="455d2-123">Authorization</span></span>|<span data-ttu-id="455d2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="455d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="455d2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="455d2-125">Accept</span></span>|<span data-ttu-id="455d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="455d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="455d2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="455d2-127">Request body</span></span>
<span data-ttu-id="455d2-128">В тексте запроса добавьте представление объекта [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="455d2-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="455d2-129">В следующей таблице приведены свойства, необходимые при создании [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="455d2-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="455d2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="455d2-130">Property</span></span>|<span data-ttu-id="455d2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="455d2-131">Type</span></span>|<span data-ttu-id="455d2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="455d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="455d2-133">id</span><span class="sxs-lookup"><span data-stu-id="455d2-133">id</span></span>|<span data-ttu-id="455d2-134">String</span><span class="sxs-lookup"><span data-stu-id="455d2-134">String</span></span>|<span data-ttu-id="455d2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="455d2-135">Key of the entity.</span></span>|
|<span data-ttu-id="455d2-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="455d2-136">unknownUserCount</span></span>|<span data-ttu-id="455d2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="455d2-137">Int32</span></span>|<span data-ttu-id="455d2-138">Количество неизвестных пользователей</span><span class="sxs-lookup"><span data-stu-id="455d2-138">Number of unknown users</span></span>|
|<span data-ttu-id="455d2-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="455d2-139">notApplicableUserCount</span></span>|<span data-ttu-id="455d2-140">Int32</span><span class="sxs-lookup"><span data-stu-id="455d2-140">Int32</span></span>|<span data-ttu-id="455d2-141">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="455d2-141">Number of not applicable users</span></span>|
|<span data-ttu-id="455d2-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="455d2-142">compliantUserCount</span></span>|<span data-ttu-id="455d2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="455d2-143">Int32</span></span>|<span data-ttu-id="455d2-144">Число соответствующих пользователей</span><span class="sxs-lookup"><span data-stu-id="455d2-144">Number of compliant users</span></span>|
|<span data-ttu-id="455d2-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="455d2-145">remediatedUserCount</span></span>|<span data-ttu-id="455d2-146">Int32</span><span class="sxs-lookup"><span data-stu-id="455d2-146">Int32</span></span>|<span data-ttu-id="455d2-147">Количество исправленных пользователей</span><span class="sxs-lookup"><span data-stu-id="455d2-147">Number of remediated users</span></span>|
|<span data-ttu-id="455d2-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="455d2-148">nonCompliantUserCount</span></span>|<span data-ttu-id="455d2-149">Int32</span><span class="sxs-lookup"><span data-stu-id="455d2-149">Int32</span></span>|<span data-ttu-id="455d2-150">Количество несоответствующих пользователей</span><span class="sxs-lookup"><span data-stu-id="455d2-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="455d2-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="455d2-151">errorUserCount</span></span>|<span data-ttu-id="455d2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="455d2-152">Int32</span></span>|<span data-ttu-id="455d2-153">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="455d2-153">Number of error users</span></span>|
|<span data-ttu-id="455d2-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="455d2-154">conflictUserCount</span></span>|<span data-ttu-id="455d2-155">Int32</span><span class="sxs-lookup"><span data-stu-id="455d2-155">Int32</span></span>|<span data-ttu-id="455d2-156">Количество конфликтующих пользователей</span><span class="sxs-lookup"><span data-stu-id="455d2-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="455d2-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="455d2-157">Response</span></span>
<span data-ttu-id="455d2-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="455d2-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="455d2-159">Пример</span><span class="sxs-lookup"><span data-stu-id="455d2-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="455d2-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="455d2-160">Request</span></span>
<span data-ttu-id="455d2-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="455d2-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```

### <a name="response"></a><span data-ttu-id="455d2-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="455d2-162">Response</span></span>
<span data-ttu-id="455d2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="455d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "e8957887-7887-e895-8778-95e8877895e8",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```



