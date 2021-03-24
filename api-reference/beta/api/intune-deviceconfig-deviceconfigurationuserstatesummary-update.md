---
title: Обновление устройстваConfigurationUserStateSummary
description: Обновление свойств объекта deviceConfigurationUserStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8458c2f82562454c16dd73e584de5609a6e8393
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130086"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="3f107-103">Обновление устройстваConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="3f107-103">Update deviceConfigurationUserStateSummary</span></span>

<span data-ttu-id="3f107-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f107-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f107-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f107-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f107-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f107-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f107-107">Обновление свойств объекта [deviceConfigurationUserStateSummary.](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="3f107-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f107-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3f107-108">Prerequisites</span></span>
<span data-ttu-id="3f107-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f107-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f107-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f107-111">Permission type</span></span>|<span data-ttu-id="3f107-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f107-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f107-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f107-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f107-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f107-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f107-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f107-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f107-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f107-116">Not supported.</span></span>|
|<span data-ttu-id="3f107-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3f107-117">Application</span></span>|<span data-ttu-id="3f107-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f107-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f107-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f107-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="3f107-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3f107-120">Request headers</span></span>
|<span data-ttu-id="3f107-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f107-121">Header</span></span>|<span data-ttu-id="3f107-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3f107-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f107-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f107-123">Authorization</span></span>|<span data-ttu-id="3f107-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f107-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f107-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f107-125">Accept</span></span>|<span data-ttu-id="3f107-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f107-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f107-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f107-127">Request body</span></span>
<span data-ttu-id="3f107-128">В корпусе запроса поставляем представление JSON для [объекта deviceConfigurationUserStateSummary.](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="3f107-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="3f107-129">В следующей таблице показаны свойства, необходимые при создании [устройстваConfigurationUserStateSummary.](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="3f107-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="3f107-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f107-130">Property</span></span>|<span data-ttu-id="3f107-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3f107-131">Type</span></span>|<span data-ttu-id="3f107-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3f107-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f107-133">id</span><span class="sxs-lookup"><span data-stu-id="3f107-133">id</span></span>|<span data-ttu-id="3f107-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3f107-134">String</span></span>|<span data-ttu-id="3f107-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3f107-135">Key of the entity.</span></span>|
|<span data-ttu-id="3f107-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="3f107-136">unknownUserCount</span></span>|<span data-ttu-id="3f107-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3f107-137">Int32</span></span>|<span data-ttu-id="3f107-138">Число неизвестных пользователей</span><span class="sxs-lookup"><span data-stu-id="3f107-138">Number of unknown users</span></span>|
|<span data-ttu-id="3f107-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="3f107-139">notApplicableUserCount</span></span>|<span data-ttu-id="3f107-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3f107-140">Int32</span></span>|<span data-ttu-id="3f107-141">Число не применимых пользователей</span><span class="sxs-lookup"><span data-stu-id="3f107-141">Number of not applicable users</span></span>|
|<span data-ttu-id="3f107-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="3f107-142">compliantUserCount</span></span>|<span data-ttu-id="3f107-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3f107-143">Int32</span></span>|<span data-ttu-id="3f107-144">Количество совместимых пользователей</span><span class="sxs-lookup"><span data-stu-id="3f107-144">Number of compliant users</span></span>|
|<span data-ttu-id="3f107-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="3f107-145">remediatedUserCount</span></span>|<span data-ttu-id="3f107-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3f107-146">Int32</span></span>|<span data-ttu-id="3f107-147">Число исправленных пользователей</span><span class="sxs-lookup"><span data-stu-id="3f107-147">Number of remediated users</span></span>|
|<span data-ttu-id="3f107-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="3f107-148">nonCompliantUserCount</span></span>|<span data-ttu-id="3f107-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3f107-149">Int32</span></span>|<span data-ttu-id="3f107-150">Число некомплиентных пользователей</span><span class="sxs-lookup"><span data-stu-id="3f107-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="3f107-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="3f107-151">errorUserCount</span></span>|<span data-ttu-id="3f107-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3f107-152">Int32</span></span>|<span data-ttu-id="3f107-153">Число пользователей ошибок</span><span class="sxs-lookup"><span data-stu-id="3f107-153">Number of error users</span></span>|
|<span data-ttu-id="3f107-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="3f107-154">conflictUserCount</span></span>|<span data-ttu-id="3f107-155">Int32</span><span class="sxs-lookup"><span data-stu-id="3f107-155">Int32</span></span>|<span data-ttu-id="3f107-156">Число пользователей конфликтов</span><span class="sxs-lookup"><span data-stu-id="3f107-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="3f107-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f107-157">Response</span></span>
<span data-ttu-id="3f107-158">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3f107-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f107-159">Пример</span><span class="sxs-lookup"><span data-stu-id="3f107-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f107-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f107-160">Request</span></span>
<span data-ttu-id="3f107-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f107-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3f107-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f107-162">Response</span></span>
<span data-ttu-id="3f107-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f107-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




