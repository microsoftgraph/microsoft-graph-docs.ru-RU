---
title: Обновление Манажементкондитионстатемент
description: Обновление свойств объекта Манажементкондитионстатемент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ce39f9f7d3b8debce650b07a56dfe472a12c4879
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355488"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="4cabb-103">Обновление Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="4cabb-103">Update managementConditionStatement</span></span>

> <span data-ttu-id="4cabb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cabb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cabb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4cabb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cabb-106">Обновление свойств объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="4cabb-106">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cabb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4cabb-107">Prerequisites</span></span>
<span data-ttu-id="4cabb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cabb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cabb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cabb-110">Permission type</span></span>|<span data-ttu-id="4cabb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cabb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cabb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cabb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4cabb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cabb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4cabb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cabb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cabb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cabb-115">Not supported.</span></span>|
|<span data-ttu-id="4cabb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cabb-116">Application</span></span>|<span data-ttu-id="4cabb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cabb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cabb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cabb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="4cabb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cabb-119">Request headers</span></span>
|<span data-ttu-id="4cabb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4cabb-120">Header</span></span>|<span data-ttu-id="4cabb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4cabb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cabb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cabb-122">Authorization</span></span>|<span data-ttu-id="4cabb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cabb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cabb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4cabb-124">Accept</span></span>|<span data-ttu-id="4cabb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4cabb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cabb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4cabb-126">Request body</span></span>
<span data-ttu-id="4cabb-127">В тексте запроса добавьте представление объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cabb-127">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="4cabb-128">В следующей таблице приведены свойства, необходимые при создании [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md).</span><span class="sxs-lookup"><span data-stu-id="4cabb-128">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="4cabb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cabb-129">Property</span></span>|<span data-ttu-id="4cabb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4cabb-130">Type</span></span>|<span data-ttu-id="4cabb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4cabb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cabb-132">id</span><span class="sxs-lookup"><span data-stu-id="4cabb-132">id</span></span>|<span data-ttu-id="4cabb-133">String</span><span class="sxs-lookup"><span data-stu-id="4cabb-133">String</span></span>|<span data-ttu-id="4cabb-134">Уникальный идентификатор оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="4cabb-134">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="4cabb-135">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="4cabb-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="4cabb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4cabb-136">displayName</span></span>|<span data-ttu-id="4cabb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4cabb-137">String</span></span>|<span data-ttu-id="4cabb-138">Имя, определенное администратором оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="4cabb-138">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="4cabb-139">description</span><span class="sxs-lookup"><span data-stu-id="4cabb-139">description</span></span>|<span data-ttu-id="4cabb-140">String</span><span class="sxs-lookup"><span data-stu-id="4cabb-140">String</span></span>|<span data-ttu-id="4cabb-141">Заданное администратором описание оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="4cabb-141">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="4cabb-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4cabb-142">createdDateTime</span></span>|<span data-ttu-id="4cabb-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cabb-143">DateTimeOffset</span></span>|<span data-ttu-id="4cabb-144">Время создания оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="4cabb-144">The time the management condition statement was created.</span></span> <span data-ttu-id="4cabb-145">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="4cabb-145">Generated service side.</span></span>|
|<span data-ttu-id="4cabb-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4cabb-146">modifiedDateTime</span></span>|<span data-ttu-id="4cabb-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cabb-147">DateTimeOffset</span></span>|<span data-ttu-id="4cabb-148">Время последнего изменения оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="4cabb-148">The time the management condition statement was last modified.</span></span> <span data-ttu-id="4cabb-149">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="4cabb-149">Updated service side.</span></span>|
|<span data-ttu-id="4cabb-150">выражение</span><span class="sxs-lookup"><span data-stu-id="4cabb-150">expression</span></span>|[<span data-ttu-id="4cabb-151">манажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="4cabb-151">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="4cabb-152">Выражение оператора условия управления, используемое для оценки активации или деактивации оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="4cabb-152">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="4cabb-153">eTag</span><span class="sxs-lookup"><span data-stu-id="4cabb-153">eTag</span></span>|<span data-ttu-id="4cabb-154">String</span><span class="sxs-lookup"><span data-stu-id="4cabb-154">String</span></span>|<span data-ttu-id="4cabb-155">Тег ETag оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="4cabb-155">ETag of the management condition statement.</span></span> <span data-ttu-id="4cabb-156">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="4cabb-156">Updated service side.</span></span>|
|<span data-ttu-id="4cabb-157">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="4cabb-157">applicablePlatforms</span></span>|<span data-ttu-id="4cabb-158">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="4cabb-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="4cabb-159">Соответствующие платформы для этого оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="4cabb-159">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="4cabb-160">Это рассчитывается на основе условий управления, связанных с оператором условия управления, и поиском пересечения соответствующих платформ.</span><span class="sxs-lookup"><span data-stu-id="4cabb-160">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="4cabb-161">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4cabb-161">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="4cabb-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cabb-162">Response</span></span>
<span data-ttu-id="4cabb-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4cabb-163">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cabb-164">Пример</span><span class="sxs-lookup"><span data-stu-id="4cabb-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cabb-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cabb-165">Request</span></span>
<span data-ttu-id="4cabb-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cabb-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4cabb-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cabb-167">Response</span></span>
<span data-ttu-id="4cabb-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cabb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






