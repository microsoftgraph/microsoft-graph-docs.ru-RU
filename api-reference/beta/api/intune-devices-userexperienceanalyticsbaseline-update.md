---
title: Обновление userExperienceAnalyticsBaseline
description: Обновление свойств объекта userExperienceAnalyticsBaseline.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4594b56e33ff8cf7d8583c1233d5e0083bf6bcd1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154289"
---
# <a name="update-userexperienceanalyticsbaseline"></a><span data-ttu-id="8ad79-103">Обновление userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="8ad79-103">Update userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="8ad79-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ad79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ad79-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ad79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ad79-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ad79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ad79-107">Обновление свойств объекта [userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)</span><span class="sxs-lookup"><span data-stu-id="8ad79-107">Update the properties of a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ad79-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8ad79-108">Prerequisites</span></span>
<span data-ttu-id="8ad79-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ad79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ad79-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ad79-111">Permission type</span></span>|<span data-ttu-id="8ad79-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ad79-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ad79-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ad79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ad79-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ad79-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8ad79-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ad79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ad79-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ad79-116">Not supported.</span></span>|
|<span data-ttu-id="8ad79-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8ad79-117">Application</span></span>|<span data-ttu-id="8ad79-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ad79-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ad79-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ad79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

## <a name="request-headers"></a><span data-ttu-id="8ad79-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8ad79-120">Request headers</span></span>
|<span data-ttu-id="8ad79-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ad79-121">Header</span></span>|<span data-ttu-id="8ad79-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8ad79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ad79-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ad79-123">Authorization</span></span>|<span data-ttu-id="8ad79-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ad79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ad79-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ad79-125">Accept</span></span>|<span data-ttu-id="8ad79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ad79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ad79-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ad79-127">Request body</span></span>
<span data-ttu-id="8ad79-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)</span><span class="sxs-lookup"><span data-stu-id="8ad79-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

<span data-ttu-id="8ad79-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)</span><span class="sxs-lookup"><span data-stu-id="8ad79-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span></span>

|<span data-ttu-id="8ad79-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ad79-130">Property</span></span>|<span data-ttu-id="8ad79-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8ad79-131">Type</span></span>|<span data-ttu-id="8ad79-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8ad79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ad79-133">id</span><span class="sxs-lookup"><span data-stu-id="8ad79-133">id</span></span>|<span data-ttu-id="8ad79-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8ad79-134">String</span></span>|<span data-ttu-id="8ad79-135">Уникальный идентификатор базовой базы аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="8ad79-135">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="8ad79-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8ad79-136">displayName</span></span>|<span data-ttu-id="8ad79-137">Строка</span><span class="sxs-lookup"><span data-stu-id="8ad79-137">String</span></span>|<span data-ttu-id="8ad79-138">Имя базовой базы аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="8ad79-138">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="8ad79-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="8ad79-139">overallScore</span></span>|<span data-ttu-id="8ad79-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8ad79-140">Int32</span></span>|<span data-ttu-id="8ad79-141">Общая оценка базовой базы аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="8ad79-141">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="8ad79-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="8ad79-142">isBuiltIn</span></span>|<span data-ttu-id="8ad79-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ad79-143">Boolean</span></span>|<span data-ttu-id="8ad79-144">Означает, является ли текущий базовый уровень коммерческим медианым или настраиваемой базовой базой.</span><span class="sxs-lookup"><span data-stu-id="8ad79-144">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="8ad79-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ad79-145">createdDateTime</span></span>|<span data-ttu-id="8ad79-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ad79-146">DateTimeOffset</span></span>|<span data-ttu-id="8ad79-147">Дата создания настраиваемой базовой линии.</span><span class="sxs-lookup"><span data-stu-id="8ad79-147">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="8ad79-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ad79-148">Response</span></span>
<span data-ttu-id="8ad79-149">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8ad79-149">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ad79-150">Пример</span><span class="sxs-lookup"><span data-stu-id="8ad79-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ad79-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ad79-151">Request</span></span>
<span data-ttu-id="8ad79-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ad79-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "displayName": "Display Name value",
  "overallScore": 12,
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="8ad79-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ad79-153">Response</span></span>
<span data-ttu-id="8ad79-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ad79-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




