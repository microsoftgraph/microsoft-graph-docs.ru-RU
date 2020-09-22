---
title: Создание Манажементкондитионстатемент
description: Создание нового объекта Манажементкондитионстатемент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4bc4d28ce345d3f82f15d4b31b6158b919246052
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072195"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="503aa-103">Создание Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="503aa-103">Create managementConditionStatement</span></span>

<span data-ttu-id="503aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="503aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="503aa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="503aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="503aa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="503aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="503aa-107">Создание нового объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="503aa-107">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="503aa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="503aa-108">Prerequisites</span></span>
<span data-ttu-id="503aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="503aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="503aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="503aa-111">Permission type</span></span>|<span data-ttu-id="503aa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="503aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="503aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="503aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="503aa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="503aa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="503aa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="503aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="503aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="503aa-116">Not supported.</span></span>|
|<span data-ttu-id="503aa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="503aa-117">Application</span></span>|<span data-ttu-id="503aa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="503aa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="503aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="503aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="503aa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="503aa-120">Request headers</span></span>
|<span data-ttu-id="503aa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="503aa-121">Header</span></span>|<span data-ttu-id="503aa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="503aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="503aa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="503aa-123">Authorization</span></span>|<span data-ttu-id="503aa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="503aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="503aa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="503aa-125">Accept</span></span>|<span data-ttu-id="503aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="503aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="503aa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="503aa-127">Request body</span></span>
<span data-ttu-id="503aa-128">В тексте запроса добавьте представление объекта Манажементкондитионстатемент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="503aa-128">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="503aa-129">В следующей таблице приведены свойства, необходимые при создании Манажементкондитионстатемент.</span><span class="sxs-lookup"><span data-stu-id="503aa-129">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="503aa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="503aa-130">Property</span></span>|<span data-ttu-id="503aa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="503aa-131">Type</span></span>|<span data-ttu-id="503aa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="503aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="503aa-133">id</span><span class="sxs-lookup"><span data-stu-id="503aa-133">id</span></span>|<span data-ttu-id="503aa-134">String</span><span class="sxs-lookup"><span data-stu-id="503aa-134">String</span></span>|<span data-ttu-id="503aa-135">Уникальный идентификатор оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="503aa-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="503aa-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="503aa-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="503aa-137">displayName</span><span class="sxs-lookup"><span data-stu-id="503aa-137">displayName</span></span>|<span data-ttu-id="503aa-138">String</span><span class="sxs-lookup"><span data-stu-id="503aa-138">String</span></span>|<span data-ttu-id="503aa-139">Имя, определенное администратором оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="503aa-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="503aa-140">description</span><span class="sxs-lookup"><span data-stu-id="503aa-140">description</span></span>|<span data-ttu-id="503aa-141">String</span><span class="sxs-lookup"><span data-stu-id="503aa-141">String</span></span>|<span data-ttu-id="503aa-142">Заданное администратором описание оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="503aa-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="503aa-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="503aa-143">createdDateTime</span></span>|<span data-ttu-id="503aa-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="503aa-144">DateTimeOffset</span></span>|<span data-ttu-id="503aa-145">Время создания оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="503aa-145">The time the management condition statement was created.</span></span> <span data-ttu-id="503aa-146">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="503aa-146">Generated service side.</span></span>|
|<span data-ttu-id="503aa-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="503aa-147">modifiedDateTime</span></span>|<span data-ttu-id="503aa-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="503aa-148">DateTimeOffset</span></span>|<span data-ttu-id="503aa-149">Время последнего изменения оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="503aa-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="503aa-150">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="503aa-150">Updated service side.</span></span>|
|<span data-ttu-id="503aa-151">выражение</span><span class="sxs-lookup"><span data-stu-id="503aa-151">expression</span></span>|[<span data-ttu-id="503aa-152">манажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="503aa-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="503aa-153">Выражение оператора условия управления, используемое для оценки активации или деактивации оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="503aa-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="503aa-154">eTag</span><span class="sxs-lookup"><span data-stu-id="503aa-154">eTag</span></span>|<span data-ttu-id="503aa-155">String</span><span class="sxs-lookup"><span data-stu-id="503aa-155">String</span></span>|<span data-ttu-id="503aa-156">Тег ETag оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="503aa-156">ETag of the management condition statement.</span></span> <span data-ttu-id="503aa-157">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="503aa-157">Updated service side.</span></span>|
|<span data-ttu-id="503aa-158">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="503aa-158">applicablePlatforms</span></span>|<span data-ttu-id="503aa-159">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="503aa-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="503aa-160">Соответствующие платформы для этого оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="503aa-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="503aa-161">Это рассчитывается на основе условий управления, связанных с оператором условия управления, и поиском пересечения соответствующих платформ.</span><span class="sxs-lookup"><span data-stu-id="503aa-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="503aa-162">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="503aa-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="503aa-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="503aa-163">Response</span></span>
<span data-ttu-id="503aa-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="503aa-164">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="503aa-165">Пример</span><span class="sxs-lookup"><span data-stu-id="503aa-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="503aa-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="503aa-166">Request</span></span>
<span data-ttu-id="503aa-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="503aa-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
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

### <a name="response"></a><span data-ttu-id="503aa-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="503aa-168">Response</span></span>
<span data-ttu-id="503aa-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="503aa-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






