---
title: Обновление Манажементкондитионстатемент
description: Обновление свойств объекта Манажементкондитионстатемент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7030fe6fcc821e8c20f3ec4c27809217322e7b0b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465704"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="c3429-103">Обновление Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="c3429-103">Update managementConditionStatement</span></span>

<span data-ttu-id="c3429-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c3429-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3429-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3429-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3429-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3429-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3429-107">Обновление свойств объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="c3429-107">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3429-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c3429-108">Prerequisites</span></span>
<span data-ttu-id="c3429-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3429-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3429-111">Permission type</span></span>|<span data-ttu-id="c3429-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3429-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3429-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3429-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3429-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3429-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3429-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3429-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3429-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3429-116">Not supported.</span></span>|
|<span data-ttu-id="c3429-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3429-117">Application</span></span>|<span data-ttu-id="c3429-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3429-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3429-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3429-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="c3429-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c3429-120">Request headers</span></span>
|<span data-ttu-id="c3429-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3429-121">Header</span></span>|<span data-ttu-id="c3429-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c3429-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3429-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3429-123">Authorization</span></span>|<span data-ttu-id="c3429-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3429-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3429-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3429-125">Accept</span></span>|<span data-ttu-id="c3429-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3429-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3429-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3429-127">Request body</span></span>
<span data-ttu-id="c3429-128">В тексте запроса добавьте представление объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3429-128">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="c3429-129">В следующей таблице приведены свойства, необходимые при создании [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md).</span><span class="sxs-lookup"><span data-stu-id="c3429-129">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="c3429-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3429-130">Property</span></span>|<span data-ttu-id="c3429-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c3429-131">Type</span></span>|<span data-ttu-id="c3429-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c3429-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3429-133">id</span><span class="sxs-lookup"><span data-stu-id="c3429-133">id</span></span>|<span data-ttu-id="c3429-134">String</span><span class="sxs-lookup"><span data-stu-id="c3429-134">String</span></span>|<span data-ttu-id="c3429-135">Уникальный идентификатор оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c3429-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="c3429-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="c3429-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="c3429-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c3429-137">displayName</span></span>|<span data-ttu-id="c3429-138">Строка</span><span class="sxs-lookup"><span data-stu-id="c3429-138">String</span></span>|<span data-ttu-id="c3429-139">Имя, определенное администратором оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c3429-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="c3429-140">description</span><span class="sxs-lookup"><span data-stu-id="c3429-140">description</span></span>|<span data-ttu-id="c3429-141">String</span><span class="sxs-lookup"><span data-stu-id="c3429-141">String</span></span>|<span data-ttu-id="c3429-142">Заданное администратором описание оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c3429-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="c3429-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3429-143">createdDateTime</span></span>|<span data-ttu-id="c3429-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3429-144">DateTimeOffset</span></span>|<span data-ttu-id="c3429-145">Время создания оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c3429-145">The time the management condition statement was created.</span></span> <span data-ttu-id="c3429-146">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="c3429-146">Generated service side.</span></span>|
|<span data-ttu-id="c3429-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3429-147">modifiedDateTime</span></span>|<span data-ttu-id="c3429-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3429-148">DateTimeOffset</span></span>|<span data-ttu-id="c3429-149">Время последнего изменения оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c3429-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="c3429-150">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="c3429-150">Updated service side.</span></span>|
|<span data-ttu-id="c3429-151">выражение</span><span class="sxs-lookup"><span data-stu-id="c3429-151">expression</span></span>|[<span data-ttu-id="c3429-152">манажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="c3429-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="c3429-153">Выражение оператора условия управления, используемое для оценки активации или деактивации оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c3429-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="c3429-154">eTag</span><span class="sxs-lookup"><span data-stu-id="c3429-154">eTag</span></span>|<span data-ttu-id="c3429-155">String</span><span class="sxs-lookup"><span data-stu-id="c3429-155">String</span></span>|<span data-ttu-id="c3429-156">Тег ETag оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c3429-156">ETag of the management condition statement.</span></span> <span data-ttu-id="c3429-157">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="c3429-157">Updated service side.</span></span>|
|<span data-ttu-id="c3429-158">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="c3429-158">applicablePlatforms</span></span>|<span data-ttu-id="c3429-159">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="c3429-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="c3429-160">Соответствующие платформы для этого оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="c3429-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="c3429-161">Это рассчитывается на основе условий управления, связанных с оператором условия управления, и поиском пересечения соответствующих платформ.</span><span class="sxs-lookup"><span data-stu-id="c3429-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="c3429-162">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c3429-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="c3429-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3429-163">Response</span></span>
<span data-ttu-id="c3429-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3429-164">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3429-165">Пример</span><span class="sxs-lookup"><span data-stu-id="c3429-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3429-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3429-166">Request</span></span>
<span data-ttu-id="c3429-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3429-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
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

### <a name="response"></a><span data-ttu-id="c3429-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3429-168">Response</span></span>
<span data-ttu-id="c3429-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3429-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





