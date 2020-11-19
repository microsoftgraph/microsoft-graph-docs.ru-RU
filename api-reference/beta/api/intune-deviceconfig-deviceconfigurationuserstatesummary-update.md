---
title: Обновление Девицеконфигуратионусерстатесуммари
description: Обновление свойств объекта Девицеконфигуратионусерстатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 553447bfd38ead0577b0a88726894419a6ee1597
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49291402"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="90047-103">Обновление Девицеконфигуратионусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="90047-103">Update deviceConfigurationUserStateSummary</span></span>

<span data-ttu-id="90047-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90047-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90047-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90047-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90047-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90047-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90047-107">Обновление свойств объекта [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="90047-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90047-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="90047-108">Prerequisites</span></span>
<span data-ttu-id="90047-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90047-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90047-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90047-111">Permission type</span></span>|<span data-ttu-id="90047-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90047-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90047-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90047-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90047-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90047-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90047-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90047-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90047-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90047-116">Not supported.</span></span>|
|<span data-ttu-id="90047-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90047-117">Application</span></span>|<span data-ttu-id="90047-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90047-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90047-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90047-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="90047-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="90047-120">Request headers</span></span>
|<span data-ttu-id="90047-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90047-121">Header</span></span>|<span data-ttu-id="90047-122">Значение</span><span class="sxs-lookup"><span data-stu-id="90047-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90047-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90047-123">Authorization</span></span>|<span data-ttu-id="90047-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90047-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90047-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90047-125">Accept</span></span>|<span data-ttu-id="90047-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90047-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90047-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90047-127">Request body</span></span>
<span data-ttu-id="90047-128">В тексте запроса добавьте представление объекта [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90047-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="90047-129">В следующей таблице приведены свойства, необходимые при создании [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="90047-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="90047-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="90047-130">Property</span></span>|<span data-ttu-id="90047-131">Тип</span><span class="sxs-lookup"><span data-stu-id="90047-131">Type</span></span>|<span data-ttu-id="90047-132">Описание</span><span class="sxs-lookup"><span data-stu-id="90047-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90047-133">id</span><span class="sxs-lookup"><span data-stu-id="90047-133">id</span></span>|<span data-ttu-id="90047-134">String</span><span class="sxs-lookup"><span data-stu-id="90047-134">String</span></span>|<span data-ttu-id="90047-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="90047-135">Key of the entity.</span></span>|
|<span data-ttu-id="90047-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="90047-136">unknownUserCount</span></span>|<span data-ttu-id="90047-137">Int32</span><span class="sxs-lookup"><span data-stu-id="90047-137">Int32</span></span>|<span data-ttu-id="90047-138">Количество неизвестных пользователей</span><span class="sxs-lookup"><span data-stu-id="90047-138">Number of unknown users</span></span>|
|<span data-ttu-id="90047-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="90047-139">notApplicableUserCount</span></span>|<span data-ttu-id="90047-140">Int32</span><span class="sxs-lookup"><span data-stu-id="90047-140">Int32</span></span>|<span data-ttu-id="90047-141">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="90047-141">Number of not applicable users</span></span>|
|<span data-ttu-id="90047-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="90047-142">compliantUserCount</span></span>|<span data-ttu-id="90047-143">Int32</span><span class="sxs-lookup"><span data-stu-id="90047-143">Int32</span></span>|<span data-ttu-id="90047-144">Число соответствующих пользователей</span><span class="sxs-lookup"><span data-stu-id="90047-144">Number of compliant users</span></span>|
|<span data-ttu-id="90047-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="90047-145">remediatedUserCount</span></span>|<span data-ttu-id="90047-146">Int32</span><span class="sxs-lookup"><span data-stu-id="90047-146">Int32</span></span>|<span data-ttu-id="90047-147">Количество исправленных пользователей</span><span class="sxs-lookup"><span data-stu-id="90047-147">Number of remediated users</span></span>|
|<span data-ttu-id="90047-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="90047-148">nonCompliantUserCount</span></span>|<span data-ttu-id="90047-149">Int32</span><span class="sxs-lookup"><span data-stu-id="90047-149">Int32</span></span>|<span data-ttu-id="90047-150">Количество несоответствующих пользователей</span><span class="sxs-lookup"><span data-stu-id="90047-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="90047-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="90047-151">errorUserCount</span></span>|<span data-ttu-id="90047-152">Int32</span><span class="sxs-lookup"><span data-stu-id="90047-152">Int32</span></span>|<span data-ttu-id="90047-153">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="90047-153">Number of error users</span></span>|
|<span data-ttu-id="90047-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="90047-154">conflictUserCount</span></span>|<span data-ttu-id="90047-155">Int32</span><span class="sxs-lookup"><span data-stu-id="90047-155">Int32</span></span>|<span data-ttu-id="90047-156">Количество конфликтующих пользователей</span><span class="sxs-lookup"><span data-stu-id="90047-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="90047-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="90047-157">Response</span></span>
<span data-ttu-id="90047-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90047-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90047-159">Пример</span><span class="sxs-lookup"><span data-stu-id="90047-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="90047-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="90047-160">Request</span></span>
<span data-ttu-id="90047-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90047-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="90047-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="90047-162">Response</span></span>
<span data-ttu-id="90047-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90047-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




