---
title: Обновление managementConditionStatement
description: Обновление свойства объекта managementConditionStatement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 800d40bda342ea23b55e7dc9bf62a99f1e41e3df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935418"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="a42c4-103">Обновление managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="a42c4-103">Update managementConditionStatement</span></span>

> <span data-ttu-id="a42c4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a42c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a42c4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a42c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a42c4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a42c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a42c4-107">Обновление свойства объекта [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="a42c4-107">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a42c4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a42c4-108">Prerequisites</span></span>
<span data-ttu-id="a42c4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a42c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a42c4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a42c4-111">Permission type</span></span>|<span data-ttu-id="a42c4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a42c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a42c4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a42c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a42c4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a42c4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a42c4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a42c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a42c4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a42c4-116">Not supported.</span></span>|
|<span data-ttu-id="a42c4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a42c4-117">Application</span></span>|<span data-ttu-id="a42c4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a42c4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a42c4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a42c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="a42c4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a42c4-120">Request headers</span></span>
|<span data-ttu-id="a42c4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a42c4-121">Header</span></span>|<span data-ttu-id="a42c4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a42c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a42c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a42c4-123">Authorization</span></span>|<span data-ttu-id="a42c4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a42c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a42c4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a42c4-125">Accept</span></span>|<span data-ttu-id="a42c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a42c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a42c4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a42c4-127">Request body</span></span>
<span data-ttu-id="a42c4-128">В тексте запроса укажите представление JSON для объекта [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="a42c4-128">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="a42c4-129">В следующей таблице показаны свойства, которые необходимы для создания [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span><span class="sxs-lookup"><span data-stu-id="a42c4-129">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="a42c4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a42c4-130">Property</span></span>|<span data-ttu-id="a42c4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a42c4-131">Type</span></span>|<span data-ttu-id="a42c4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a42c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a42c4-133">id</span><span class="sxs-lookup"><span data-stu-id="a42c4-133">id</span></span>|<span data-ttu-id="a42c4-134">String</span><span class="sxs-lookup"><span data-stu-id="a42c4-134">String</span></span>|<span data-ttu-id="a42c4-135">Уникальный идентификатор для управления условная инструкция.</span><span class="sxs-lookup"><span data-stu-id="a42c4-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="a42c4-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="a42c4-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="a42c4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a42c4-137">displayName</span></span>|<span data-ttu-id="a42c4-138">String</span><span class="sxs-lookup"><span data-stu-id="a42c4-138">String</span></span>|<span data-ttu-id="a42c4-139">Имя оператора условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="a42c4-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="a42c4-140">описание</span><span class="sxs-lookup"><span data-stu-id="a42c4-140">description</span></span>|<span data-ttu-id="a42c4-141">String</span><span class="sxs-lookup"><span data-stu-id="a42c4-141">String</span></span>|<span data-ttu-id="a42c4-142">Описание управления условная инструкция определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="a42c4-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="a42c4-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a42c4-143">createdDateTime</span></span>|<span data-ttu-id="a42c4-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a42c4-144">DateTimeOffset</span></span>|<span data-ttu-id="a42c4-145">Время создания условная инструкция управления.</span><span class="sxs-lookup"><span data-stu-id="a42c4-145">The time the management condition statement was created.</span></span> <span data-ttu-id="a42c4-146">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="a42c4-146">Generated service side.</span></span>|
|<span data-ttu-id="a42c4-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a42c4-147">modifiedDateTime</span></span>|<span data-ttu-id="a42c4-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a42c4-148">DateTimeOffset</span></span>|<span data-ttu-id="a42c4-149">Время последнего изменения условная инструкция управления.</span><span class="sxs-lookup"><span data-stu-id="a42c4-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="a42c4-150">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="a42c4-150">Updated service side.</span></span>|
|<span data-ttu-id="a42c4-151">выражение</span><span class="sxs-lookup"><span data-stu-id="a42c4-151">expression</span></span>|[<span data-ttu-id="a42c4-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="a42c4-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="a42c4-153">Выражение оператора условия управления, используется для оценки Если инструкции с условием управления был активирован деактивирован.</span><span class="sxs-lookup"><span data-stu-id="a42c4-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="a42c4-154">eTag</span><span class="sxs-lookup"><span data-stu-id="a42c4-154">eTag</span></span>|<span data-ttu-id="a42c4-155">String</span><span class="sxs-lookup"><span data-stu-id="a42c4-155">String</span></span>|<span data-ttu-id="a42c4-156">ETag условная инструкция управления.</span><span class="sxs-lookup"><span data-stu-id="a42c4-156">ETag of the management condition statement.</span></span> <span data-ttu-id="a42c4-157">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="a42c4-157">Updated service side.</span></span>|
|<span data-ttu-id="a42c4-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="a42c4-158">applicablePlatforms</span></span>|<span data-ttu-id="a42c4-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a42c4-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="a42c4-160">Применимые платформы для этой условная инструкция управления.</span><span class="sxs-lookup"><span data-stu-id="a42c4-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="a42c4-161">Отсчитывается от нужна условия управления, связанные с управлением условие оператора и поиск пересечения применимых платформ.</span><span class="sxs-lookup"><span data-stu-id="a42c4-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="a42c4-162">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="a42c4-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="a42c4-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="a42c4-163">Response</span></span>
<span data-ttu-id="a42c4-164">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a42c4-164">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a42c4-165">Пример</span><span class="sxs-lookup"><span data-stu-id="a42c4-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="a42c4-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="a42c4-166">Request</span></span>
<span data-ttu-id="a42c4-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a42c4-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
Content-type: application/json
Content-length: 256

{
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

### <a name="response"></a><span data-ttu-id="a42c4-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="a42c4-168">Response</span></span>
<span data-ttu-id="a42c4-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a42c4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





