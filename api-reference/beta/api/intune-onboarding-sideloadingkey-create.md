---
title: Создание Сиделоадингкэй
description: Создание нового объекта Сиделоадингкэй.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: afaae9fca5d6f459b94e5a6e7a7818d9426a0b6f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142954"
---
# <a name="create-sideloadingkey"></a><span data-ttu-id="77a98-103">Создание Сиделоадингкэй</span><span class="sxs-lookup"><span data-stu-id="77a98-103">Create sideLoadingKey</span></span>

> <span data-ttu-id="77a98-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77a98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77a98-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77a98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77a98-106">Создание нового объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="77a98-106">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77a98-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="77a98-107">Prerequisites</span></span>
<span data-ttu-id="77a98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="77a98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="77a98-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77a98-110">Permission type</span></span>|<span data-ttu-id="77a98-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77a98-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77a98-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77a98-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77a98-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77a98-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="77a98-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77a98-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77a98-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77a98-115">Not supported.</span></span>|
|<span data-ttu-id="77a98-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77a98-116">Application</span></span>|<span data-ttu-id="77a98-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77a98-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77a98-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77a98-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="77a98-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77a98-119">Request headers</span></span>
|<span data-ttu-id="77a98-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77a98-120">Header</span></span>|<span data-ttu-id="77a98-121">Значение</span><span class="sxs-lookup"><span data-stu-id="77a98-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77a98-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77a98-122">Authorization</span></span>|<span data-ttu-id="77a98-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="77a98-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77a98-124">Accept</span><span class="sxs-lookup"><span data-stu-id="77a98-124">Accept</span></span>|<span data-ttu-id="77a98-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77a98-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77a98-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77a98-126">Request body</span></span>
<span data-ttu-id="77a98-127">В тексте запроса добавьте представление объекта Сиделоадингкэй в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77a98-127">In the request body, supply a JSON representation for the sideLoadingKey object.</span></span>

<span data-ttu-id="77a98-128">В следующей таблице приведены свойства, необходимые при создании Сиделоадингкэй.</span><span class="sxs-lookup"><span data-stu-id="77a98-128">The following table shows the properties that are required when you create the sideLoadingKey.</span></span>

|<span data-ttu-id="77a98-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="77a98-129">Property</span></span>|<span data-ttu-id="77a98-130">Тип</span><span class="sxs-lookup"><span data-stu-id="77a98-130">Type</span></span>|<span data-ttu-id="77a98-131">Описание</span><span class="sxs-lookup"><span data-stu-id="77a98-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77a98-132">id</span><span class="sxs-lookup"><span data-stu-id="77a98-132">id</span></span>|<span data-ttu-id="77a98-133">String</span><span class="sxs-lookup"><span data-stu-id="77a98-133">String</span></span>|<span data-ttu-id="77a98-134">Уникальный идентификатор ключа загрузки на стороне.</span><span class="sxs-lookup"><span data-stu-id="77a98-134">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="77a98-135">value</span><span class="sxs-lookup"><span data-stu-id="77a98-135">value</span></span>|<span data-ttu-id="77a98-136">String</span><span class="sxs-lookup"><span data-stu-id="77a98-136">String</span></span>|<span data-ttu-id="77a98-137">Значение ключа загрузки на стороне, это значение 5x5, разделенное хифенс.</span><span class="sxs-lookup"><span data-stu-id="77a98-137">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="77a98-138">displayName</span><span class="sxs-lookup"><span data-stu-id="77a98-138">displayName</span></span>|<span data-ttu-id="77a98-139">String</span><span class="sxs-lookup"><span data-stu-id="77a98-139">String</span></span>|<span data-ttu-id="77a98-140">Имя ключа загрузки на стороне, отображаемое для администраторов ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="77a98-140">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="77a98-141">description</span><span class="sxs-lookup"><span data-stu-id="77a98-141">description</span></span>|<span data-ttu-id="77a98-142">String</span><span class="sxs-lookup"><span data-stu-id="77a98-142">String</span></span>|<span data-ttu-id="77a98-143">Описание ключа загрузки на стороне, которое отображается для администраторов ИТ-специалистов..</span><span class="sxs-lookup"><span data-stu-id="77a98-143">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="77a98-144">Тоталактиватион</span><span class="sxs-lookup"><span data-stu-id="77a98-144">totalActivation</span></span>|<span data-ttu-id="77a98-145">Int32</span><span class="sxs-lookup"><span data-stu-id="77a98-145">Int32</span></span>|<span data-ttu-id="77a98-146">Клавиша загрузки на боковой стороне общая активация отображается для администраторов ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="77a98-146">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="77a98-147">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="77a98-147">lastUpdatedDateTime</span></span>|<span data-ttu-id="77a98-148">String</span><span class="sxs-lookup"><span data-stu-id="77a98-148">String</span></span>|<span data-ttu-id="77a98-149">Клавиша загрузки на боковой стороне Дата последнего обновления отображается для администраторов ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="77a98-149">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="77a98-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="77a98-150">Response</span></span>
<span data-ttu-id="77a98-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77a98-151">If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77a98-152">Пример</span><span class="sxs-lookup"><span data-stu-id="77a98-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="77a98-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="77a98-153">Request</span></span>
<span data-ttu-id="77a98-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77a98-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="77a98-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="77a98-155">Response</span></span>
<span data-ttu-id="77a98-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77a98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




