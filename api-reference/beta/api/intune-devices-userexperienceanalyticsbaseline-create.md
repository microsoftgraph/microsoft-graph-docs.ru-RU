---
title: Создание Усерекспериенцеаналитиксбаселине
description: Создание нового объекта Усерекспериенцеаналитиксбаселине.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f78a3f9684068d9859c91ed75c91507a50f01bc9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202537"
---
# <a name="create-userexperienceanalyticsbaseline"></a><span data-ttu-id="e45bb-103">Создание Усерекспериенцеаналитиксбаселине</span><span class="sxs-lookup"><span data-stu-id="e45bb-103">Create userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="e45bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e45bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e45bb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e45bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e45bb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e45bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e45bb-107">Создание нового объекта [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="e45bb-107">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e45bb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e45bb-108">Prerequisites</span></span>
<span data-ttu-id="e45bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e45bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e45bb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e45bb-111">Permission type</span></span>|<span data-ttu-id="e45bb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e45bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e45bb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e45bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e45bb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45bb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e45bb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e45bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e45bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e45bb-116">Not supported.</span></span>|
|<span data-ttu-id="e45bb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e45bb-117">Application</span></span>|<span data-ttu-id="e45bb-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45bb-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e45bb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e45bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="e45bb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e45bb-120">Request headers</span></span>
|<span data-ttu-id="e45bb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e45bb-121">Header</span></span>|<span data-ttu-id="e45bb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e45bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e45bb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e45bb-123">Authorization</span></span>|<span data-ttu-id="e45bb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e45bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e45bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e45bb-125">Accept</span></span>|<span data-ttu-id="e45bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e45bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e45bb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e45bb-127">Request body</span></span>
<span data-ttu-id="e45bb-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксбаселине в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e45bb-128">In the request body, supply a JSON representation for the userExperienceAnalyticsBaseline object.</span></span>

<span data-ttu-id="e45bb-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксбаселине.</span><span class="sxs-lookup"><span data-stu-id="e45bb-129">The following table shows the properties that are required when you create the userExperienceAnalyticsBaseline.</span></span>

|<span data-ttu-id="e45bb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e45bb-130">Property</span></span>|<span data-ttu-id="e45bb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e45bb-131">Type</span></span>|<span data-ttu-id="e45bb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e45bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e45bb-133">id</span><span class="sxs-lookup"><span data-stu-id="e45bb-133">id</span></span>|<span data-ttu-id="e45bb-134">String</span><span class="sxs-lookup"><span data-stu-id="e45bb-134">String</span></span>|<span data-ttu-id="e45bb-135">Уникальный идентификатор базового идентификатора аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="e45bb-135">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="e45bb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e45bb-136">displayName</span></span>|<span data-ttu-id="e45bb-137">String</span><span class="sxs-lookup"><span data-stu-id="e45bb-137">String</span></span>|<span data-ttu-id="e45bb-138">Имя базового объекта аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="e45bb-138">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="e45bb-139">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="e45bb-139">overallScore</span></span>|<span data-ttu-id="e45bb-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e45bb-140">Int32</span></span>|<span data-ttu-id="e45bb-141">Общий показатель базового уровня для аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="e45bb-141">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="e45bb-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="e45bb-142">isBuiltIn</span></span>|<span data-ttu-id="e45bb-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="e45bb-143">Boolean</span></span>|<span data-ttu-id="e45bb-144">Указывает, является ли текущий базовый планом коммерческого медианы или настраиваемым базовым планом.</span><span class="sxs-lookup"><span data-stu-id="e45bb-144">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="e45bb-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e45bb-145">createdDateTime</span></span>|<span data-ttu-id="e45bb-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e45bb-146">DateTimeOffset</span></span>|<span data-ttu-id="e45bb-147">Дата создания настраиваемого базового плана.</span><span class="sxs-lookup"><span data-stu-id="e45bb-147">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="e45bb-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="e45bb-148">Response</span></span>
<span data-ttu-id="e45bb-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e45bb-149">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e45bb-150">Пример</span><span class="sxs-lookup"><span data-stu-id="e45bb-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="e45bb-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="e45bb-151">Request</span></span>
<span data-ttu-id="e45bb-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e45bb-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "displayName": "Display Name value",
  "overallScore": 12,
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="e45bb-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e45bb-153">Response</span></span>
<span data-ttu-id="e45bb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e45bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 266

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "1cce2cab-2cab-1cce-ab2c-ce1cab2cce1c",
  "displayName": "Display Name value",
  "overallScore": 12,
  "isBuiltIn": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00"
}
```




