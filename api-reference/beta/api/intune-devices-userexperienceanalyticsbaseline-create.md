---
title: Создание Усерекспериенцеаналитиксбаселине
description: Создание нового объекта Усерекспериенцеаналитиксбаселине.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f69341f0e38335c6c9372fcc6a235644e5c5f3a8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944563"
---
# <a name="create-userexperienceanalyticsbaseline"></a><span data-ttu-id="2822f-103">Создание Усерекспериенцеаналитиксбаселине</span><span class="sxs-lookup"><span data-stu-id="2822f-103">Create userExperienceAnalyticsBaseline</span></span>

> <span data-ttu-id="2822f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2822f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2822f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2822f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2822f-106">Создание нового объекта [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="2822f-106">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2822f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2822f-107">Prerequisites</span></span>
<span data-ttu-id="2822f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2822f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2822f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2822f-110">Permission type</span></span>|<span data-ttu-id="2822f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2822f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2822f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2822f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2822f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2822f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2822f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2822f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2822f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2822f-115">Not supported.</span></span>|
|<span data-ttu-id="2822f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2822f-116">Application</span></span>|<span data-ttu-id="2822f-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2822f-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2822f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2822f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="2822f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2822f-119">Request headers</span></span>
|<span data-ttu-id="2822f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2822f-120">Header</span></span>|<span data-ttu-id="2822f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2822f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2822f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2822f-122">Authorization</span></span>|<span data-ttu-id="2822f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2822f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2822f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2822f-124">Accept</span></span>|<span data-ttu-id="2822f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2822f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2822f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2822f-126">Request body</span></span>
<span data-ttu-id="2822f-127">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксбаселине в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2822f-127">In the request body, supply a JSON representation for the userExperienceAnalyticsBaseline object.</span></span>

<span data-ttu-id="2822f-128">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксбаселине.</span><span class="sxs-lookup"><span data-stu-id="2822f-128">The following table shows the properties that are required when you create the userExperienceAnalyticsBaseline.</span></span>

|<span data-ttu-id="2822f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2822f-129">Property</span></span>|<span data-ttu-id="2822f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2822f-130">Type</span></span>|<span data-ttu-id="2822f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2822f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2822f-132">id</span><span class="sxs-lookup"><span data-stu-id="2822f-132">id</span></span>|<span data-ttu-id="2822f-133">String</span><span class="sxs-lookup"><span data-stu-id="2822f-133">String</span></span>|<span data-ttu-id="2822f-134">Уникальный идентификатор базового идентификатора аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="2822f-134">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="2822f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2822f-135">displayName</span></span>|<span data-ttu-id="2822f-136">Строка</span><span class="sxs-lookup"><span data-stu-id="2822f-136">String</span></span>|<span data-ttu-id="2822f-137">Имя базового объекта аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="2822f-137">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="2822f-138">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="2822f-138">overallScore</span></span>|<span data-ttu-id="2822f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2822f-139">Int32</span></span>|<span data-ttu-id="2822f-140">Общий показатель базового уровня для аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="2822f-140">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="2822f-141">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="2822f-141">isBuiltIn</span></span>|<span data-ttu-id="2822f-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="2822f-142">Boolean</span></span>|<span data-ttu-id="2822f-143">Указывает, является ли текущий базовый планом коммерческого медианы или настраиваемым базовым планом.</span><span class="sxs-lookup"><span data-stu-id="2822f-143">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="2822f-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2822f-144">createdDateTime</span></span>|<span data-ttu-id="2822f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2822f-145">DateTimeOffset</span></span>|<span data-ttu-id="2822f-146">Дата создания настраиваемого базового плана.</span><span class="sxs-lookup"><span data-stu-id="2822f-146">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="2822f-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="2822f-147">Response</span></span>
<span data-ttu-id="2822f-148">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2822f-148">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2822f-149">Пример</span><span class="sxs-lookup"><span data-stu-id="2822f-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="2822f-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="2822f-150">Request</span></span>
<span data-ttu-id="2822f-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2822f-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2822f-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="2822f-152">Response</span></span>
<span data-ttu-id="2822f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2822f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





