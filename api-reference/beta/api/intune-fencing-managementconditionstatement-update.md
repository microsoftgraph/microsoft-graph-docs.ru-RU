---
title: Update managementConditionStatement
description: Обновление свойств объекта managementConditionStatement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 819d17f2884c1581a088646d4f3e107a32af78b0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153610"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="cf564-103">Update managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="cf564-103">Update managementConditionStatement</span></span>

<span data-ttu-id="cf564-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf564-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf564-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf564-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf564-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf564-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf564-107">Обновление свойств объекта [managementConditionStatement.](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="cf564-107">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf564-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf564-108">Prerequisites</span></span>
<span data-ttu-id="cf564-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf564-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf564-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf564-111">Permission type</span></span>|<span data-ttu-id="cf564-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf564-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf564-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf564-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf564-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf564-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf564-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf564-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf564-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf564-116">Not supported.</span></span>|
|<span data-ttu-id="cf564-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cf564-117">Application</span></span>|<span data-ttu-id="cf564-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf564-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf564-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf564-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="cf564-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cf564-120">Request headers</span></span>
|<span data-ttu-id="cf564-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf564-121">Header</span></span>|<span data-ttu-id="cf564-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf564-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf564-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf564-123">Authorization</span></span>|<span data-ttu-id="cf564-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf564-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf564-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf564-125">Accept</span></span>|<span data-ttu-id="cf564-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf564-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf564-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf564-127">Request body</span></span>
<span data-ttu-id="cf564-128">В теле запроса поставляем представление JSON для [объекта managementConditionStatement.](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="cf564-128">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="cf564-129">В следующей таблице показаны свойства, необходимые при создании [managementConditionStatement.](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="cf564-129">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="cf564-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf564-130">Property</span></span>|<span data-ttu-id="cf564-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cf564-131">Type</span></span>|<span data-ttu-id="cf564-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cf564-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf564-133">id</span><span class="sxs-lookup"><span data-stu-id="cf564-133">id</span></span>|<span data-ttu-id="cf564-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cf564-134">String</span></span>|<span data-ttu-id="cf564-135">Уникальный идентификатор для утверждения условий управления.</span><span class="sxs-lookup"><span data-stu-id="cf564-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="cf564-136">Созданное в системе значение, назначенное при его создания.</span><span class="sxs-lookup"><span data-stu-id="cf564-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="cf564-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cf564-137">displayName</span></span>|<span data-ttu-id="cf564-138">Строка</span><span class="sxs-lookup"><span data-stu-id="cf564-138">String</span></span>|<span data-ttu-id="cf564-139">Администратор определил имя заявления об условиях управления.</span><span class="sxs-lookup"><span data-stu-id="cf564-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="cf564-140">description</span><span class="sxs-lookup"><span data-stu-id="cf564-140">description</span></span>|<span data-ttu-id="cf564-141">Строка</span><span class="sxs-lookup"><span data-stu-id="cf564-141">String</span></span>|<span data-ttu-id="cf564-142">Администратор определил описание инструкции по состоянию управления.</span><span class="sxs-lookup"><span data-stu-id="cf564-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="cf564-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf564-143">createdDateTime</span></span>|<span data-ttu-id="cf564-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf564-144">DateTimeOffset</span></span>|<span data-ttu-id="cf564-145">Время создания заявления об условиях управления.</span><span class="sxs-lookup"><span data-stu-id="cf564-145">The time the management condition statement was created.</span></span> <span data-ttu-id="cf564-146">Сгенерированная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="cf564-146">Generated service side.</span></span>|
|<span data-ttu-id="cf564-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf564-147">modifiedDateTime</span></span>|<span data-ttu-id="cf564-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf564-148">DateTimeOffset</span></span>|<span data-ttu-id="cf564-149">Время последнего изменения состояния управления.</span><span class="sxs-lookup"><span data-stu-id="cf564-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="cf564-150">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="cf564-150">Updated service side.</span></span>|
|<span data-ttu-id="cf564-151">выражение</span><span class="sxs-lookup"><span data-stu-id="cf564-151">expression</span></span>|[<span data-ttu-id="cf564-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="cf564-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="cf564-153">Выражение заявления об условиях управления, используемое для оценки активации или отключения заявления об условиях управления.</span><span class="sxs-lookup"><span data-stu-id="cf564-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="cf564-154">eTag</span><span class="sxs-lookup"><span data-stu-id="cf564-154">eTag</span></span>|<span data-ttu-id="cf564-155">String</span><span class="sxs-lookup"><span data-stu-id="cf564-155">String</span></span>|<span data-ttu-id="cf564-156">ETag заявления об условиях управления.</span><span class="sxs-lookup"><span data-stu-id="cf564-156">ETag of the management condition statement.</span></span> <span data-ttu-id="cf564-157">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="cf564-157">Updated service side.</span></span>|
|<span data-ttu-id="cf564-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="cf564-158">applicablePlatforms</span></span>|<span data-ttu-id="cf564-159">[коллекция devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="cf564-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="cf564-160">Применимые платформы для этого утверждения условий управления.</span><span class="sxs-lookup"><span data-stu-id="cf564-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="cf564-161">Это рассчитывается из поиска условий управления, связанных с утверждением условий управления и поиска пересечения применимых платформ.</span><span class="sxs-lookup"><span data-stu-id="cf564-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="cf564-162">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="cf564-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="cf564-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf564-163">Response</span></span>
<span data-ttu-id="cf564-164">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cf564-164">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf564-165">Пример</span><span class="sxs-lookup"><span data-stu-id="cf564-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf564-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf564-166">Request</span></span>
<span data-ttu-id="cf564-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf564-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cf564-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf564-168">Response</span></span>
<span data-ttu-id="cf564-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf564-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




