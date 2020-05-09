---
title: Создание Манажементкондитионстатемент
description: Создание нового объекта Манажементкондитионстатемент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0872c8c863a818b124337c4a04bc2b4e3cfe9e94
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177774"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="1565c-103">Создание Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="1565c-103">Create managementConditionStatement</span></span>

<span data-ttu-id="1565c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1565c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1565c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1565c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1565c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1565c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1565c-107">Создание нового объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="1565c-107">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1565c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1565c-108">Prerequisites</span></span>
<span data-ttu-id="1565c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1565c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1565c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1565c-111">Permission type</span></span>|<span data-ttu-id="1565c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1565c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1565c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1565c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1565c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1565c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1565c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1565c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1565c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1565c-116">Not supported.</span></span>|
|<span data-ttu-id="1565c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1565c-117">Application</span></span>|<span data-ttu-id="1565c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1565c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1565c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1565c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="1565c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1565c-120">Request headers</span></span>
|<span data-ttu-id="1565c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1565c-121">Header</span></span>|<span data-ttu-id="1565c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1565c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1565c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1565c-123">Authorization</span></span>|<span data-ttu-id="1565c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1565c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1565c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1565c-125">Accept</span></span>|<span data-ttu-id="1565c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1565c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1565c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1565c-127">Request body</span></span>
<span data-ttu-id="1565c-128">В тексте запроса добавьте представление объекта Манажементкондитионстатемент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1565c-128">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="1565c-129">В следующей таблице приведены свойства, необходимые при создании Манажементкондитионстатемент.</span><span class="sxs-lookup"><span data-stu-id="1565c-129">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="1565c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1565c-130">Property</span></span>|<span data-ttu-id="1565c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1565c-131">Type</span></span>|<span data-ttu-id="1565c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1565c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1565c-133">id</span><span class="sxs-lookup"><span data-stu-id="1565c-133">id</span></span>|<span data-ttu-id="1565c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1565c-134">String</span></span>|<span data-ttu-id="1565c-135">Уникальный идентификатор оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1565c-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="1565c-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="1565c-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="1565c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1565c-137">displayName</span></span>|<span data-ttu-id="1565c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="1565c-138">String</span></span>|<span data-ttu-id="1565c-139">Имя, определенное администратором оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1565c-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="1565c-140">description</span><span class="sxs-lookup"><span data-stu-id="1565c-140">description</span></span>|<span data-ttu-id="1565c-141">String</span><span class="sxs-lookup"><span data-stu-id="1565c-141">String</span></span>|<span data-ttu-id="1565c-142">Заданное администратором описание оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1565c-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="1565c-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1565c-143">createdDateTime</span></span>|<span data-ttu-id="1565c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1565c-144">DateTimeOffset</span></span>|<span data-ttu-id="1565c-145">Время создания оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1565c-145">The time the management condition statement was created.</span></span> <span data-ttu-id="1565c-146">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="1565c-146">Generated service side.</span></span>|
|<span data-ttu-id="1565c-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1565c-147">modifiedDateTime</span></span>|<span data-ttu-id="1565c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1565c-148">DateTimeOffset</span></span>|<span data-ttu-id="1565c-149">Время последнего изменения оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1565c-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="1565c-150">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="1565c-150">Updated service side.</span></span>|
|<span data-ttu-id="1565c-151">выражение</span><span class="sxs-lookup"><span data-stu-id="1565c-151">expression</span></span>|[<span data-ttu-id="1565c-152">манажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="1565c-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="1565c-153">Выражение оператора условия управления, используемое для оценки активации или деактивации оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1565c-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="1565c-154">eTag</span><span class="sxs-lookup"><span data-stu-id="1565c-154">eTag</span></span>|<span data-ttu-id="1565c-155">String</span><span class="sxs-lookup"><span data-stu-id="1565c-155">String</span></span>|<span data-ttu-id="1565c-156">Тег ETag оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1565c-156">ETag of the management condition statement.</span></span> <span data-ttu-id="1565c-157">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="1565c-157">Updated service side.</span></span>|
|<span data-ttu-id="1565c-158">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="1565c-158">applicablePlatforms</span></span>|<span data-ttu-id="1565c-159">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="1565c-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="1565c-160">Соответствующие платформы для этого оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1565c-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="1565c-161">Это рассчитывается на основе условий управления, связанных с оператором условия управления, и поиском пересечения соответствующих платформ.</span><span class="sxs-lookup"><span data-stu-id="1565c-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="1565c-162">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="1565c-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="1565c-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="1565c-163">Response</span></span>
<span data-ttu-id="1565c-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1565c-164">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1565c-165">Пример</span><span class="sxs-lookup"><span data-stu-id="1565c-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="1565c-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="1565c-166">Request</span></span>
<span data-ttu-id="1565c-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1565c-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1565c-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="1565c-168">Response</span></span>
<span data-ttu-id="1565c-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1565c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



