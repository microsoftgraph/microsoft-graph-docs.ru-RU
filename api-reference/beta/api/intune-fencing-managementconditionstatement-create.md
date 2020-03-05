---
title: Создание Манажементкондитионстатемент
description: Создание нового объекта Манажементкондитионстатемент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 954218aa1493bac9a414142c2c9b8782499ccadc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465809"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="9f939-103">Создание Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="9f939-103">Create managementConditionStatement</span></span>

<span data-ttu-id="9f939-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9f939-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f939-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f939-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f939-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f939-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f939-107">Создание нового объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="9f939-107">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f939-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f939-108">Prerequisites</span></span>
<span data-ttu-id="9f939-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f939-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f939-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f939-111">Permission type</span></span>|<span data-ttu-id="9f939-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f939-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f939-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f939-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f939-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f939-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f939-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f939-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f939-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f939-116">Not supported.</span></span>|
|<span data-ttu-id="9f939-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f939-117">Application</span></span>|<span data-ttu-id="9f939-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f939-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f939-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f939-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="9f939-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9f939-120">Request headers</span></span>
|<span data-ttu-id="9f939-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f939-121">Header</span></span>|<span data-ttu-id="9f939-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9f939-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f939-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f939-123">Authorization</span></span>|<span data-ttu-id="9f939-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f939-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f939-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f939-125">Accept</span></span>|<span data-ttu-id="9f939-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f939-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f939-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f939-127">Request body</span></span>
<span data-ttu-id="9f939-128">В тексте запроса добавьте представление объекта Манажементкондитионстатемент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f939-128">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="9f939-129">В следующей таблице приведены свойства, необходимые при создании Манажементкондитионстатемент.</span><span class="sxs-lookup"><span data-stu-id="9f939-129">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="9f939-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f939-130">Property</span></span>|<span data-ttu-id="9f939-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9f939-131">Type</span></span>|<span data-ttu-id="9f939-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f939-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f939-133">id</span><span class="sxs-lookup"><span data-stu-id="9f939-133">id</span></span>|<span data-ttu-id="9f939-134">String</span><span class="sxs-lookup"><span data-stu-id="9f939-134">String</span></span>|<span data-ttu-id="9f939-135">Уникальный идентификатор оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="9f939-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="9f939-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="9f939-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="9f939-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9f939-137">displayName</span></span>|<span data-ttu-id="9f939-138">Строка</span><span class="sxs-lookup"><span data-stu-id="9f939-138">String</span></span>|<span data-ttu-id="9f939-139">Имя, определенное администратором оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="9f939-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="9f939-140">description</span><span class="sxs-lookup"><span data-stu-id="9f939-140">description</span></span>|<span data-ttu-id="9f939-141">String</span><span class="sxs-lookup"><span data-stu-id="9f939-141">String</span></span>|<span data-ttu-id="9f939-142">Заданное администратором описание оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="9f939-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="9f939-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f939-143">createdDateTime</span></span>|<span data-ttu-id="9f939-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f939-144">DateTimeOffset</span></span>|<span data-ttu-id="9f939-145">Время создания оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="9f939-145">The time the management condition statement was created.</span></span> <span data-ttu-id="9f939-146">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="9f939-146">Generated service side.</span></span>|
|<span data-ttu-id="9f939-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f939-147">modifiedDateTime</span></span>|<span data-ttu-id="9f939-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f939-148">DateTimeOffset</span></span>|<span data-ttu-id="9f939-149">Время последнего изменения оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="9f939-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="9f939-150">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="9f939-150">Updated service side.</span></span>|
|<span data-ttu-id="9f939-151">выражение</span><span class="sxs-lookup"><span data-stu-id="9f939-151">expression</span></span>|[<span data-ttu-id="9f939-152">манажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="9f939-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="9f939-153">Выражение оператора условия управления, используемое для оценки активации или деактивации оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="9f939-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="9f939-154">eTag</span><span class="sxs-lookup"><span data-stu-id="9f939-154">eTag</span></span>|<span data-ttu-id="9f939-155">String</span><span class="sxs-lookup"><span data-stu-id="9f939-155">String</span></span>|<span data-ttu-id="9f939-156">Тег ETag оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="9f939-156">ETag of the management condition statement.</span></span> <span data-ttu-id="9f939-157">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="9f939-157">Updated service side.</span></span>|
|<span data-ttu-id="9f939-158">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="9f939-158">applicablePlatforms</span></span>|<span data-ttu-id="9f939-159">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="9f939-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="9f939-160">Соответствующие платформы для этого оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="9f939-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="9f939-161">Это рассчитывается на основе условий управления, связанных с оператором условия управления, и поиском пересечения соответствующих платформ.</span><span class="sxs-lookup"><span data-stu-id="9f939-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="9f939-162">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="9f939-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="9f939-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f939-163">Response</span></span>
<span data-ttu-id="9f939-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f939-164">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f939-165">Пример</span><span class="sxs-lookup"><span data-stu-id="9f939-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f939-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f939-166">Request</span></span>
<span data-ttu-id="9f939-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f939-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f939-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f939-168">Response</span></span>
<span data-ttu-id="9f939-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f939-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





