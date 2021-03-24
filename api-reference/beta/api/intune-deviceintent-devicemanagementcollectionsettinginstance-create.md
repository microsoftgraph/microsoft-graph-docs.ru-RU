---
title: Создание deviceManagementCollectionSettingInstance
description: Создание нового объекта deviceManagementCollectionSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cdf43022cb12c212daf408911479d6cdb8bd55a3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129029"
---
# <a name="create-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="0bf87-103">Создание deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="0bf87-103">Create deviceManagementCollectionSettingInstance</span></span>

<span data-ttu-id="0bf87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bf87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bf87-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bf87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bf87-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bf87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bf87-107">Создание нового [объекта deviceManagementCollectionSettingInstance.](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0bf87-107">Create a new [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bf87-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0bf87-108">Prerequisites</span></span>
<span data-ttu-id="0bf87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bf87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bf87-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bf87-111">Permission type</span></span>|<span data-ttu-id="0bf87-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bf87-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bf87-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bf87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bf87-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bf87-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0bf87-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bf87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bf87-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bf87-116">Not supported.</span></span>|
|<span data-ttu-id="0bf87-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0bf87-117">Application</span></span>|<span data-ttu-id="0bf87-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bf87-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bf87-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bf87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/settings
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="0bf87-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0bf87-120">Request headers</span></span>
|<span data-ttu-id="0bf87-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0bf87-121">Header</span></span>|<span data-ttu-id="0bf87-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0bf87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bf87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bf87-123">Authorization</span></span>|<span data-ttu-id="0bf87-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bf87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bf87-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0bf87-125">Accept</span></span>|<span data-ttu-id="0bf87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bf87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bf87-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0bf87-127">Request body</span></span>
<span data-ttu-id="0bf87-128">В теле запроса поставляем представление JSON для объекта deviceManagementCollectionSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="0bf87-128">In the request body, supply a JSON representation for the deviceManagementCollectionSettingInstance object.</span></span>

<span data-ttu-id="0bf87-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementCollectionSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="0bf87-129">The following table shows the properties that are required when you create the deviceManagementCollectionSettingInstance.</span></span>

|<span data-ttu-id="0bf87-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bf87-130">Property</span></span>|<span data-ttu-id="0bf87-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0bf87-131">Type</span></span>|<span data-ttu-id="0bf87-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0bf87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bf87-133">id</span><span class="sxs-lookup"><span data-stu-id="0bf87-133">id</span></span>|<span data-ttu-id="0bf87-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0bf87-134">String</span></span>|<span data-ttu-id="0bf87-135">ID экземпляра параметра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0bf87-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="0bf87-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="0bf87-136">definitionId</span></span>|<span data-ttu-id="0bf87-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0bf87-137">String</span></span>|<span data-ttu-id="0bf87-138">ID определения параметра для этого экземпляра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0bf87-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="0bf87-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="0bf87-139">valueJson</span></span>|<span data-ttu-id="0bf87-140">Строка</span><span class="sxs-lookup"><span data-stu-id="0bf87-140">String</span></span>|<span data-ttu-id="0bf87-141">Представление JSON значения, унаследованной от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0bf87-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0bf87-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bf87-142">Response</span></span>
<span data-ttu-id="0bf87-143">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0bf87-143">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bf87-144">Пример</span><span class="sxs-lookup"><span data-stu-id="0bf87-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bf87-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bf87-145">Request</span></span>
<span data-ttu-id="0bf87-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0bf87-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="0bf87-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bf87-147">Response</span></span>
<span data-ttu-id="0bf87-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0bf87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```




