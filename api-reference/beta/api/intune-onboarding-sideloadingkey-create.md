---
title: Создание sideLoadingKey
description: Создайте новый объект sideLoadingKey.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a484745aae11ba967f3077bf674c9bc8dd8c6db
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148745"
---
# <a name="create-sideloadingkey"></a><span data-ttu-id="ea39d-103">Создание sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="ea39d-103">Create sideLoadingKey</span></span>

<span data-ttu-id="ea39d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea39d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea39d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea39d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea39d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea39d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea39d-107">Создайте новый [объект sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)</span><span class="sxs-lookup"><span data-stu-id="ea39d-107">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea39d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea39d-108">Prerequisites</span></span>
<span data-ttu-id="ea39d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea39d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea39d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea39d-111">Permission type</span></span>|<span data-ttu-id="ea39d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea39d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea39d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea39d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea39d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea39d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ea39d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea39d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea39d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea39d-116">Not supported.</span></span>|
|<span data-ttu-id="ea39d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ea39d-117">Application</span></span>|<span data-ttu-id="ea39d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea39d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea39d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea39d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="ea39d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ea39d-120">Request headers</span></span>
|<span data-ttu-id="ea39d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea39d-121">Header</span></span>|<span data-ttu-id="ea39d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ea39d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea39d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea39d-123">Authorization</span></span>|<span data-ttu-id="ea39d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea39d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea39d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ea39d-125">Accept</span></span>|<span data-ttu-id="ea39d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea39d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea39d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea39d-127">Request body</span></span>
<span data-ttu-id="ea39d-128">В теле запроса поставляем представление JSON для объекта sideLoadingKey.</span><span class="sxs-lookup"><span data-stu-id="ea39d-128">In the request body, supply a JSON representation for the sideLoadingKey object.</span></span>

<span data-ttu-id="ea39d-129">В следующей таблице показаны свойства, необходимые при создании sideLoadingKey.</span><span class="sxs-lookup"><span data-stu-id="ea39d-129">The following table shows the properties that are required when you create the sideLoadingKey.</span></span>

|<span data-ttu-id="ea39d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea39d-130">Property</span></span>|<span data-ttu-id="ea39d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ea39d-131">Type</span></span>|<span data-ttu-id="ea39d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ea39d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea39d-133">id</span><span class="sxs-lookup"><span data-stu-id="ea39d-133">id</span></span>|<span data-ttu-id="ea39d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ea39d-134">String</span></span>|<span data-ttu-id="ea39d-135">Уникальный ID side Loading Key.</span><span class="sxs-lookup"><span data-stu-id="ea39d-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="ea39d-136">value</span><span class="sxs-lookup"><span data-stu-id="ea39d-136">value</span></span>|<span data-ttu-id="ea39d-137">String</span><span class="sxs-lookup"><span data-stu-id="ea39d-137">String</span></span>|<span data-ttu-id="ea39d-138">Ключевое значение side Loading — это значение 5x5, разделенное hiphens.</span><span class="sxs-lookup"><span data-stu-id="ea39d-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="ea39d-139">displayName</span><span class="sxs-lookup"><span data-stu-id="ea39d-139">displayName</span></span>|<span data-ttu-id="ea39d-140">Строка</span><span class="sxs-lookup"><span data-stu-id="ea39d-140">String</span></span>|<span data-ttu-id="ea39d-141">Имя клавиши боковой загрузки, отображаемой администраторам ITPro.</span><span class="sxs-lookup"><span data-stu-id="ea39d-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="ea39d-142">description</span><span class="sxs-lookup"><span data-stu-id="ea39d-142">description</span></span>|<span data-ttu-id="ea39d-143">Строка</span><span class="sxs-lookup"><span data-stu-id="ea39d-143">String</span></span>|<span data-ttu-id="ea39d-144">Описание клавиши боковой загрузки, отображаемой администраторам ITPro..</span><span class="sxs-lookup"><span data-stu-id="ea39d-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="ea39d-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="ea39d-145">totalActivation</span></span>|<span data-ttu-id="ea39d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ea39d-146">Int32</span></span>|<span data-ttu-id="ea39d-147">Полная активация клавиши боковой загрузки, отображаемая администраторам ITPro.</span><span class="sxs-lookup"><span data-stu-id="ea39d-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="ea39d-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea39d-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="ea39d-149">Строка</span><span class="sxs-lookup"><span data-stu-id="ea39d-149">String</span></span>|<span data-ttu-id="ea39d-150">Клавиша side Loading Last Updated Date, отображаемая администраторам ITPro.</span><span class="sxs-lookup"><span data-stu-id="ea39d-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="ea39d-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea39d-151">Response</span></span>
<span data-ttu-id="ea39d-152">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ea39d-152">If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea39d-153">Пример</span><span class="sxs-lookup"><span data-stu-id="ea39d-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea39d-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea39d-154">Request</span></span>
<span data-ttu-id="ea39d-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea39d-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
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

### <a name="response"></a><span data-ttu-id="ea39d-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea39d-156">Response</span></span>
<span data-ttu-id="ea39d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea39d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




