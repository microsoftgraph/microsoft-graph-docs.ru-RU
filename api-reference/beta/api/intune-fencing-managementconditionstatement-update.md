---
title: Обновление managementConditionStatement
description: Обновление свойства объекта managementConditionStatement.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 02d5301ca81bf5b1479454f65a6c9e9630a8f284
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417044"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="7140a-103">Обновление managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="7140a-103">Update managementConditionStatement</span></span>

> <span data-ttu-id="7140a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7140a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7140a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7140a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7140a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7140a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7140a-107">Обновление свойства объекта [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="7140a-107">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7140a-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="7140a-108">Prerequisites</span></span>
<span data-ttu-id="7140a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7140a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7140a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7140a-111">Permission type</span></span>|<span data-ttu-id="7140a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7140a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7140a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7140a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7140a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7140a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7140a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7140a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7140a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7140a-116">Not supported.</span></span>|
|<span data-ttu-id="7140a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7140a-117">Application</span></span>|<span data-ttu-id="7140a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7140a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7140a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7140a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="7140a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7140a-120">Request headers</span></span>
|<span data-ttu-id="7140a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7140a-121">Header</span></span>|<span data-ttu-id="7140a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7140a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7140a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7140a-123">Authorization</span></span>|<span data-ttu-id="7140a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7140a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7140a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7140a-125">Accept</span></span>|<span data-ttu-id="7140a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7140a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7140a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7140a-127">Request body</span></span>
<span data-ttu-id="7140a-128">В тексте запроса укажите представление JSON для объекта [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="7140a-128">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="7140a-129">В следующей таблице показаны свойства, которые необходимы для создания [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span><span class="sxs-lookup"><span data-stu-id="7140a-129">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="7140a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7140a-130">Property</span></span>|<span data-ttu-id="7140a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7140a-131">Type</span></span>|<span data-ttu-id="7140a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7140a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7140a-133">id</span><span class="sxs-lookup"><span data-stu-id="7140a-133">id</span></span>|<span data-ttu-id="7140a-134">String</span><span class="sxs-lookup"><span data-stu-id="7140a-134">String</span></span>|<span data-ttu-id="7140a-135">Уникальный идентификатор для управления условная инструкция.</span><span class="sxs-lookup"><span data-stu-id="7140a-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="7140a-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="7140a-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="7140a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7140a-137">displayName</span></span>|<span data-ttu-id="7140a-138">String</span><span class="sxs-lookup"><span data-stu-id="7140a-138">String</span></span>|<span data-ttu-id="7140a-139">Имя оператора условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="7140a-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="7140a-140">description</span><span class="sxs-lookup"><span data-stu-id="7140a-140">description</span></span>|<span data-ttu-id="7140a-141">String</span><span class="sxs-lookup"><span data-stu-id="7140a-141">String</span></span>|<span data-ttu-id="7140a-142">Описание управления условная инструкция определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="7140a-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="7140a-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7140a-143">createdDateTime</span></span>|<span data-ttu-id="7140a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7140a-144">DateTimeOffset</span></span>|<span data-ttu-id="7140a-145">Время создания условная инструкция управления.</span><span class="sxs-lookup"><span data-stu-id="7140a-145">The time the management condition statement was created.</span></span> <span data-ttu-id="7140a-146">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="7140a-146">Generated service side.</span></span>|
|<span data-ttu-id="7140a-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7140a-147">modifiedDateTime</span></span>|<span data-ttu-id="7140a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7140a-148">DateTimeOffset</span></span>|<span data-ttu-id="7140a-149">Время последнего изменения условная инструкция управления.</span><span class="sxs-lookup"><span data-stu-id="7140a-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="7140a-150">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="7140a-150">Updated service side.</span></span>|
|<span data-ttu-id="7140a-151">выражение</span><span class="sxs-lookup"><span data-stu-id="7140a-151">expression</span></span>|[<span data-ttu-id="7140a-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="7140a-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="7140a-153">Выражение оператора условия управления, используется для оценки Если инструкции с условием управления был активирован деактивирован.</span><span class="sxs-lookup"><span data-stu-id="7140a-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="7140a-154">eTag</span><span class="sxs-lookup"><span data-stu-id="7140a-154">eTag</span></span>|<span data-ttu-id="7140a-155">String</span><span class="sxs-lookup"><span data-stu-id="7140a-155">String</span></span>|<span data-ttu-id="7140a-156">ETag условная инструкция управления.</span><span class="sxs-lookup"><span data-stu-id="7140a-156">ETag of the management condition statement.</span></span> <span data-ttu-id="7140a-157">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="7140a-157">Updated service side.</span></span>|
|<span data-ttu-id="7140a-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="7140a-158">applicablePlatforms</span></span>|<span data-ttu-id="7140a-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7140a-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="7140a-160">Применимые платформы для этой условная инструкция управления.</span><span class="sxs-lookup"><span data-stu-id="7140a-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="7140a-161">Отсчитывается от нужна условия управления, связанные с управлением условие оператора и поиск пересечения применимых платформ.</span><span class="sxs-lookup"><span data-stu-id="7140a-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="7140a-162">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="7140a-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="7140a-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="7140a-163">Response</span></span>
<span data-ttu-id="7140a-164">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7140a-164">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7140a-165">Пример</span><span class="sxs-lookup"><span data-stu-id="7140a-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="7140a-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="7140a-166">Request</span></span>
<span data-ttu-id="7140a-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7140a-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7140a-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="7140a-168">Response</span></span>
<span data-ttu-id="7140a-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7140a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




