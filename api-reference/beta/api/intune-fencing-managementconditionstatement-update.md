---
title: Обновление Манажементкондитионстатемент
description: Обновление свойств объекта Манажементкондитионстатемент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 173a2b22320de975568a9d56ad113f5881bbef38
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054093"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="32a2e-103">Обновление Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="32a2e-103">Update managementConditionStatement</span></span>

<span data-ttu-id="32a2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32a2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32a2e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32a2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32a2e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32a2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32a2e-107">Обновление свойств объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="32a2e-107">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32a2e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="32a2e-108">Prerequisites</span></span>
<span data-ttu-id="32a2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32a2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32a2e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32a2e-111">Permission type</span></span>|<span data-ttu-id="32a2e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32a2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32a2e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32a2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32a2e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32a2e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32a2e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32a2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32a2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32a2e-116">Not supported.</span></span>|
|<span data-ttu-id="32a2e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32a2e-117">Application</span></span>|<span data-ttu-id="32a2e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32a2e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32a2e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32a2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="32a2e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="32a2e-120">Request headers</span></span>
|<span data-ttu-id="32a2e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32a2e-121">Header</span></span>|<span data-ttu-id="32a2e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="32a2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32a2e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32a2e-123">Authorization</span></span>|<span data-ttu-id="32a2e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32a2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32a2e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="32a2e-125">Accept</span></span>|<span data-ttu-id="32a2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32a2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32a2e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32a2e-127">Request body</span></span>
<span data-ttu-id="32a2e-128">В тексте запроса добавьте представление объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32a2e-128">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="32a2e-129">В следующей таблице приведены свойства, необходимые при создании [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md).</span><span class="sxs-lookup"><span data-stu-id="32a2e-129">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="32a2e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="32a2e-130">Property</span></span>|<span data-ttu-id="32a2e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="32a2e-131">Type</span></span>|<span data-ttu-id="32a2e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="32a2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32a2e-133">id</span><span class="sxs-lookup"><span data-stu-id="32a2e-133">id</span></span>|<span data-ttu-id="32a2e-134">String</span><span class="sxs-lookup"><span data-stu-id="32a2e-134">String</span></span>|<span data-ttu-id="32a2e-135">Уникальный идентификатор оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="32a2e-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="32a2e-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="32a2e-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="32a2e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="32a2e-137">displayName</span></span>|<span data-ttu-id="32a2e-138">String</span><span class="sxs-lookup"><span data-stu-id="32a2e-138">String</span></span>|<span data-ttu-id="32a2e-139">Имя, определенное администратором оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="32a2e-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="32a2e-140">description</span><span class="sxs-lookup"><span data-stu-id="32a2e-140">description</span></span>|<span data-ttu-id="32a2e-141">String</span><span class="sxs-lookup"><span data-stu-id="32a2e-141">String</span></span>|<span data-ttu-id="32a2e-142">Заданное администратором описание оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="32a2e-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="32a2e-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32a2e-143">createdDateTime</span></span>|<span data-ttu-id="32a2e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32a2e-144">DateTimeOffset</span></span>|<span data-ttu-id="32a2e-145">Время создания оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="32a2e-145">The time the management condition statement was created.</span></span> <span data-ttu-id="32a2e-146">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="32a2e-146">Generated service side.</span></span>|
|<span data-ttu-id="32a2e-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32a2e-147">modifiedDateTime</span></span>|<span data-ttu-id="32a2e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32a2e-148">DateTimeOffset</span></span>|<span data-ttu-id="32a2e-149">Время последнего изменения оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="32a2e-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="32a2e-150">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="32a2e-150">Updated service side.</span></span>|
|<span data-ttu-id="32a2e-151">выражение</span><span class="sxs-lookup"><span data-stu-id="32a2e-151">expression</span></span>|[<span data-ttu-id="32a2e-152">манажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="32a2e-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="32a2e-153">Выражение оператора условия управления, используемое для оценки активации или деактивации оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="32a2e-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="32a2e-154">eTag</span><span class="sxs-lookup"><span data-stu-id="32a2e-154">eTag</span></span>|<span data-ttu-id="32a2e-155">String</span><span class="sxs-lookup"><span data-stu-id="32a2e-155">String</span></span>|<span data-ttu-id="32a2e-156">Тег ETag оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="32a2e-156">ETag of the management condition statement.</span></span> <span data-ttu-id="32a2e-157">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="32a2e-157">Updated service side.</span></span>|
|<span data-ttu-id="32a2e-158">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="32a2e-158">applicablePlatforms</span></span>|<span data-ttu-id="32a2e-159">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="32a2e-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="32a2e-160">Соответствующие платформы для этого оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="32a2e-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="32a2e-161">Это рассчитывается на основе условий управления, связанных с оператором условия управления, и поиском пересечения соответствующих платформ.</span><span class="sxs-lookup"><span data-stu-id="32a2e-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="32a2e-162">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="32a2e-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="32a2e-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="32a2e-163">Response</span></span>
<span data-ttu-id="32a2e-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32a2e-164">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32a2e-165">Пример</span><span class="sxs-lookup"><span data-stu-id="32a2e-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="32a2e-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="32a2e-166">Request</span></span>
<span data-ttu-id="32a2e-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32a2e-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
Content-type: application/json
Content-length: 358

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "Value value"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```

### <a name="response"></a><span data-ttu-id="32a2e-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="32a2e-168">Response</span></span>
<span data-ttu-id="32a2e-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32a2e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "Value value"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```






