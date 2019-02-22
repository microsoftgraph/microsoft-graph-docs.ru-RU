---
title: Создание Манажементкондитионстатемент
description: Создание нового объекта Манажементкондитионстатемент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f19cef2899a11a57b06590c006de2181865a9d45
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156863"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="37d17-103">Создание Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="37d17-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="37d17-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37d17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37d17-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37d17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37d17-106">Создание нового объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="37d17-106">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37d17-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="37d17-107">Prerequisites</span></span>
<span data-ttu-id="37d17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="37d17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="37d17-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37d17-110">Permission type</span></span>|<span data-ttu-id="37d17-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37d17-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37d17-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37d17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37d17-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37d17-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37d17-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37d17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37d17-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37d17-115">Not supported.</span></span>|
|<span data-ttu-id="37d17-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37d17-116">Application</span></span>|<span data-ttu-id="37d17-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37d17-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37d17-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37d17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="37d17-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37d17-119">Request headers</span></span>
|<span data-ttu-id="37d17-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37d17-120">Header</span></span>|<span data-ttu-id="37d17-121">Значение</span><span class="sxs-lookup"><span data-stu-id="37d17-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37d17-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37d17-122">Authorization</span></span>|<span data-ttu-id="37d17-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="37d17-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37d17-124">Accept</span><span class="sxs-lookup"><span data-stu-id="37d17-124">Accept</span></span>|<span data-ttu-id="37d17-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37d17-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37d17-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37d17-126">Request body</span></span>
<span data-ttu-id="37d17-127">В тексте запроса добавьте представление объекта Манажементкондитионстатемент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37d17-127">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="37d17-128">В следующей таблице приведены свойства, необходимые при создании Манажементкондитионстатемент.</span><span class="sxs-lookup"><span data-stu-id="37d17-128">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="37d17-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="37d17-129">Property</span></span>|<span data-ttu-id="37d17-130">Тип</span><span class="sxs-lookup"><span data-stu-id="37d17-130">Type</span></span>|<span data-ttu-id="37d17-131">Описание</span><span class="sxs-lookup"><span data-stu-id="37d17-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37d17-132">id</span><span class="sxs-lookup"><span data-stu-id="37d17-132">id</span></span>|<span data-ttu-id="37d17-133">String</span><span class="sxs-lookup"><span data-stu-id="37d17-133">String</span></span>|<span data-ttu-id="37d17-134">Уникальный идентификатор оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="37d17-134">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="37d17-135">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="37d17-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="37d17-136">displayName</span><span class="sxs-lookup"><span data-stu-id="37d17-136">displayName</span></span>|<span data-ttu-id="37d17-137">String</span><span class="sxs-lookup"><span data-stu-id="37d17-137">String</span></span>|<span data-ttu-id="37d17-138">Имя, определенное администратором оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="37d17-138">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="37d17-139">description</span><span class="sxs-lookup"><span data-stu-id="37d17-139">description</span></span>|<span data-ttu-id="37d17-140">Строка</span><span class="sxs-lookup"><span data-stu-id="37d17-140">String</span></span>|<span data-ttu-id="37d17-141">Заданное администратором описание оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="37d17-141">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="37d17-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37d17-142">createdDateTime</span></span>|<span data-ttu-id="37d17-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37d17-143">DateTimeOffset</span></span>|<span data-ttu-id="37d17-144">Время создания оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="37d17-144">The time the management condition statement was created.</span></span> <span data-ttu-id="37d17-145">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="37d17-145">Generated service side.</span></span>|
|<span data-ttu-id="37d17-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37d17-146">modifiedDateTime</span></span>|<span data-ttu-id="37d17-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37d17-147">DateTimeOffset</span></span>|<span data-ttu-id="37d17-148">Время последнего изменения оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="37d17-148">The time the management condition statement was last modified.</span></span> <span data-ttu-id="37d17-149">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="37d17-149">Updated service side.</span></span>|
|<span data-ttu-id="37d17-150">выражение</span><span class="sxs-lookup"><span data-stu-id="37d17-150">expression</span></span>|[<span data-ttu-id="37d17-151">Манажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="37d17-151">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="37d17-152">Выражение оператора условия управления, используемое для оценки активации или деактивации оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="37d17-152">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="37d17-153">eTag</span><span class="sxs-lookup"><span data-stu-id="37d17-153">eTag</span></span>|<span data-ttu-id="37d17-154">String</span><span class="sxs-lookup"><span data-stu-id="37d17-154">String</span></span>|<span data-ttu-id="37d17-155">Тег ETag оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="37d17-155">ETag of the management condition statement.</span></span> <span data-ttu-id="37d17-156">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="37d17-156">Updated service side.</span></span>|
|<span data-ttu-id="37d17-157">Аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="37d17-157">applicablePlatforms</span></span>|<span data-ttu-id="37d17-158">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="37d17-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="37d17-159">Соответствующие платформы для этого оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="37d17-159">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="37d17-160">Это рассчитывается на основе условий управления, связанных с оператором условия управления, и поиском пересечения соответствующих платформ.</span><span class="sxs-lookup"><span data-stu-id="37d17-160">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="37d17-161">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="37d17-161">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="37d17-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="37d17-162">Response</span></span>
<span data-ttu-id="37d17-163">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37d17-163">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37d17-164">Пример</span><span class="sxs-lookup"><span data-stu-id="37d17-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="37d17-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="37d17-165">Request</span></span>
<span data-ttu-id="37d17-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37d17-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37d17-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="37d17-167">Response</span></span>
<span data-ttu-id="37d17-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37d17-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




