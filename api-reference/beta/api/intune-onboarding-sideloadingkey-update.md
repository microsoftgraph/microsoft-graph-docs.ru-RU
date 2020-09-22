---
title: Обновление Сиделоадингкэй
description: Обновление свойств объекта Сиделоадингкэй.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02efc04ca0d9293310e720b5119014d3a4513bee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093786"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="279bb-103">Обновление Сиделоадингкэй</span><span class="sxs-lookup"><span data-stu-id="279bb-103">Update sideLoadingKey</span></span>

<span data-ttu-id="279bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="279bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="279bb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="279bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="279bb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="279bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="279bb-107">Обновление свойств объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="279bb-107">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="279bb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="279bb-108">Prerequisites</span></span>
<span data-ttu-id="279bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="279bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="279bb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="279bb-111">Permission type</span></span>|<span data-ttu-id="279bb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="279bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="279bb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="279bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="279bb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="279bb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="279bb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="279bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="279bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="279bb-116">Not supported.</span></span>|
|<span data-ttu-id="279bb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="279bb-117">Application</span></span>|<span data-ttu-id="279bb-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="279bb-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="279bb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="279bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="279bb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="279bb-120">Request headers</span></span>
|<span data-ttu-id="279bb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="279bb-121">Header</span></span>|<span data-ttu-id="279bb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="279bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="279bb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="279bb-123">Authorization</span></span>|<span data-ttu-id="279bb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="279bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="279bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="279bb-125">Accept</span></span>|<span data-ttu-id="279bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="279bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="279bb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="279bb-127">Request body</span></span>
<span data-ttu-id="279bb-128">В тексте запроса добавьте представление объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="279bb-128">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="279bb-129">В следующей таблице приведены свойства, необходимые при создании [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md).</span><span class="sxs-lookup"><span data-stu-id="279bb-129">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="279bb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="279bb-130">Property</span></span>|<span data-ttu-id="279bb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="279bb-131">Type</span></span>|<span data-ttu-id="279bb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="279bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="279bb-133">id</span><span class="sxs-lookup"><span data-stu-id="279bb-133">id</span></span>|<span data-ttu-id="279bb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="279bb-134">String</span></span>|<span data-ttu-id="279bb-135">Уникальный идентификатор ключа загрузки на стороне.</span><span class="sxs-lookup"><span data-stu-id="279bb-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="279bb-136">value</span><span class="sxs-lookup"><span data-stu-id="279bb-136">value</span></span>|<span data-ttu-id="279bb-137">String</span><span class="sxs-lookup"><span data-stu-id="279bb-137">String</span></span>|<span data-ttu-id="279bb-138">Значение ключа загрузки на стороне, это значение 5x5, разделенное хифенс.</span><span class="sxs-lookup"><span data-stu-id="279bb-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="279bb-139">displayName</span><span class="sxs-lookup"><span data-stu-id="279bb-139">displayName</span></span>|<span data-ttu-id="279bb-140">Строка</span><span class="sxs-lookup"><span data-stu-id="279bb-140">String</span></span>|<span data-ttu-id="279bb-141">Имя ключа загрузки на стороне, отображаемое для администраторов ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="279bb-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="279bb-142">description</span><span class="sxs-lookup"><span data-stu-id="279bb-142">description</span></span>|<span data-ttu-id="279bb-143">Строка</span><span class="sxs-lookup"><span data-stu-id="279bb-143">String</span></span>|<span data-ttu-id="279bb-144">Описание ключа загрузки на стороне, которое отображается для администраторов ИТ-специалистов..</span><span class="sxs-lookup"><span data-stu-id="279bb-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="279bb-145">тоталактиватион</span><span class="sxs-lookup"><span data-stu-id="279bb-145">totalActivation</span></span>|<span data-ttu-id="279bb-146">Int32</span><span class="sxs-lookup"><span data-stu-id="279bb-146">Int32</span></span>|<span data-ttu-id="279bb-147">Клавиша загрузки на боковой стороне общая активация отображается для администраторов ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="279bb-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="279bb-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="279bb-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="279bb-149">Строка</span><span class="sxs-lookup"><span data-stu-id="279bb-149">String</span></span>|<span data-ttu-id="279bb-150">Клавиша загрузки на боковой стороне Дата последнего обновления отображается для администраторов ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="279bb-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="279bb-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="279bb-151">Response</span></span>
<span data-ttu-id="279bb-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="279bb-152">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="279bb-153">Пример</span><span class="sxs-lookup"><span data-stu-id="279bb-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="279bb-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="279bb-154">Request</span></span>
<span data-ttu-id="279bb-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="279bb-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="279bb-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="279bb-156">Response</span></span>
<span data-ttu-id="279bb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="279bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```






