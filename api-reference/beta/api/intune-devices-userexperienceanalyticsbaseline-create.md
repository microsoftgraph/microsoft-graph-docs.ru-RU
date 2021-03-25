---
title: Создание userExperienceAnalyticsBaseline
description: Создание нового объекта userExperienceAnalyticsBaseline.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4887e2d15e1a8d1b89dab3b72aa53344f499d523
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157963"
---
# <a name="create-userexperienceanalyticsbaseline"></a><span data-ttu-id="4e53a-103">Создание userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="4e53a-103">Create userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="4e53a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e53a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e53a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e53a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e53a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e53a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e53a-107">Создание нового [объекта userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)</span><span class="sxs-lookup"><span data-stu-id="4e53a-107">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e53a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4e53a-108">Prerequisites</span></span>
<span data-ttu-id="4e53a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e53a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e53a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e53a-111">Permission type</span></span>|<span data-ttu-id="4e53a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e53a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e53a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e53a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e53a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e53a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4e53a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e53a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e53a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e53a-116">Not supported.</span></span>|
|<span data-ttu-id="4e53a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4e53a-117">Application</span></span>|<span data-ttu-id="4e53a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e53a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e53a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e53a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="4e53a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4e53a-120">Request headers</span></span>
|<span data-ttu-id="4e53a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e53a-121">Header</span></span>|<span data-ttu-id="4e53a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e53a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e53a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e53a-123">Authorization</span></span>|<span data-ttu-id="4e53a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e53a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e53a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e53a-125">Accept</span></span>|<span data-ttu-id="4e53a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e53a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e53a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e53a-127">Request body</span></span>
<span data-ttu-id="4e53a-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="4e53a-128">In the request body, supply a JSON representation for the userExperienceAnalyticsBaseline object.</span></span>

<span data-ttu-id="4e53a-129">В следующей таблице показаны свойства, необходимые при создании пользовательского интерфейсаExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="4e53a-129">The following table shows the properties that are required when you create the userExperienceAnalyticsBaseline.</span></span>

|<span data-ttu-id="4e53a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e53a-130">Property</span></span>|<span data-ttu-id="4e53a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e53a-131">Type</span></span>|<span data-ttu-id="4e53a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e53a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e53a-133">id</span><span class="sxs-lookup"><span data-stu-id="4e53a-133">id</span></span>|<span data-ttu-id="4e53a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4e53a-134">String</span></span>|<span data-ttu-id="4e53a-135">Уникальный идентификатор базовой базы аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="4e53a-135">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="4e53a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4e53a-136">displayName</span></span>|<span data-ttu-id="4e53a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4e53a-137">String</span></span>|<span data-ttu-id="4e53a-138">Имя базовой базы аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="4e53a-138">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="4e53a-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="4e53a-139">overallScore</span></span>|<span data-ttu-id="4e53a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4e53a-140">Int32</span></span>|<span data-ttu-id="4e53a-141">Общая оценка базовой базы аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="4e53a-141">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="4e53a-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="4e53a-142">isBuiltIn</span></span>|<span data-ttu-id="4e53a-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e53a-143">Boolean</span></span>|<span data-ttu-id="4e53a-144">Означает, является ли текущий базовый уровень коммерческим медианым или настраиваемой базовой базой.</span><span class="sxs-lookup"><span data-stu-id="4e53a-144">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="4e53a-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e53a-145">createdDateTime</span></span>|<span data-ttu-id="4e53a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e53a-146">DateTimeOffset</span></span>|<span data-ttu-id="4e53a-147">Дата создания настраиваемой базовой линии.</span><span class="sxs-lookup"><span data-stu-id="4e53a-147">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="4e53a-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e53a-148">Response</span></span>
<span data-ttu-id="4e53a-149">В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4e53a-149">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e53a-150">Пример</span><span class="sxs-lookup"><span data-stu-id="4e53a-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e53a-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e53a-151">Request</span></span>
<span data-ttu-id="4e53a-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e53a-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4e53a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e53a-153">Response</span></span>
<span data-ttu-id="4e53a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e53a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




