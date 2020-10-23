---
title: Обновление Девицеконфигуратионусерстатесуммари
description: Обновление свойств объекта Девицеконфигуратионусерстатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aadb068c2511192cc341404a43dc60b957b0210b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731290"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="01733-103">Обновление Девицеконфигуратионусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="01733-103">Update deviceConfigurationUserStateSummary</span></span>

<span data-ttu-id="01733-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01733-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01733-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01733-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01733-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01733-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01733-107">Обновление свойств объекта [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="01733-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01733-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01733-108">Prerequisites</span></span>
<span data-ttu-id="01733-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01733-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01733-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01733-111">Permission type</span></span>|<span data-ttu-id="01733-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01733-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01733-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01733-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01733-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01733-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01733-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01733-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01733-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01733-116">Not supported.</span></span>|
|<span data-ttu-id="01733-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01733-117">Application</span></span>|<span data-ttu-id="01733-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01733-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01733-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01733-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="01733-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="01733-120">Request headers</span></span>
|<span data-ttu-id="01733-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01733-121">Header</span></span>|<span data-ttu-id="01733-122">Значение</span><span class="sxs-lookup"><span data-stu-id="01733-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01733-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01733-123">Authorization</span></span>|<span data-ttu-id="01733-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01733-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01733-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01733-125">Accept</span></span>|<span data-ttu-id="01733-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01733-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01733-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01733-127">Request body</span></span>
<span data-ttu-id="01733-128">В тексте запроса добавьте представление объекта [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01733-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="01733-129">В следующей таблице приведены свойства, необходимые при создании [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="01733-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="01733-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="01733-130">Property</span></span>|<span data-ttu-id="01733-131">Тип</span><span class="sxs-lookup"><span data-stu-id="01733-131">Type</span></span>|<span data-ttu-id="01733-132">Описание</span><span class="sxs-lookup"><span data-stu-id="01733-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01733-133">id</span><span class="sxs-lookup"><span data-stu-id="01733-133">id</span></span>|<span data-ttu-id="01733-134">Строка</span><span class="sxs-lookup"><span data-stu-id="01733-134">String</span></span>|<span data-ttu-id="01733-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="01733-135">Key of the entity.</span></span>|
|<span data-ttu-id="01733-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="01733-136">unknownUserCount</span></span>|<span data-ttu-id="01733-137">Int32</span><span class="sxs-lookup"><span data-stu-id="01733-137">Int32</span></span>|<span data-ttu-id="01733-138">Количество неизвестных пользователей</span><span class="sxs-lookup"><span data-stu-id="01733-138">Number of unknown users</span></span>|
|<span data-ttu-id="01733-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="01733-139">notApplicableUserCount</span></span>|<span data-ttu-id="01733-140">Int32</span><span class="sxs-lookup"><span data-stu-id="01733-140">Int32</span></span>|<span data-ttu-id="01733-141">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="01733-141">Number of not applicable users</span></span>|
|<span data-ttu-id="01733-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="01733-142">compliantUserCount</span></span>|<span data-ttu-id="01733-143">Int32</span><span class="sxs-lookup"><span data-stu-id="01733-143">Int32</span></span>|<span data-ttu-id="01733-144">Число соответствующих пользователей</span><span class="sxs-lookup"><span data-stu-id="01733-144">Number of compliant users</span></span>|
|<span data-ttu-id="01733-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="01733-145">remediatedUserCount</span></span>|<span data-ttu-id="01733-146">Int32</span><span class="sxs-lookup"><span data-stu-id="01733-146">Int32</span></span>|<span data-ttu-id="01733-147">Количество исправленных пользователей</span><span class="sxs-lookup"><span data-stu-id="01733-147">Number of remediated users</span></span>|
|<span data-ttu-id="01733-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="01733-148">nonCompliantUserCount</span></span>|<span data-ttu-id="01733-149">Int32</span><span class="sxs-lookup"><span data-stu-id="01733-149">Int32</span></span>|<span data-ttu-id="01733-150">Количество несоответствующих пользователей</span><span class="sxs-lookup"><span data-stu-id="01733-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="01733-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="01733-151">errorUserCount</span></span>|<span data-ttu-id="01733-152">Int32</span><span class="sxs-lookup"><span data-stu-id="01733-152">Int32</span></span>|<span data-ttu-id="01733-153">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="01733-153">Number of error users</span></span>|
|<span data-ttu-id="01733-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="01733-154">conflictUserCount</span></span>|<span data-ttu-id="01733-155">Int32</span><span class="sxs-lookup"><span data-stu-id="01733-155">Int32</span></span>|<span data-ttu-id="01733-156">Количество конфликтующих пользователей</span><span class="sxs-lookup"><span data-stu-id="01733-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="01733-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="01733-157">Response</span></span>
<span data-ttu-id="01733-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01733-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01733-159">Пример</span><span class="sxs-lookup"><span data-stu-id="01733-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="01733-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="01733-160">Request</span></span>
<span data-ttu-id="01733-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01733-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01733-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="01733-162">Response</span></span>
<span data-ttu-id="01733-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01733-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





