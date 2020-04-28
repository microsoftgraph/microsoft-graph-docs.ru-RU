---
title: Создание Секуритибаселинекатегористатесуммари
description: Создание нового объекта Секуритибаселинекатегористатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 99123c0dd864d4a876489b4da51ac3391a31af31
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381395"
---
# <a name="create-securitybaselinecategorystatesummary"></a><span data-ttu-id="04544-103">Создание Секуритибаселинекатегористатесуммари</span><span class="sxs-lookup"><span data-stu-id="04544-103">Create securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="04544-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04544-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04544-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04544-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04544-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04544-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04544-107">Создание нового объекта [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="04544-107">Create a new [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04544-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="04544-108">Prerequisites</span></span>
<span data-ttu-id="04544-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04544-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04544-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04544-111">Permission type</span></span>|<span data-ttu-id="04544-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04544-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04544-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04544-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04544-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04544-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="04544-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04544-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04544-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04544-116">Not supported.</span></span>|
|<span data-ttu-id="04544-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04544-117">Application</span></span>|<span data-ttu-id="04544-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04544-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04544-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04544-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="04544-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="04544-120">Request headers</span></span>
|<span data-ttu-id="04544-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04544-121">Header</span></span>|<span data-ttu-id="04544-122">Значение</span><span class="sxs-lookup"><span data-stu-id="04544-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04544-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04544-123">Authorization</span></span>|<span data-ttu-id="04544-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04544-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04544-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04544-125">Accept</span></span>|<span data-ttu-id="04544-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04544-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04544-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04544-127">Request body</span></span>
<span data-ttu-id="04544-128">В тексте запроса добавьте представление объекта Секуритибаселинекатегористатесуммари в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04544-128">In the request body, supply a JSON representation for the securityBaselineCategoryStateSummary object.</span></span>

<span data-ttu-id="04544-129">В следующей таблице приведены свойства, необходимые при создании Секуритибаселинекатегористатесуммари.</span><span class="sxs-lookup"><span data-stu-id="04544-129">The following table shows the properties that are required when you create the securityBaselineCategoryStateSummary.</span></span>

|<span data-ttu-id="04544-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="04544-130">Property</span></span>|<span data-ttu-id="04544-131">Тип</span><span class="sxs-lookup"><span data-stu-id="04544-131">Type</span></span>|<span data-ttu-id="04544-132">Описание</span><span class="sxs-lookup"><span data-stu-id="04544-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04544-133">id</span><span class="sxs-lookup"><span data-stu-id="04544-133">id</span></span>|<span data-ttu-id="04544-134">String</span><span class="sxs-lookup"><span data-stu-id="04544-134">String</span></span>|<span data-ttu-id="04544-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="04544-135">Unique identifier of the entity.</span></span> <span data-ttu-id="04544-136">Наследуется от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="04544-136">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="04544-137">секурекаунт</span><span class="sxs-lookup"><span data-stu-id="04544-137">secureCount</span></span>|<span data-ttu-id="04544-138">Int32</span><span class="sxs-lookup"><span data-stu-id="04544-138">Int32</span></span>|<span data-ttu-id="04544-139">Количество защищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="04544-139">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="04544-140">нотсекурекаунт</span><span class="sxs-lookup"><span data-stu-id="04544-140">notSecureCount</span></span>|<span data-ttu-id="04544-141">Int32</span><span class="sxs-lookup"><span data-stu-id="04544-141">Int32</span></span>|<span data-ttu-id="04544-142">Количество незащищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="04544-142">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="04544-143">unknownCount</span><span class="sxs-lookup"><span data-stu-id="04544-143">unknownCount</span></span>|<span data-ttu-id="04544-144">Int32</span><span class="sxs-lookup"><span data-stu-id="04544-144">Int32</span></span>|<span data-ttu-id="04544-145">Количество неизвестных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="04544-145">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="04544-146">errorCount</span><span class="sxs-lookup"><span data-stu-id="04544-146">errorCount</span></span>|<span data-ttu-id="04544-147">Int32</span><span class="sxs-lookup"><span data-stu-id="04544-147">Int32</span></span>|<span data-ttu-id="04544-148">Количество устройств с ошибками, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="04544-148">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="04544-149">conflictCount</span><span class="sxs-lookup"><span data-stu-id="04544-149">conflictCount</span></span>|<span data-ttu-id="04544-150">Int32</span><span class="sxs-lookup"><span data-stu-id="04544-150">Int32</span></span>|<span data-ttu-id="04544-151">Количество устройств с конфликтами, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="04544-151">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="04544-152">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="04544-152">notApplicableCount</span></span>|<span data-ttu-id="04544-153">Int32</span><span class="sxs-lookup"><span data-stu-id="04544-153">Int32</span></span>|<span data-ttu-id="04544-154">Количество неприменимых устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="04544-154">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="04544-155">displayName</span><span class="sxs-lookup"><span data-stu-id="04544-155">displayName</span></span>|<span data-ttu-id="04544-156">Строка</span><span class="sxs-lookup"><span data-stu-id="04544-156">String</span></span>|<span data-ttu-id="04544-157">Имя категории</span><span class="sxs-lookup"><span data-stu-id="04544-157">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="04544-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="04544-158">Response</span></span>
<span data-ttu-id="04544-159">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04544-159">If successful, this method returns a `201 Created` response code and a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04544-160">Пример</span><span class="sxs-lookup"><span data-stu-id="04544-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="04544-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="04544-161">Request</span></span>
<span data-ttu-id="04544-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04544-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="04544-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="04544-163">Response</span></span>
<span data-ttu-id="04544-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04544-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "7a650997-0997-7a65-9709-657a9709657a",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```



