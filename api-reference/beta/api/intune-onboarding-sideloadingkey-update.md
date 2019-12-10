---
title: Обновление Сиделоадингкэй
description: Обновление свойств объекта Сиделоадингкэй.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 185da7bfe48ca8d2cf9b74ac1ca32b95c7ae2de1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941542"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="4ae2d-103">Обновление Сиделоадингкэй</span><span class="sxs-lookup"><span data-stu-id="4ae2d-103">Update sideLoadingKey</span></span>

> <span data-ttu-id="4ae2d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ae2d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ae2d-106">Обновление свойств объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="4ae2d-106">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ae2d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4ae2d-107">Prerequisites</span></span>
<span data-ttu-id="4ae2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ae2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ae2d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ae2d-110">Permission type</span></span>|<span data-ttu-id="4ae2d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ae2d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ae2d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ae2d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ae2d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ae2d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4ae2d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ae2d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ae2d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-115">Not supported.</span></span>|
|<span data-ttu-id="4ae2d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ae2d-116">Application</span></span>|<span data-ttu-id="4ae2d-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ae2d-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ae2d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ae2d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="4ae2d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4ae2d-119">Request headers</span></span>
|<span data-ttu-id="4ae2d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ae2d-120">Header</span></span>|<span data-ttu-id="4ae2d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4ae2d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ae2d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ae2d-122">Authorization</span></span>|<span data-ttu-id="4ae2d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ae2d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4ae2d-124">Accept</span></span>|<span data-ttu-id="4ae2d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ae2d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ae2d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4ae2d-126">Request body</span></span>
<span data-ttu-id="4ae2d-127">В тексте запроса добавьте представление объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-127">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="4ae2d-128">В следующей таблице приведены свойства, необходимые при создании [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md).</span><span class="sxs-lookup"><span data-stu-id="4ae2d-128">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="4ae2d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ae2d-129">Property</span></span>|<span data-ttu-id="4ae2d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4ae2d-130">Type</span></span>|<span data-ttu-id="4ae2d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4ae2d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ae2d-132">id</span><span class="sxs-lookup"><span data-stu-id="4ae2d-132">id</span></span>|<span data-ttu-id="4ae2d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4ae2d-133">String</span></span>|<span data-ttu-id="4ae2d-134">Уникальный идентификатор ключа загрузки на стороне.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-134">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="4ae2d-135">value</span><span class="sxs-lookup"><span data-stu-id="4ae2d-135">value</span></span>|<span data-ttu-id="4ae2d-136">String</span><span class="sxs-lookup"><span data-stu-id="4ae2d-136">String</span></span>|<span data-ttu-id="4ae2d-137">Значение ключа загрузки на стороне, это значение 5x5, разделенное хифенс.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-137">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="4ae2d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="4ae2d-138">displayName</span></span>|<span data-ttu-id="4ae2d-139">Строка</span><span class="sxs-lookup"><span data-stu-id="4ae2d-139">String</span></span>|<span data-ttu-id="4ae2d-140">Имя ключа загрузки на стороне, отображаемое для администраторов ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-140">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="4ae2d-141">description</span><span class="sxs-lookup"><span data-stu-id="4ae2d-141">description</span></span>|<span data-ttu-id="4ae2d-142">String</span><span class="sxs-lookup"><span data-stu-id="4ae2d-142">String</span></span>|<span data-ttu-id="4ae2d-143">Описание ключа загрузки на стороне, которое отображается для администраторов ИТ-специалистов..</span><span class="sxs-lookup"><span data-stu-id="4ae2d-143">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="4ae2d-144">тоталактиватион</span><span class="sxs-lookup"><span data-stu-id="4ae2d-144">totalActivation</span></span>|<span data-ttu-id="4ae2d-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4ae2d-145">Int32</span></span>|<span data-ttu-id="4ae2d-146">Клавиша загрузки на боковой стороне общая активация отображается для администраторов ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-146">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="4ae2d-147">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ae2d-147">lastUpdatedDateTime</span></span>|<span data-ttu-id="4ae2d-148">Строка</span><span class="sxs-lookup"><span data-stu-id="4ae2d-148">String</span></span>|<span data-ttu-id="4ae2d-149">Клавиша загрузки на боковой стороне Дата последнего обновления отображается для администраторов ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-149">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="4ae2d-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ae2d-150">Response</span></span>
<span data-ttu-id="4ae2d-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-151">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ae2d-152">Пример</span><span class="sxs-lookup"><span data-stu-id="4ae2d-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ae2d-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ae2d-153">Request</span></span>
<span data-ttu-id="4ae2d-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4ae2d-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ae2d-155">Response</span></span>
<span data-ttu-id="4ae2d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





