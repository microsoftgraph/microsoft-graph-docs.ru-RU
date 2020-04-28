---
title: Создание Сиделоадингкэй
description: Создание нового объекта Сиделоадингкэй.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0591e70f624d73ca6de2b2779b31b5610d7a9613
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448728"
---
# <a name="create-sideloadingkey"></a><span data-ttu-id="1e515-103">Создание Сиделоадингкэй</span><span class="sxs-lookup"><span data-stu-id="1e515-103">Create sideLoadingKey</span></span>

<span data-ttu-id="1e515-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e515-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e515-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e515-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e515-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e515-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e515-107">Создание нового объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="1e515-107">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e515-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1e515-108">Prerequisites</span></span>
<span data-ttu-id="1e515-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e515-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e515-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e515-111">Permission type</span></span>|<span data-ttu-id="1e515-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e515-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e515-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e515-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e515-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e515-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1e515-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e515-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e515-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e515-116">Not supported.</span></span>|
|<span data-ttu-id="1e515-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e515-117">Application</span></span>|<span data-ttu-id="1e515-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e515-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e515-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e515-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="1e515-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1e515-120">Request headers</span></span>
|<span data-ttu-id="1e515-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e515-121">Header</span></span>|<span data-ttu-id="1e515-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1e515-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e515-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e515-123">Authorization</span></span>|<span data-ttu-id="1e515-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e515-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e515-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e515-125">Accept</span></span>|<span data-ttu-id="1e515-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e515-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e515-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1e515-127">Request body</span></span>
<span data-ttu-id="1e515-128">В тексте запроса добавьте представление объекта Сиделоадингкэй в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e515-128">In the request body, supply a JSON representation for the sideLoadingKey object.</span></span>

<span data-ttu-id="1e515-129">В следующей таблице приведены свойства, необходимые при создании Сиделоадингкэй.</span><span class="sxs-lookup"><span data-stu-id="1e515-129">The following table shows the properties that are required when you create the sideLoadingKey.</span></span>

|<span data-ttu-id="1e515-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e515-130">Property</span></span>|<span data-ttu-id="1e515-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1e515-131">Type</span></span>|<span data-ttu-id="1e515-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1e515-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e515-133">id</span><span class="sxs-lookup"><span data-stu-id="1e515-133">id</span></span>|<span data-ttu-id="1e515-134">String</span><span class="sxs-lookup"><span data-stu-id="1e515-134">String</span></span>|<span data-ttu-id="1e515-135">Уникальный идентификатор ключа загрузки на стороне.</span><span class="sxs-lookup"><span data-stu-id="1e515-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="1e515-136">value</span><span class="sxs-lookup"><span data-stu-id="1e515-136">value</span></span>|<span data-ttu-id="1e515-137">String</span><span class="sxs-lookup"><span data-stu-id="1e515-137">String</span></span>|<span data-ttu-id="1e515-138">Значение ключа загрузки на стороне, это значение 5x5, разделенное хифенс.</span><span class="sxs-lookup"><span data-stu-id="1e515-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="1e515-139">displayName</span><span class="sxs-lookup"><span data-stu-id="1e515-139">displayName</span></span>|<span data-ttu-id="1e515-140">Строка</span><span class="sxs-lookup"><span data-stu-id="1e515-140">String</span></span>|<span data-ttu-id="1e515-141">Имя ключа загрузки на стороне, отображаемое для администраторов ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="1e515-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="1e515-142">description</span><span class="sxs-lookup"><span data-stu-id="1e515-142">description</span></span>|<span data-ttu-id="1e515-143">String</span><span class="sxs-lookup"><span data-stu-id="1e515-143">String</span></span>|<span data-ttu-id="1e515-144">Описание ключа загрузки на стороне, которое отображается для администраторов ИТ-специалистов..</span><span class="sxs-lookup"><span data-stu-id="1e515-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="1e515-145">тоталактиватион</span><span class="sxs-lookup"><span data-stu-id="1e515-145">totalActivation</span></span>|<span data-ttu-id="1e515-146">Int32</span><span class="sxs-lookup"><span data-stu-id="1e515-146">Int32</span></span>|<span data-ttu-id="1e515-147">Клавиша загрузки на боковой стороне общая активация отображается для администраторов ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="1e515-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="1e515-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e515-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="1e515-149">String</span><span class="sxs-lookup"><span data-stu-id="1e515-149">String</span></span>|<span data-ttu-id="1e515-150">Клавиша загрузки на боковой стороне Дата последнего обновления отображается для администраторов ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="1e515-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="1e515-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e515-151">Response</span></span>
<span data-ttu-id="1e515-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e515-152">If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e515-153">Пример</span><span class="sxs-lookup"><span data-stu-id="1e515-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e515-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e515-154">Request</span></span>
<span data-ttu-id="1e515-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e515-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1e515-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e515-156">Response</span></span>
<span data-ttu-id="1e515-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e515-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



