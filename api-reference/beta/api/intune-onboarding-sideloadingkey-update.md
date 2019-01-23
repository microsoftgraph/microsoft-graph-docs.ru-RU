---
title: Обновление sideLoadingKey
description: Обновление свойства объекта sideLoadingKey.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4fd498404543353c45714f739a68b0195ae3d3dd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409862"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="e919b-103">Обновление sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="e919b-103">Update sideLoadingKey</span></span>

> <span data-ttu-id="e919b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e919b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e919b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e919b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e919b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e919b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e919b-107">Обновление свойства объекта [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="e919b-107">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e919b-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="e919b-108">Prerequisites</span></span>
<span data-ttu-id="e919b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e919b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e919b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e919b-111">Permission type</span></span>|<span data-ttu-id="e919b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e919b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e919b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e919b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e919b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e919b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e919b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e919b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e919b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e919b-116">Not supported.</span></span>|
|<span data-ttu-id="e919b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e919b-117">Application</span></span>|<span data-ttu-id="e919b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e919b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e919b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e919b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="e919b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e919b-120">Request headers</span></span>
|<span data-ttu-id="e919b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e919b-121">Header</span></span>|<span data-ttu-id="e919b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e919b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e919b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e919b-123">Authorization</span></span>|<span data-ttu-id="e919b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e919b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e919b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e919b-125">Accept</span></span>|<span data-ttu-id="e919b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e919b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e919b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e919b-127">Request body</span></span>
<span data-ttu-id="e919b-128">В тексте запроса укажите представление JSON для объекта [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="e919b-128">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="e919b-129">В следующей таблице показаны свойства, которые необходимы для создания [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span><span class="sxs-lookup"><span data-stu-id="e919b-129">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="e919b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e919b-130">Property</span></span>|<span data-ttu-id="e919b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e919b-131">Type</span></span>|<span data-ttu-id="e919b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e919b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e919b-133">id</span><span class="sxs-lookup"><span data-stu-id="e919b-133">id</span></span>|<span data-ttu-id="e919b-134">String</span><span class="sxs-lookup"><span data-stu-id="e919b-134">String</span></span>|<span data-ttu-id="e919b-135">Со стороны загрузка уникальный идентификатор ключа.</span><span class="sxs-lookup"><span data-stu-id="e919b-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="e919b-136">value</span><span class="sxs-lookup"><span data-stu-id="e919b-136">value</span></span>|<span data-ttu-id="e919b-137">String</span><span class="sxs-lookup"><span data-stu-id="e919b-137">String</span></span>|<span data-ttu-id="e919b-138">Со стороны загрузки ключ значение — значение 5 x 5, разделенных hiphens.</span><span class="sxs-lookup"><span data-stu-id="e919b-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="e919b-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e919b-139">displayName</span></span>|<span data-ttu-id="e919b-140">String</span><span class="sxs-lookup"><span data-stu-id="e919b-140">String</span></span>|<span data-ttu-id="e919b-141">Со стороны загрузка ключа имя, отображаемое для администраторов для ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="e919b-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="e919b-142">description</span><span class="sxs-lookup"><span data-stu-id="e919b-142">description</span></span>|<span data-ttu-id="e919b-143">String</span><span class="sxs-lookup"><span data-stu-id="e919b-143">String</span></span>|<span data-ttu-id="e919b-144">Со стороны загрузки ключ описание, отображаемое для администраторов для ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="e919b-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="e919b-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="e919b-145">totalActivation</span></span>|<span data-ttu-id="e919b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e919b-146">Int32</span></span>|<span data-ttu-id="e919b-147">Со стороны загрузки ключ общее активация отображаются для администраторов для ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="e919b-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="e919b-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e919b-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="e919b-149">String</span><span class="sxs-lookup"><span data-stu-id="e919b-149">String</span></span>|<span data-ttu-id="e919b-150">Со стороны загрузки ключ обновлен Дата последнего отображаются для администраторов для ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="e919b-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="e919b-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="e919b-151">Response</span></span>
<span data-ttu-id="e919b-152">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e919b-152">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e919b-153">Пример</span><span class="sxs-lookup"><span data-stu-id="e919b-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="e919b-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="e919b-154">Request</span></span>
<span data-ttu-id="e919b-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e919b-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e919b-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="e919b-156">Response</span></span>
<span data-ttu-id="e919b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e919b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




