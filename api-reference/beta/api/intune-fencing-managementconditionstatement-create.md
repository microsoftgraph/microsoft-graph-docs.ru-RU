---
title: Создание Манажементкондитионстатемент
description: Создание нового объекта Манажементкондитионстатемент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c73bd08d3736b90803dd80c56f370e08f2fb5c3e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804774"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="c325d-103">Создание Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="c325d-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="c325d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c325d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c325d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c325d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c325d-106">Создание нового объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="c325d-106">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c325d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c325d-107">Prerequisites</span></span>
<span data-ttu-id="c325d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c325d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c325d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c325d-110">Permission type</span></span>|<span data-ttu-id="c325d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c325d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c325d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c325d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c325d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c325d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c325d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c325d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c325d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c325d-115">Not supported.</span></span>|
|<span data-ttu-id="c325d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c325d-116">Application</span></span>|<span data-ttu-id="c325d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c325d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c325d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c325d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="c325d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c325d-119">Request headers</span></span>
|<span data-ttu-id="c325d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c325d-120">Header</span></span>|<span data-ttu-id="c325d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c325d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c325d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c325d-122">Authorization</span></span>|<span data-ttu-id="c325d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c325d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c325d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c325d-124">Accept</span></span>|<span data-ttu-id="c325d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c325d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c325d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c325d-126">Request body</span></span>
<span data-ttu-id="c325d-127">В тексте запроса добавьте представление объекта Манажементкондитионстатемент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c325d-127">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="c325d-128">В следующей таблице приведены свойства, необходимые при создании Манажементкондитионстатемент.</span><span class="sxs-lookup"><span data-stu-id="c325d-128">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="c325d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c325d-129">Property</span></span>|<span data-ttu-id="c325d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c325d-130">Type</span></span>|<span data-ttu-id="c325d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c325d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c325d-132">id</span><span class="sxs-lookup"><span data-stu-id="c325d-132">id</span></span>|<span data-ttu-id="c325d-133">String</span><span class="sxs-lookup"><span data-stu-id="c325d-133">String</span></span>|<span data-ttu-id="c325d-134">Уникальный идентификатор оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c325d-134">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="c325d-135">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="c325d-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="c325d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c325d-136">displayName</span></span>|<span data-ttu-id="c325d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c325d-137">String</span></span>|<span data-ttu-id="c325d-138">Имя, определенное администратором оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c325d-138">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="c325d-139">description</span><span class="sxs-lookup"><span data-stu-id="c325d-139">description</span></span>|<span data-ttu-id="c325d-140">String</span><span class="sxs-lookup"><span data-stu-id="c325d-140">String</span></span>|<span data-ttu-id="c325d-141">Заданное администратором описание оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c325d-141">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="c325d-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c325d-142">createdDateTime</span></span>|<span data-ttu-id="c325d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c325d-143">DateTimeOffset</span></span>|<span data-ttu-id="c325d-144">Время создания оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c325d-144">The time the management condition statement was created.</span></span> <span data-ttu-id="c325d-145">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="c325d-145">Generated service side.</span></span>|
|<span data-ttu-id="c325d-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c325d-146">modifiedDateTime</span></span>|<span data-ttu-id="c325d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c325d-147">DateTimeOffset</span></span>|<span data-ttu-id="c325d-148">Время последнего изменения оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c325d-148">The time the management condition statement was last modified.</span></span> <span data-ttu-id="c325d-149">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="c325d-149">Updated service side.</span></span>|
|<span data-ttu-id="c325d-150">выражение</span><span class="sxs-lookup"><span data-stu-id="c325d-150">expression</span></span>|[<span data-ttu-id="c325d-151">манажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="c325d-151">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="c325d-152">Выражение оператора условия управления, используемое для оценки активации или деактивации оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c325d-152">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="c325d-153">eTag</span><span class="sxs-lookup"><span data-stu-id="c325d-153">eTag</span></span>|<span data-ttu-id="c325d-154">String</span><span class="sxs-lookup"><span data-stu-id="c325d-154">String</span></span>|<span data-ttu-id="c325d-155">Тег ETag оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c325d-155">ETag of the management condition statement.</span></span> <span data-ttu-id="c325d-156">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="c325d-156">Updated service side.</span></span>|
|<span data-ttu-id="c325d-157">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="c325d-157">applicablePlatforms</span></span>|<span data-ttu-id="c325d-158">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="c325d-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="c325d-159">Соответствующие платформы для этого оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c325d-159">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="c325d-160">Это рассчитывается на основе условий управления, связанных с оператором условия управления, и поиском пересечения соответствующих платформ.</span><span class="sxs-lookup"><span data-stu-id="c325d-160">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="c325d-161">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c325d-161">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="c325d-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="c325d-162">Response</span></span>
<span data-ttu-id="c325d-163">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c325d-163">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c325d-164">Пример</span><span class="sxs-lookup"><span data-stu-id="c325d-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="c325d-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="c325d-165">Request</span></span>
<span data-ttu-id="c325d-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c325d-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```

### <a name="response"></a><span data-ttu-id="c325d-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="c325d-167">Response</span></span>
<span data-ttu-id="c325d-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c325d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 491

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```




