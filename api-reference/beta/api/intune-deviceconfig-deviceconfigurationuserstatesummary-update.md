---
title: Обновление Девицеконфигуратионусерстатесуммари
description: Обновление свойств объекта Девицеконфигуратионусерстатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc833a4e49db0048430a359d09fe857b571cd35a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967505"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="44074-103">Обновление Девицеконфигуратионусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="44074-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="44074-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44074-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44074-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44074-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44074-106">Обновление свойств объекта [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="44074-106">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44074-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="44074-107">Prerequisites</span></span>
<span data-ttu-id="44074-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44074-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44074-110">Permission type</span></span>|<span data-ttu-id="44074-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44074-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44074-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44074-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44074-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44074-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44074-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44074-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44074-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44074-115">Not supported.</span></span>|
|<span data-ttu-id="44074-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44074-116">Application</span></span>|<span data-ttu-id="44074-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44074-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44074-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44074-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="44074-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44074-119">Request headers</span></span>
|<span data-ttu-id="44074-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44074-120">Header</span></span>|<span data-ttu-id="44074-121">Значение</span><span class="sxs-lookup"><span data-stu-id="44074-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44074-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44074-122">Authorization</span></span>|<span data-ttu-id="44074-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44074-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44074-124">Accept</span><span class="sxs-lookup"><span data-stu-id="44074-124">Accept</span></span>|<span data-ttu-id="44074-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44074-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44074-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44074-126">Request body</span></span>
<span data-ttu-id="44074-127">В тексте запроса добавьте представление объекта [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44074-127">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="44074-128">В следующей таблице приведены свойства, необходимые при создании [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="44074-128">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="44074-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="44074-129">Property</span></span>|<span data-ttu-id="44074-130">Тип</span><span class="sxs-lookup"><span data-stu-id="44074-130">Type</span></span>|<span data-ttu-id="44074-131">Описание</span><span class="sxs-lookup"><span data-stu-id="44074-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44074-132">id</span><span class="sxs-lookup"><span data-stu-id="44074-132">id</span></span>|<span data-ttu-id="44074-133">String</span><span class="sxs-lookup"><span data-stu-id="44074-133">String</span></span>|<span data-ttu-id="44074-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="44074-134">Key of the entity.</span></span>|
|<span data-ttu-id="44074-135">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="44074-135">unknownUserCount</span></span>|<span data-ttu-id="44074-136">Int32</span><span class="sxs-lookup"><span data-stu-id="44074-136">Int32</span></span>|<span data-ttu-id="44074-137">Количество неизвестных пользователей</span><span class="sxs-lookup"><span data-stu-id="44074-137">Number of unknown users</span></span>|
|<span data-ttu-id="44074-138">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="44074-138">notApplicableUserCount</span></span>|<span data-ttu-id="44074-139">Int32</span><span class="sxs-lookup"><span data-stu-id="44074-139">Int32</span></span>|<span data-ttu-id="44074-140">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="44074-140">Number of not applicable users</span></span>|
|<span data-ttu-id="44074-141">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="44074-141">compliantUserCount</span></span>|<span data-ttu-id="44074-142">Int32</span><span class="sxs-lookup"><span data-stu-id="44074-142">Int32</span></span>|<span data-ttu-id="44074-143">Число соответствующих пользователей</span><span class="sxs-lookup"><span data-stu-id="44074-143">Number of compliant users</span></span>|
|<span data-ttu-id="44074-144">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="44074-144">remediatedUserCount</span></span>|<span data-ttu-id="44074-145">Int32</span><span class="sxs-lookup"><span data-stu-id="44074-145">Int32</span></span>|<span data-ttu-id="44074-146">Количество исправленных пользователей</span><span class="sxs-lookup"><span data-stu-id="44074-146">Number of remediated users</span></span>|
|<span data-ttu-id="44074-147">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="44074-147">nonCompliantUserCount</span></span>|<span data-ttu-id="44074-148">Int32</span><span class="sxs-lookup"><span data-stu-id="44074-148">Int32</span></span>|<span data-ttu-id="44074-149">Количество несоответствующих пользователей</span><span class="sxs-lookup"><span data-stu-id="44074-149">Number of NonCompliant users</span></span>|
|<span data-ttu-id="44074-150">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="44074-150">errorUserCount</span></span>|<span data-ttu-id="44074-151">Int32</span><span class="sxs-lookup"><span data-stu-id="44074-151">Int32</span></span>|<span data-ttu-id="44074-152">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="44074-152">Number of error users</span></span>|
|<span data-ttu-id="44074-153">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="44074-153">conflictUserCount</span></span>|<span data-ttu-id="44074-154">Int32</span><span class="sxs-lookup"><span data-stu-id="44074-154">Int32</span></span>|<span data-ttu-id="44074-155">Количество конфликтующих пользователей</span><span class="sxs-lookup"><span data-stu-id="44074-155">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="44074-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="44074-156">Response</span></span>
<span data-ttu-id="44074-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44074-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44074-158">Пример</span><span class="sxs-lookup"><span data-stu-id="44074-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="44074-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="44074-159">Request</span></span>
<span data-ttu-id="44074-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44074-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="44074-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="44074-161">Response</span></span>
<span data-ttu-id="44074-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44074-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





