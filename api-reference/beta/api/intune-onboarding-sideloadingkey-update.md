---
title: Обновление sideLoadingKey
description: Обновление свойств объекта sideLoadingKey.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 65ae9cfcb7fd2d66c8b56108929a284f26d840fa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152672"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="a286b-103">Обновление sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="a286b-103">Update sideLoadingKey</span></span>

<span data-ttu-id="a286b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a286b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a286b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a286b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a286b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a286b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a286b-107">Обновление свойств объекта [sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)</span><span class="sxs-lookup"><span data-stu-id="a286b-107">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a286b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a286b-108">Prerequisites</span></span>
<span data-ttu-id="a286b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a286b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a286b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a286b-111">Permission type</span></span>|<span data-ttu-id="a286b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a286b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a286b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a286b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a286b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a286b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a286b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a286b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a286b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a286b-116">Not supported.</span></span>|
|<span data-ttu-id="a286b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a286b-117">Application</span></span>|<span data-ttu-id="a286b-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a286b-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a286b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a286b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="a286b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a286b-120">Request headers</span></span>
|<span data-ttu-id="a286b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a286b-121">Header</span></span>|<span data-ttu-id="a286b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a286b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a286b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a286b-123">Authorization</span></span>|<span data-ttu-id="a286b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a286b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a286b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a286b-125">Accept</span></span>|<span data-ttu-id="a286b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a286b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a286b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a286b-127">Request body</span></span>
<span data-ttu-id="a286b-128">В теле запроса поставляем представление JSON для [объекта sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)</span><span class="sxs-lookup"><span data-stu-id="a286b-128">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="a286b-129">В следующей таблице показаны свойства, необходимые при создании [sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)</span><span class="sxs-lookup"><span data-stu-id="a286b-129">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="a286b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a286b-130">Property</span></span>|<span data-ttu-id="a286b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a286b-131">Type</span></span>|<span data-ttu-id="a286b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a286b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a286b-133">id</span><span class="sxs-lookup"><span data-stu-id="a286b-133">id</span></span>|<span data-ttu-id="a286b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a286b-134">String</span></span>|<span data-ttu-id="a286b-135">Уникальный ID side Loading Key.</span><span class="sxs-lookup"><span data-stu-id="a286b-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="a286b-136">value</span><span class="sxs-lookup"><span data-stu-id="a286b-136">value</span></span>|<span data-ttu-id="a286b-137">String</span><span class="sxs-lookup"><span data-stu-id="a286b-137">String</span></span>|<span data-ttu-id="a286b-138">Ключевое значение side Loading — это значение 5x5, разделенное hiphens.</span><span class="sxs-lookup"><span data-stu-id="a286b-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="a286b-139">displayName</span><span class="sxs-lookup"><span data-stu-id="a286b-139">displayName</span></span>|<span data-ttu-id="a286b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="a286b-140">String</span></span>|<span data-ttu-id="a286b-141">Имя клавиши боковой загрузки, отображаемой администраторам ITPro.</span><span class="sxs-lookup"><span data-stu-id="a286b-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="a286b-142">description</span><span class="sxs-lookup"><span data-stu-id="a286b-142">description</span></span>|<span data-ttu-id="a286b-143">Строка</span><span class="sxs-lookup"><span data-stu-id="a286b-143">String</span></span>|<span data-ttu-id="a286b-144">Описание клавиши боковой загрузки, отображаемой администраторам ITPro..</span><span class="sxs-lookup"><span data-stu-id="a286b-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="a286b-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="a286b-145">totalActivation</span></span>|<span data-ttu-id="a286b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a286b-146">Int32</span></span>|<span data-ttu-id="a286b-147">Полная активация клавиши боковой загрузки, отображаемая администраторам ITPro.</span><span class="sxs-lookup"><span data-stu-id="a286b-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="a286b-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a286b-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="a286b-149">Строка</span><span class="sxs-lookup"><span data-stu-id="a286b-149">String</span></span>|<span data-ttu-id="a286b-150">Клавиша side Loading Last Updated Date, отображаемая администраторам ITPro.</span><span class="sxs-lookup"><span data-stu-id="a286b-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="a286b-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="a286b-151">Response</span></span>
<span data-ttu-id="a286b-152">В случае успешной работы этот метод возвращает код ответа и `200 OK` обновленный [объект sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a286b-152">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a286b-153">Пример</span><span class="sxs-lookup"><span data-stu-id="a286b-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="a286b-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="a286b-154">Request</span></span>
<span data-ttu-id="a286b-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a286b-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a286b-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="a286b-156">Response</span></span>
<span data-ttu-id="a286b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a286b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




