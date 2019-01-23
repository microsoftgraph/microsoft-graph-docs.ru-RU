---
title: Обновление deviceConfigurationUserStateSummary
description: Обновление свойства объекта deviceConfigurationUserStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 425ac4f2697363f92f61bdd627172fd074bf94b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420663"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="9947d-103">Обновление deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="9947d-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="9947d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9947d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9947d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9947d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9947d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9947d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9947d-107">Обновление свойства объекта [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9947d-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9947d-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="9947d-108">Prerequisites</span></span>
<span data-ttu-id="9947d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9947d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9947d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9947d-111">Permission type</span></span>|<span data-ttu-id="9947d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9947d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9947d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9947d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9947d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9947d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9947d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9947d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9947d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9947d-116">Not supported.</span></span>|
|<span data-ttu-id="9947d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9947d-117">Application</span></span>|<span data-ttu-id="9947d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9947d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9947d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9947d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="9947d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9947d-120">Request headers</span></span>
|<span data-ttu-id="9947d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9947d-121">Header</span></span>|<span data-ttu-id="9947d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9947d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9947d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9947d-123">Authorization</span></span>|<span data-ttu-id="9947d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9947d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9947d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9947d-125">Accept</span></span>|<span data-ttu-id="9947d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9947d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9947d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9947d-127">Request body</span></span>
<span data-ttu-id="9947d-128">В тексте запроса укажите представление JSON для объекта [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9947d-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="9947d-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9947d-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="9947d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9947d-130">Property</span></span>|<span data-ttu-id="9947d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9947d-131">Type</span></span>|<span data-ttu-id="9947d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9947d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9947d-133">id</span><span class="sxs-lookup"><span data-stu-id="9947d-133">id</span></span>|<span data-ttu-id="9947d-134">String</span><span class="sxs-lookup"><span data-stu-id="9947d-134">String</span></span>|<span data-ttu-id="9947d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9947d-135">Key of the entity.</span></span>|
|<span data-ttu-id="9947d-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="9947d-136">unknownUserCount</span></span>|<span data-ttu-id="9947d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9947d-137">Int32</span></span>|<span data-ttu-id="9947d-138">Число неизвестным пользователям</span><span class="sxs-lookup"><span data-stu-id="9947d-138">Number of unknown users</span></span>|
|<span data-ttu-id="9947d-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="9947d-139">notApplicableUserCount</span></span>|<span data-ttu-id="9947d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9947d-140">Int32</span></span>|<span data-ttu-id="9947d-141">Число пользователей не применим</span><span class="sxs-lookup"><span data-stu-id="9947d-141">Number of not applicable users</span></span>|
|<span data-ttu-id="9947d-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="9947d-142">compliantUserCount</span></span>|<span data-ttu-id="9947d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9947d-143">Int32</span></span>|<span data-ttu-id="9947d-144">Количество требованиям пользователей</span><span class="sxs-lookup"><span data-stu-id="9947d-144">Number of compliant users</span></span>|
|<span data-ttu-id="9947d-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="9947d-145">remediatedUserCount</span></span>|<span data-ttu-id="9947d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9947d-146">Int32</span></span>|<span data-ttu-id="9947d-147">Количество проверка пользователей</span><span class="sxs-lookup"><span data-stu-id="9947d-147">Number of remediated users</span></span>|
|<span data-ttu-id="9947d-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="9947d-148">nonCompliantUserCount</span></span>|<span data-ttu-id="9947d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9947d-149">Int32</span></span>|<span data-ttu-id="9947d-150">Количество несовместимой пользователей</span><span class="sxs-lookup"><span data-stu-id="9947d-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="9947d-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="9947d-151">errorUserCount</span></span>|<span data-ttu-id="9947d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9947d-152">Int32</span></span>|<span data-ttu-id="9947d-153">Число пользователей об ошибках</span><span class="sxs-lookup"><span data-stu-id="9947d-153">Number of error users</span></span>|
|<span data-ttu-id="9947d-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="9947d-154">conflictUserCount</span></span>|<span data-ttu-id="9947d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="9947d-155">Int32</span></span>|<span data-ttu-id="9947d-156">Число пользователей конфликта</span><span class="sxs-lookup"><span data-stu-id="9947d-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="9947d-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="9947d-157">Response</span></span>
<span data-ttu-id="9947d-158">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9947d-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9947d-159">Пример</span><span class="sxs-lookup"><span data-stu-id="9947d-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="9947d-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="9947d-160">Request</span></span>
<span data-ttu-id="9947d-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9947d-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9947d-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="9947d-162">Response</span></span>
<span data-ttu-id="9947d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9947d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




