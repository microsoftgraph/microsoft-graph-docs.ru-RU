---
title: Создание Секуритибаселинекатегористатесуммари
description: Создание нового объекта Секуритибаселинекатегористатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7612952f7e91d9dc0eec10893440ecf47dcc1fe7
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188915"
---
# <a name="create-securitybaselinecategorystatesummary"></a><span data-ttu-id="d93e0-103">Создание Секуритибаселинекатегористатесуммари</span><span class="sxs-lookup"><span data-stu-id="d93e0-103">Create securityBaselineCategoryStateSummary</span></span>

> <span data-ttu-id="d93e0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d93e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d93e0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d93e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d93e0-106">Создание нового объекта [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d93e0-106">Create a new [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d93e0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d93e0-107">Prerequisites</span></span>
<span data-ttu-id="d93e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d93e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d93e0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d93e0-110">Permission type</span></span>|<span data-ttu-id="d93e0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d93e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d93e0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d93e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d93e0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d93e0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d93e0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d93e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d93e0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d93e0-115">Not supported.</span></span>|
|<span data-ttu-id="d93e0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d93e0-116">Application</span></span>|<span data-ttu-id="d93e0-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d93e0-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d93e0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d93e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d93e0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d93e0-119">Request headers</span></span>
|<span data-ttu-id="d93e0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d93e0-120">Header</span></span>|<span data-ttu-id="d93e0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d93e0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d93e0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d93e0-122">Authorization</span></span>|<span data-ttu-id="d93e0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d93e0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d93e0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d93e0-124">Accept</span></span>|<span data-ttu-id="d93e0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d93e0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d93e0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d93e0-126">Request body</span></span>
<span data-ttu-id="d93e0-127">В тексте запроса добавьте представление объекта Секуритибаселинекатегористатесуммари в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d93e0-127">In the request body, supply a JSON representation for the securityBaselineCategoryStateSummary object.</span></span>

<span data-ttu-id="d93e0-128">В следующей таблице приведены свойства, необходимые при создании Секуритибаселинекатегористатесуммари.</span><span class="sxs-lookup"><span data-stu-id="d93e0-128">The following table shows the properties that are required when you create the securityBaselineCategoryStateSummary.</span></span>

|<span data-ttu-id="d93e0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d93e0-129">Property</span></span>|<span data-ttu-id="d93e0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d93e0-130">Type</span></span>|<span data-ttu-id="d93e0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d93e0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d93e0-132">id</span><span class="sxs-lookup"><span data-stu-id="d93e0-132">id</span></span>|<span data-ttu-id="d93e0-133">String</span><span class="sxs-lookup"><span data-stu-id="d93e0-133">String</span></span>|<span data-ttu-id="d93e0-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="d93e0-134">Unique identifier of the entity.</span></span> <span data-ttu-id="d93e0-135">Наследуется от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="d93e0-135">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d93e0-136">секурекаунт</span><span class="sxs-lookup"><span data-stu-id="d93e0-136">secureCount</span></span>|<span data-ttu-id="d93e0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d93e0-137">Int32</span></span>|<span data-ttu-id="d93e0-138">Количество защищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="d93e0-138">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d93e0-139">нотсекурекаунт</span><span class="sxs-lookup"><span data-stu-id="d93e0-139">notSecureCount</span></span>|<span data-ttu-id="d93e0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d93e0-140">Int32</span></span>|<span data-ttu-id="d93e0-141">Количество незащищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="d93e0-141">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d93e0-142">unknownCount</span><span class="sxs-lookup"><span data-stu-id="d93e0-142">unknownCount</span></span>|<span data-ttu-id="d93e0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d93e0-143">Int32</span></span>|<span data-ttu-id="d93e0-144">Количество неизвестных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="d93e0-144">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d93e0-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="d93e0-145">errorCount</span></span>|<span data-ttu-id="d93e0-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d93e0-146">Int32</span></span>|<span data-ttu-id="d93e0-147">Количество устройств с ошибками, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="d93e0-147">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d93e0-148">conflictCount</span><span class="sxs-lookup"><span data-stu-id="d93e0-148">conflictCount</span></span>|<span data-ttu-id="d93e0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d93e0-149">Int32</span></span>|<span data-ttu-id="d93e0-150">Количество устройств с конфликтами, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="d93e0-150">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d93e0-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d93e0-151">notApplicableCount</span></span>|<span data-ttu-id="d93e0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d93e0-152">Int32</span></span>|<span data-ttu-id="d93e0-153">Количество неприменимых устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="d93e0-153">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d93e0-154">displayName</span><span class="sxs-lookup"><span data-stu-id="d93e0-154">displayName</span></span>|<span data-ttu-id="d93e0-155">Строка</span><span class="sxs-lookup"><span data-stu-id="d93e0-155">String</span></span>|<span data-ttu-id="d93e0-156">Имя категории</span><span class="sxs-lookup"><span data-stu-id="d93e0-156">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="d93e0-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="d93e0-157">Response</span></span>
<span data-ttu-id="d93e0-158">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d93e0-158">If successful, this method returns a `201 Created` response code and a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d93e0-159">Пример</span><span class="sxs-lookup"><span data-stu-id="d93e0-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="d93e0-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="d93e0-160">Request</span></span>
<span data-ttu-id="d93e0-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d93e0-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d93e0-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="d93e0-162">Response</span></span>
<span data-ttu-id="d93e0-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d93e0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




