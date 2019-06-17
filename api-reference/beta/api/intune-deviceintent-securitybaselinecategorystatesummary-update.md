---
title: Обновление Секуритибаселинекатегористатесуммари
description: Обновление свойств объекта Секуритибаселинекатегористатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 559a4befe8c5a11f7683be35f5ade8a39a323e03
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959595"
---
# <a name="update-securitybaselinecategorystatesummary"></a><span data-ttu-id="e8e05-103">Обновление Секуритибаселинекатегористатесуммари</span><span class="sxs-lookup"><span data-stu-id="e8e05-103">Update securityBaselineCategoryStateSummary</span></span>

> <span data-ttu-id="e8e05-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8e05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8e05-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8e05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8e05-106">Обновление свойств объекта [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e8e05-106">Update the properties of a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8e05-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e8e05-107">Prerequisites</span></span>
<span data-ttu-id="e8e05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8e05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8e05-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8e05-110">Permission type</span></span>|<span data-ttu-id="e8e05-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8e05-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8e05-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8e05-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8e05-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8e05-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8e05-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8e05-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8e05-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8e05-115">Not supported.</span></span>|
|<span data-ttu-id="e8e05-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8e05-116">Application</span></span>|<span data-ttu-id="e8e05-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8e05-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8e05-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8e05-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="e8e05-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8e05-119">Request headers</span></span>
|<span data-ttu-id="e8e05-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8e05-120">Header</span></span>|<span data-ttu-id="e8e05-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e8e05-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8e05-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8e05-122">Authorization</span></span>|<span data-ttu-id="e8e05-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8e05-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8e05-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e8e05-124">Accept</span></span>|<span data-ttu-id="e8e05-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8e05-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8e05-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e8e05-126">Request body</span></span>
<span data-ttu-id="e8e05-127">В тексте запроса добавьте представление объекта [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8e05-127">In the request body, supply a JSON representation for the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

<span data-ttu-id="e8e05-128">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e8e05-128">The following table shows the properties that are required when you create the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span></span>

|<span data-ttu-id="e8e05-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8e05-129">Property</span></span>|<span data-ttu-id="e8e05-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e8e05-130">Type</span></span>|<span data-ttu-id="e8e05-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e8e05-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8e05-132">id</span><span class="sxs-lookup"><span data-stu-id="e8e05-132">id</span></span>|<span data-ttu-id="e8e05-133">String</span><span class="sxs-lookup"><span data-stu-id="e8e05-133">String</span></span>|<span data-ttu-id="e8e05-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="e8e05-134">Unique identifier of the entity.</span></span> <span data-ttu-id="e8e05-135">Наследуется от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e8e05-135">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="e8e05-136">Секурекаунт</span><span class="sxs-lookup"><span data-stu-id="e8e05-136">secureCount</span></span>|<span data-ttu-id="e8e05-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e8e05-137">Int32</span></span>|<span data-ttu-id="e8e05-138">Количество защищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e8e05-138">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="e8e05-139">Нотсекурекаунт</span><span class="sxs-lookup"><span data-stu-id="e8e05-139">notSecureCount</span></span>|<span data-ttu-id="e8e05-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e8e05-140">Int32</span></span>|<span data-ttu-id="e8e05-141">Количество незащищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e8e05-141">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="e8e05-142">unknownCount</span><span class="sxs-lookup"><span data-stu-id="e8e05-142">unknownCount</span></span>|<span data-ttu-id="e8e05-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e8e05-143">Int32</span></span>|<span data-ttu-id="e8e05-144">Количество неизвестных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e8e05-144">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="e8e05-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="e8e05-145">errorCount</span></span>|<span data-ttu-id="e8e05-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e8e05-146">Int32</span></span>|<span data-ttu-id="e8e05-147">Количество устройств с ошибками, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e8e05-147">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="e8e05-148">conflictCount</span><span class="sxs-lookup"><span data-stu-id="e8e05-148">conflictCount</span></span>|<span data-ttu-id="e8e05-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e8e05-149">Int32</span></span>|<span data-ttu-id="e8e05-150">Количество устройств с конфликтами, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e8e05-150">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="e8e05-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e8e05-151">notApplicableCount</span></span>|<span data-ttu-id="e8e05-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e8e05-152">Int32</span></span>|<span data-ttu-id="e8e05-153">Количество неприменимых устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e8e05-153">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="e8e05-154">displayName</span><span class="sxs-lookup"><span data-stu-id="e8e05-154">displayName</span></span>|<span data-ttu-id="e8e05-155">Строка</span><span class="sxs-lookup"><span data-stu-id="e8e05-155">String</span></span>|<span data-ttu-id="e8e05-156">Имя категории</span><span class="sxs-lookup"><span data-stu-id="e8e05-156">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="e8e05-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8e05-157">Response</span></span>
<span data-ttu-id="e8e05-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8e05-158">If successful, this method returns a `200 OK` response code and an updated [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8e05-159">Пример</span><span class="sxs-lookup"><span data-stu-id="e8e05-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8e05-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8e05-160">Request</span></span>
<span data-ttu-id="e8e05-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8e05-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="e8e05-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8e05-162">Response</span></span>
<span data-ttu-id="e8e05-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8e05-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





